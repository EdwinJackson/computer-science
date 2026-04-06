In machine learning, embedding is a way of representing data as points in space where the locations of those points in space are semantically meaningful. Embeddings are vectors or arrays of numbers that represent the meaning and the context of tokens processed by the model. They are used to encode and decode input and output texts and can vary in size and dimension.

Example in 3D
![[vectors-in-3d-space.png]]

_Words are plotted in 3-dimensional space. Embeddings can have hundreds or thousands of dimensions–too many for humans to visualize._

With Word2Vec, similar words cluster together in space–so the vector/point representing “king”, “queen” and “prince” will all cluster nearby. Same thing with synonyms (“walked,” “strolled,” “jogged”).

For other data types, it’s the same thing. A song embedding would plot similar-sounding songs nearby. An image embedding would plot similar-looking images nearby. A customer-embedding would plot customers with similar buying habits nearby. I could build a function, for example, that takes as input a word (i.e. “king”) and finds me its ten closest synonyms. This is called a "*nearest neighbour search*".

Not terribly interesting to do with single words, but imagine instead if we embedded whole movie plots. Then we could build a function that, given the synopsis of one movie, gives us ten similar movies. Or, given one news article, recommends semantically similar articles.

Individual words, as in the case of Word2Vec, but also entire sentences and chunks of text. One of the most popular open-source embedding models is called the [Universal Sentence Encoder](https://www.tensorflow.org/hub/tutorials/semantic_similarity_with_tf_hub_universal_encoder) (USE). The name is a bit misleading because USE can be used to encode not only sentences but also entire text chunks. Here’s a visual from the TensorFlow website. The heat map shows how similar different sentences are according to their distance in embedding space.
![[heat-map-vectorized-embeddings.png]]

The Universal Sentence Encoder model has tons of uses, especially when it comes to text search. That’s because USE embeddings capture sentence meanings rather than overfitting individual words.

### **Embeddings solve the [[encoding]] problem**

Embeddings are dense numerical representations of real-world objects and relationships, expressed as a vector. The vector space quantifies the semantic similarity between categories. Embedding vectors that are close to each other are considered similar. Sometimes, they are used directly for the “Similar items to this” section in an e-commerce store. Other times, embeddings are passed to other models. In those cases, the model can share learnings across similar items rather than treating them as two completely unique categories, as is the case with one-hot encodings. For this reason, embeddings can be used to accurately represent sparse data like clickstreams, text, and e-commerce purchases as features to downstream models. On the other hand, embeddings are much more expensive to compute than one-hot encodings and are far less interpretable.

### How are Embeddings created?

A common way to create an embedding requires us to first set up a supervised machine-learning problem. As a side-effect, training that model encodes categories into embedding vectors. For example, we can set up a model that predicts the next movie a user will watch based on what they are watching now. An embedding model will factorize the input into a vector, which will be used to predict the next movie. This means that similar vectors are movies that are commonly watched after similar movies. This makes for a great representation to be used for personalization. So even though we are solving a supervised problem, often called the surrogate problem, the actual creation of embeddings is an unsupervised process.

Defining a surrogate problem is an art, dramatically affecting the embeddings' behaviour. For example, YouTube’s recommender team realized that using the “predict the next video a user is going to click on” resulted in clickbait becoming rampantly recommended. They moved to “predict the next video and how long they are going to watch it” as a surrogate problem and achieved far better results.

Common Embedding Models
- 

[(1) Machine Learning's Most Useful Multitool: Embeddings - Dale on AI](https://daleonai.com/embeddings-explained)
[(2) Embeddings in Machine Learning: Everything You Need to Know](https://www.featureform.com/post/the-definitive-guide-to-embeddings)
[(3) Embedding - Wikipedia](https://en.wikipedia.org/wiki/Embedding)
[(4) LLM AI Embeddings | Microsoft Learn](https://learn.microsoft.com/en-us/semantic-kernel/concepts-ai/embeddings)
[(5) Embeddings | Machine Learning | Google Developers](https://developers.google.com/machine-learning/crash-course/embeddings/video-lecture)
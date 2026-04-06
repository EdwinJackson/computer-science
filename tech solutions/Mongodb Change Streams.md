[📖 Documentation ](https://www.mongodb.com/docs/kafka-connector/current/source-connector/fundamentals/change-streams/?tck=mongodb_ai_chatbot#change-streams-1)

Change streams are a MongoDB feature that allow you to receive real-time updates on data changes. Change streams return **change event documents**.

A change event document contains idempotent instructions to describe a change that occurred in your MongoDB deployment and metadata related to that change. Change event documents are generated from data in the [oplog.](https://www.mongodb.com/docs/manual/reference/glossary/#std-term-oplog)

> Important! **Change streams only run on MongoDB replica sets and sharded clusters. Standalone MongoDB instances cannot produce a change stream.**


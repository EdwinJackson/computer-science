Linear search is a simple algorithm that can be used to find an element in a list or an array. It works by iterating over each element of the list or array and comparing it with the target element. If the current element matches the target, the algorithm returns its index. If none of the elements match the target, the algorithm returns -1.

The main advantage of linear search is that it is easy to implement and does not require any preprocessing or sorting of the data. However, the main disadvantage is that it is inefficient for large or unsorted data sets. 

## Specs
|      | Time   | Space |
| ---- | ------ | ----- |
| Best | $O(n)$ | $O(1)$      |

The time complexity of the linear search is $O(n)$, where n is the number of elements in the list or array. This means that the worst-case scenario is that the algorithm has to check every element before finding the target or concluding that it does not exist. The space complexity of the linear search is $O(1)$, which means that it does not use any extra memory apart from the input data and a few variables.

## Implementation
```ts
const bandMembers = [
  { name: "Jisoo", number: "+82 06 0555 6666" },
  { name: "Jennie", number: "+82 06 0555 4444" },
  { name: "Rose", number: "+82 06 0555 3333" },
  { name: "Lisa", number: "+82 06 0555 2222" },
  { name: "RM", number: "+82 06 0555 1111" },
  { name: "J-Hope", number: "+82 06 0555 9999" },
  { name: "Suga", number: "+82 06 0555 8888" },
  { name: "Jimin", number: "+82 06 0555 7777" },
  { name: "V", number: "+82 06 0555 5555" },
  { name: "Jungkook", number: "+82 06 0555 0000" },
  { name: "IU", number: "+82 06 0555 1234" },
  { name: "Taeyeon", number: "+82 06 0555 2345" },
  { name: "G-Dragon", number: "+82 06 0555 3456" },
  { name: "Taeyang", number: "+82 06 0555 4567" },
  { name: "TOP", number: "+82 06 0555 5678" },
  { name: "Daesung", number: "+82 06 0555 6789" },
  { name: "Seungri", number: "+82 06 0555 7890" }
];

// the Array.prototype.find operation is an example of linear search
const jennie = bandMembers.find((contact) => contact.name === "Jennie")
sendTextMessage(jennie, "Band practice started 43 seconds ago!")
```

## Relates To
- [[Order & Search]]
- [[Binary Search]]
- [[Selection Sort]]
Binary search is a search algorithm that finds the position of a target value within a sorted array. It works by repeatedly dividing the array into two halves, and comparing the target value with the middle element of each half. If the target value is equal to the middle element, then the position is found. If the target value is smaller than the middle element, then the search continues in the left half of the array. If the target value is larger than the middle element, then the search continues in the right half of the array. This process repeats until either the target value is found or the array is empty.

## Spec

Binary search is an efficient algorithm because it eliminates half of the possible elements in each iteration. The time complexity of binary search is O(log n), where n is the number of elements in the array. The space complexity of binary search is O(1), because it only requires a constant amount of extra space to store the indices of the left and right halves.

## Implementation

```ts
interface BandMember {
  name: string;
  number: string;
}

const bandMembers: BandMember[] = [
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

function binarySearch(bandMembers: BandMember[], targetName: string, left: number, right: number): BandMember | undefined {
  if (left >= right) {
    return undefined;
  }

  const mid = Math.floor((left + right) / 2);
  const midName = bandMembers[mid].name;

  if (midName === targetName) {
    return bandMembers[mid];
  } else if (midName < targetName) {
    return binarySearch(bandMembers, targetName, mid + 1, right);
  } else {
    return binarySearch(bandMembers, targetName, left, mid - 1);
  }
}

// Sort the bandMembers array by name
bandMembers.sort((a, b) => a.name.localeCompare(b.name));

const targetName = "Taeyang";
const result = binarySearch(bandMembers, targetName, 0, bandMembers.length - 1);
console.log(result); // Output: { name: "Taeyang", number: "+82 06 0555 4567" }
```

- The `binarySearch` function takes parameters: `bandMembers`, `targetName`, `left`, and `right`.
- `left`, and `right`, represent the left and right boundaries of the search space within the `bandMembers` array.
- The function checks if `left` is greater or equal to `right`, which indicates that the search space is empty, and returns `undefined` in that case.
- The function calculates the `mid` index as the average of `left` and `right`, and retrieves the corresponding name of the band member from the array.
- If the `midName` is equal to the `targetName`, the band member object is found and returned.
- If the `midName` is less than the `targetName`, it means the desired band member is in the **right half** of the remaining array, so the `binarySearch` function is recursively called with the 
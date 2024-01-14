```ts
/**

Do not return anything, modify nums in-place instead.

*/

function rotate(nums: number[], k: number): void {

const pivot = k % nums.length

let left = 0

let right = nums.length - 1

  

reverse(nums, left, right)

  

left = 0

right = pivot - 1

reverse(nums, left, right)

  

left = pivot

right = nums.length - 1

reverse(nums, left, right)

};

  

function reverse(nums: number[], left: number, right: number): void {

while(left < right) {

const temp = nums[left]

nums[left] = nums[right]

nums[right] = temp

left++

right--

}

}
```
# Notes
- Rotating the an array by k, is the same as performing the following steps
	- reversing the entire array
	- Finding the pivot which is k % array.length
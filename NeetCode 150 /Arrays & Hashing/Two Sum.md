## Question
[Two Sum](https://leetcode.com/problems/two-sum/)




## Solution

### Brute-Force
1. Using two loops we will iterate over the array and check if the sum is equal to target.
2. if we found two such indecies where sum == target store them in the ans array,
3. ans[0] = i.  ans[1] = j.
4. return the ans.

TC - O(N<sup>2</sup>).
SC - O(1).

### Approach 2
1. Sort the array, place two pointer 1 at start and 1 at end
2. As the array is sorted, we have elements with more magnitude at the end and lighter elements at the start.
3. Calculate sum of your placed pointers and check if sum > target or sum < target.
4. if sum > target , decrement the right pointer and calculate sum again.
5. if sum < taget, decrement left pointer.
6. Once we found the sum store indecies i and j and return the ans.

   TC - O(NlogN).
   SC - O(1).


### Optimal Approach
We can easily solve this in O(N) time complexity using HashMap or HashSet. We will use HashMap here because we have to store index of the value. 

1. Iterate over the array and check if our map contains the value (target - nums[i])(TC - O(1))
2. If yes, then get the index if that value and and our current index and store this in ans array.
3. If No, then put the current index element in the map with the index as its value.

  TC - O(N).
  SC - O(N).


# Question

[Group Anagram](https://leetcode.com/problems/group-anagrams/)


# Solution

An Anagram is a word or phrase formed by rearranging the letters of a different word or phrase, typically using all the original letters exactly once.

Intution to solve this question is to group words with same character frequency togther. We can do this using Hashmap. 
To have character count in each letter create a Array of size 26 and for every string in the input array and put it in the the Hashmap as key.
Now, put the current string in the same key.

T.C - O(N)
S.C - O(N)


# Question 
[Top K frequent Elements](https://leetcode.com/problems/top-k-frequent-elements/description/)


# Solution 

We have to sort elements on the basis of frequency, so first we will make a frequency hashmap then make a pair of element with its frequency and
sort this pair on basis of descending frequency. Then we will return top k elements from our sorted array. 

T.C - O(N logN)
S.C - O(N)



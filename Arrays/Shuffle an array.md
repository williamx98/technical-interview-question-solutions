# Shuffle an array 

[Question Link](https://leetcode.com/problems/shuffle-an-array/)  

Shuffle a set of numbers without duplicates.  

##### Constraints:

### Explanation:
TLDR: 

### Notes:


## Solution:
```Python
class Solution(object):

    def __init__(self, nums):
        """
        :type nums: List[int]
        """
        self.data = nums

    def reset(self):
        """
        Resets the array to its original configuration and return it.
        :rtype: List[int]
        """
        return self.data

    def shuffle(self):
        """
        """
        Returns a random shuffling of the array.
        :rtype: List[int]
        """
        copy = list(copy)
        for i in range(len(copy)):
            swap = random.randrange(i, len(copy))
            temp = copy[swap]
            copy[swap] = copy[i]
            copy[i] = temp
            
        return copy
```
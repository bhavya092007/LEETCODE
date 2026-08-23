# LeetCode Java Solutions & Explanations

---

## 1. Restore String (Shuffle String)

### Problem Summary
Given a string `s` and an integer array `indices` of the same length, restore the shuffled string such that the character at the $i^{\text{th}}$ position moves to `indices[i]` in the shuffled string.

### Solution
```java
class Solution {
    public String restoreString(String s, int[] indices) {
        int n = s.length();
        
        // 1. Create a character array of the same length to store the restored characters
        char[] ans = new char[n];
        
        // 2. Iterate through each character of the original string
        for (int i = 0; i < n; i++) {
            // Place the character at its target index:
            // s.charAt(i) belongs at position indices[i] in the result
            ans[indices[i]] = s.charAt(i);
        }
        
        // 3. Convert the character array back into a String and return
        return new String(ans);
    }
}
```

### Complexity
* **Time Complexity:** $O(N)$ — Single pass through the string of length $N$.
* **Space Complexity:** $O(N)$ — Memory allocated for the output character array.

---

## 2. Build Array from Permutation

### Problem Summary
Given a zero-based permutation `nums` (0-indexed), build an array `ans` of the same length where `ans[i] = nums[nums[i]]` for each $0 \le i < \text{nums.length}$.

### Solution
```java
class Solution {
    public int[] buildArray(int[] nums) {
        int n = nums.length;
        
        // 1. Create a new array of the same size to store the transformed values
        int[] ans = new int[n];
        
        // 2. Iterate through each index of the input array
        for (int i = 0; i < n; i++) {
            // Map each index according to the permutation rule: ans[i] = nums[nums[i]]
            ans[i] = nums[nums[i]];
        }
        
        // 3. Return the newly built array
        return ans;
    }
}
```

### Complexity
* **Time Complexity:** $O(N)$ — Single pass across the array.
* **Space Complexity:** $O(N)$ — Output array of size $N$ ($O(1)$ auxiliary space).

---

## 3. How Many Numbers Are Smaller Than the Current Number

### Problem Summary
Given an array `nums`, for each `nums[i]` find out how many numbers in the array are strictly smaller than it.

### Solution (Brute Force - $O(N^2)$)
```java
class Solution {
    public int[] smallerNumbersThanCurrent(int[] nums) {
        int n = nums.length;
        int count[] = new int[n];
        
        // Nested loop comparing all pairs
        for (int i = 0; i < n; i++) {
            for (int j = 0; j < n; j++) {
                if (nums[i] > nums[j]) {
                    count[i]++;
                }
            }
        }
        return count;
    }
}
```

### Optimal Solution (Bucket / Counting Sort - $O(N)$)
```java
class Solution {
    public int[] smallerNumbersThanCurrent(int[] nums) {
        // 1. Bucket array for value frequencies (LeetCode constraint: 0 <= nums[i] <= 100)
        int[] bucket = new int[101];
        
        // 2. Count the frequency of each number in nums
        for (int num : nums) {
            bucket[num]++;
        }
        
        // 3. Compute running prefix sums:
        // bucket[i] becomes the total count of numbers strictly smaller than i
        int runningCount = 0;
        for (int i = 0; i < bucket.length; i++) {
            int temp = bucket[i];          // Store current number's frequency
            bucket[i] = runningCount;      // Elements strictly smaller than i
            runningCount += temp;          // Update running total for next values
        }
        
        // 4. Map each original element to its precomputed count
        int[] ans = new int[nums.length];
        for (int i = 0; i < nums.length; i++) {
            ans[i] = bucket[nums[i]];
        }
        
        return ans;
    }
}
```

### Complexity (Optimal)
* **Time Complexity:** $O(N)$ — Linear scan to count frequencies and build the output array.
* **Space Complexity:** $O(1)$ — Fixed-size bucket array of 101 elements.

---

## 4. Find Numbers with Even Number of Digits

### Problem Summary
Given an array `nums` of integers, return how many of them contain an even number of digits.

### Solution (Loop-Based Digit Count)
```java
class Solution {
    public int findNumbers(int[] nums) {
        int ans = 0;

        for (int i = 0; i < nums.length; i++) {
            int digits = 0;
            int num = nums[i];

            // Count digits by successive division
            while (num != 0) {
                num /= 10;
                digits++;
            }

            if (digits % 2 == 0) {
                ans++;
            }
        }
        return ans;
    }
}
```

### Optimal Solution (Logarithmic $O(1)$ Digit Count)
```java
class Solution {
    public int findNumbers(int[] nums) {
        int ans = 0;

        for (int num : nums) {
            // Math.log10(num) + 1 gives the exact number of digits for any positive integer
            int digits = (int) Math.log10(num) + 1;

            if (digits % 2 == 0) {
                ans++;
            }
        }
        return ans;
    }
}
```

### Complexity (Optimal)
* **Time Complexity:** $O(N)$ — Single pass; calculating digits takes $O(1)$ mathematical operations.
* **Space Complexity:** $O(1)$ — Constant auxiliary space.

---

## 5. Shuffle the Array

### Problem Summary
Given the array `nums` consisting of $2n$ elements in the form $[x_1, x_2, \dots, x_n, y_1, y_2, \dots, y_n]$, return the array in the form $[x_1, y_1, x_2, y_2, \dots, x_n, y_n]$.

### Solution
```java
class Solution {
    public int[] shuffle(int[] nums, int n) {
        // 1. Result array of total size 2n
        int[] array = new int[2 * n];
        int k = 0;

        // 2. Interleave elements from the first half [0..n-1] and second half [n..2n-1]
        for (int i = 0; i < n; i++) {
            array[k++] = nums[i];      // Place x_i
            array[k++] = nums[i + n];  // Place y_i
        }

        return array;
    }
}
```

### Complexity
* **Time Complexity:** $O(n)$ — Traverses $n$ steps to populate all $2n$ elements.
* **Space Complexity:** $O(n)$ — Allocates output array of size $2n$.

---

## 6. Kids With the Greatest Number of Candies

### Problem Summary
There are $n$ kids with candies. You are given an integer array `candies`, where each `candies[i]` represents the number of candies the $i^{\text{th}}$ kid has, and an integer `extraCandies`. Return a boolean array of length $n$, where `result[i]` is `true` if, after giving the $i^{\text{th}}$ kid all `extraCandies`, they will have the greatest number of candies among all the kids.

### Solution
```java
class Solution {
    public List<Boolean> kidsWithCandies(int[] candies, int extraCandies) {
        int max = 0;
        List<Boolean> list = new ArrayList<>();

        // 1. Find the current maximum candies among all kids
        for (int j = 0; j < candies.length; j++) {
            if (candies[j] > max) {
                max = candies[j];
            }
        }

        // 2. Check if current kid + extraCandies can reach or exceed the maximum
        for (int i = 0; i < candies.length; i++) {
            int total = candies[i] + extraCandies;
            if (total >= max) {
                list.add(true);
            } else {
                list.add(false);
            }
        }

        return list;
    }
}
```

### Complexity
* **Time Complexity:** $O(N)$ — Two linear passes over the array.
* **Space Complexity:** $O(N)$ — Return list size of $N$ ($O(1)$ auxiliary space).

---

## 7. Find the Highest Altitude

### Problem Summary
There is a biker going on a road trip starting at point 0 with altitude 0. Given an integer array `gain` of length $n$ where `gain[i]` is the net gain in altitude between points $i$ and $i + 1$, return the highest altitude of a point.

### Approach 1: Prefix Array ($O(N)$ Space)
```java
class Solution {
    public int largestAltitude(int[] gain) {
        int altitude = 0;
        int max = 0;
        int[] alt = new int[gain.length + 1];
        
        // 1. Calculate prefix sums of altitudes
        for (int i = 0; i < gain.length; i++) {
            altitude += gain[i];
            alt[i + 1] = altitude;
        }

        // 2. Find the maximum altitude recorded
        for (int j = 0; j < alt.length; j++) {
            if (alt[j] > max) {
                max = alt[j];
            }
        }
        return max;
    }
}
```

### Approach 2: Single Pass In-Place ($O(1)$ Space)
```java
class Solution {
    public int largestAltitude(int[] gain) {
        int max = 0;
        int current = 0;

        // Track running altitude and update maximum on the fly
        for (int i = 0; i < gain.length; i++) {
            current += gain[i];
            max = Math.max(current, max);
        }

        return max;
    }
}
```

### Complexity (Optimal)
* **Time Complexity:** $O(N)$ — Single pass through `gain`.
* **Space Complexity:** $O(1)$ — Only two scalar variables used.

---

## 8. Squares of a Sorted Array

### Problem Summary
Given an integer array `nums` sorted in non-decreasing order, return an array of the squares of each number sorted in non-decreasing order.

### Solution (Square + Bubble Sort)
```java
class Solution {
    public int[] sortedSquares(int[] nums) {
        int n = nums.length;
        int[] sqr = new int[n];
        int temp;

        // 1. Square every element
        for (int i = 0; i < n; i++) {
            sqr[i] = nums[i] * nums[i];
        }

        // 2. Bubble Sort the squared array
        for (int j = 0; j < sqr.length - 1; j++) {
            for (int k = 0; k < sqr.length - j - 1; k++) {
                if (sqr[k] > sqr[k + 1]) {
                    temp = sqr[k];
                    sqr[k] = sqr[k + 1];
                    sqr[k + 1] = temp;
                }
            }
        }
        return sqr;
    }
}
```

### Complexity
* **Time Complexity:** $O(N^2)$ — Due to Bubble Sort passes.
* **Space Complexity:** $O(N)$ — Extra array `sqr` to store squared numbers.

---

## 9. Max Consecutive Ones

### Problem Summary
Given a binary array `nums`, return the maximum number of consecutive 1's in the array.

### Solution
```java
class Solution {
    public int findMaxConsecutiveOnes(int[] nums) {
        int current = 0; // Tracks running consecutive 1s
        int max = 0;     // Stores maximum streak

        for (int i = 0; i < nums.length; i++) {
            if (nums[i] == 1) {
                current++;
                if (current > max) {
                    max = current;
                }
            } else {
                // Reset streak on encounter of 0
                current = 0;
            }
        }
        return max;
    }
}
```

### Complexity
* **Time Complexity:** $O(N)$ — Single scan through `nums`.
* **Space Complexity:** $O(1)$ — Auxiliary constant space.

---

## 10. Third Maximum Number

### Problem Summary
Given an integer array `nums`, return the third distinct maximum number in this array. If the third maximum does not exist, return the maximum number.

### Solution (Bubble Sort + Backward Distinct Scan)
```java
class Solution {
    public int thirdMax(int[] nums) {
        int temp;
        int count = 1; // Count of distinct maximums found

        // 1. Sort array in ascending order using Bubble Sort
        for (int i = 0; i < nums.length - 1; i++) {
            for (int j = 0; j < nums.length - i - 1; j++) {
                if (nums[j] > nums[j + 1]) {
                    temp = nums[j];
                    nums[j] = nums[j + 1];
                    nums[j + 1] = temp;
                }
            }
        }

        // 2. Scan backward to find the 3rd distinct maximum
        for (int k = nums.length - 1; k > 0; k--) {
            if (nums[k] != nums[k - 1]) {
                count++;
            } else {
                continue;
            }

            if (count == 3) {
                return nums[k - 1];
            }
        }

        // 3. Fallback: return the largest element if fewer than 3 distinct values exist
        return nums[nums.length - 1];
    }
}
```

### Complexity
* **Time Complexity:** $O(N^2)$ — Dominated by Bubble Sort.
* **Space Complexity:** $O(1)$ — In-place array operations.

---

## 11. Remove Duplicates from Sorted Array

### Problem Summary
Given an integer array `nums` sorted in non-decreasing order, remove the duplicates in-place such that each unique element appears only once. Return the number of unique elements `k`.

### Solution (Two Pointers)
```java
class Solution {
    public int removeDuplicates(int[] nums) {
        if (nums.length == 0) return 0;
        
        // 1. Pointer 'k' tracks where the next unique element should be placed
        int k = 1;
     
        // 2. Fast pointer 'i' scans elements from index 1
        for (int i = 1; i < nums.length; i++) {
            // When a new distinct value is encountered:
            if (nums[i] != nums[i - 1]) {
                nums[k] = nums[i]; // Write unique element to index k
                k++;               // Advance placement boundary
            }
        }
        
        // 3. Return total count of unique elements
        return k;
    }
}
```

### Complexity
* **Time Complexity:** $O(N)$ — Single pass through the sorted array.
* **Space Complexity:** $O(1)$ — Modifies array strictly in-place.

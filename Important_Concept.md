### Key Concept

This pattern is commonly used to find the **maximum element** in an array or collection.

```java
if(current > max)
{
    max = current;
}

Frequency Array Rule:

freq[s.charAt(i) - 'a']++

means

"Increase the count of the current character."

# Enhanced For Loop vs Normal For Loop in Java

## Enhanced For Loop (For-Each Loop)

```java
for(int num : nums) {
    // code
}
```

### Meaning

- `nums` = array
- `num` = current element of the array

The loop automatically takes each value from `nums` one by one.

Example:

```java
int[] nums = {10, 20, 30};

for(int num : nums) {
    System.out.println(num);
}
```

Output:

```text
10
20
30
```

---

## Expanded Version

The above loop is equivalent to:

```java
for(int i = 0; i < nums.length; i++) {
    int num = nums[i];

    // same code
}
```

### Breakdown

```java
int i = 0;
```

Start from index 0.

```java
i < nums.length;
```

Continue until the last index.

```java
i++;
```

Move to the next index.

```java
int num = nums[i];
```

Store the current element in `num`.

---

## Example

```java
int[] nums = {10, 20, 30};

for(int i = 0; i < nums.length; i++) {
    int num = nums[i];
    System.out.println(num);
}
```

Output:

```text
10
20
30
```

---

## When to Use Each

### Use Enhanced For Loop

```java
for(int num : nums)
```

When you only need the value.

Examples:
- Sum of array
- Finding duplicates
- Finding maximum value

### Use Normal For Loop

```java
for(int i = 0; i < nums.length; i++)
```

When you need the index.

Examples:
- Two Sum
- Contains Duplicate II
- Accessing neighboring elements
- Updating array values by index

---

## Memory Trick

```text
for(int num : nums)
```

Read as:

"For every number num in nums"

```text
for(int i = 0; i < nums.length; i++)
```

Read as:

"For every index i in nums"
```


# Day 12 - Binary Search Notes

Date: 28-07-2026

Problems Solved:
- 278 - First Bad Version
- 374 - Guess Number Higher or Lower
- 852 - Peak Index in a Mountain Array


## Binary Search

Binary Search is an algorithm that reduces the search space by half in every step.

Instead of checking every element:

O(n)

Binary Search removes half of the possible answers:

O(log n)


Main Question:

"After checking the middle element, can I remove half of the possibilities?"


If yes, Binary Search can be applied.


---

## O(log n) Understanding

O(log n) means repeatedly dividing the input size by 2.


Example:

n = 16

16 → 8 → 4 → 2 → 1


Only 4 operations are required.


Important:

Number of loops does not decide complexity.

The way the value changes decides complexity.


Example:

i++

Usually O(n)


i = i / 2

Usually O(log n)



---

## Mid Calculation


## Important Concepts Learned Today

### Linked List Concepts

#### 1. Dummy Node Pattern

```java
ListNode dummy = new ListNode(-1);
```

Purpose:

```text
Creates a safe starting point for building a new linked list.
Avoids special handling of the first node.
```

---

#### 2. Tail Pointer

```java
ListNode tail = dummy;
```

Purpose:

```text
Always points to the last node
of the merged linked list.
```

Pattern:

```java
tail.next = node;
tail = tail.next;
```

---

#### 3. ListNode Reference Understanding

```java
tail.next = list1;
```

Learning:

```text
We are attaching existing nodes,
not creating new ones.
```

---

#### 4. Linked Lists Do Not Have

```java
head.length
head[i]
```

Important reminder:

```text
Linked Lists use references,
not indexing.
```

---

### Binary Search Concepts

#### 5. O(log n) Hint

Learning:

```text
Whenever I see O(log n),
I should immediately think about Binary Search.
```

---

#### 6. Overflow Safe Mid Calculation

Instead of:

```java
int mid = (start + end) / 2;
```

Use:

```java
int mid = start + (end - start) / 2;
```

Reason:

```text
Avoids integer overflow.
```

---

#### 7. Rotated Array Observation

Learning:

```text
Even if the whole array is not sorted,
at least one half is always sorted.
```

Example:

```text
4 5 6 7 | 0 1 2
```

Left half is sorted.

---

#### 8. Detecting Sorted Half

```java
nums[start] <= nums[mid]
```

Meaning:

```text
Left half is sorted.
```

Otherwise:

```text
Right half is sorted.
```

---

#### 9. Range Checking

Instead of directly comparing:

```java
nums[mid] < target
```

Learned to check:

```java
target >= nums[start]
&&
target < nums[mid]
```

This determines whether the target lies inside the sorted half.

---

### Problem Solving Concepts

#### 10. Pattern Recognition

Learning:

```text
Do not immediately think about code.

First identify:

Which pattern is this?
```

Examples:

```text
Linked List
→ Pointer Manipulation

O(log n)
→ Binary Search

Merge Two Sorted Lists
→ Merge Pattern
```

---

#### 11. Thinking Mistake Identified

Today I noticed that I often:

```text
Jump into coding
before fully understanding the logic.
```

Need to improve:

```text
Understand pattern first
↓
Dry run example
↓
Then code
```

---

#### 12. Small Win

I independently recognized:

```text
O(log n)
→ Binary Search
```

This shows my pattern recognition is improving.

---

### Keywords Added To My Toolkit

```text
Dummy Node
Tail Pointer
Reference Manipulation
Merge Pattern
Rotated Binary Search
Sorted Half Detection
Range Checking
Pattern Recognition
Overflow Safe Mid
```


Correct Binary Search mid formula:


```java
int mid = start + (end - start) / 2;

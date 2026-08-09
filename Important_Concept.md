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


## Important Concepts Gained Today

### HashSet Basics

Today was my first practical use of HashSet in a LeetCode problem.

Learned:

```java
HashSet<Integer> set = new HashSet<>();
```

Useful methods:

```java
add()
contains()
size()
```

---

### Fast Lookup

I learned that HashSet allows quick checking of whether an element exists.

```java
set.contains(value)
```

This avoids unnecessary nested loops.

---

### Unique Elements

HashSet automatically removes duplicates.

Example:

```java
set.add(2);
set.add(2);
set.add(2);
```

Result:

```text
[2]
```

This perfectly matched the requirement of the Intersection problem.

---

### Collection vs Array

Today I understood that:

```text
HashSet<Integer>
```

and

```text
int[]
```

are completely different types.

A collection cannot be returned directly when the function expects an array.

---

### HashSet → Array Conversion

Learned how to convert:

```text
HashSet<Integer>
```

into:

```text
int[]
```

before returning the final answer.

---

### Pattern Learned

```text
Store values
↓
Fast lookup using contains()
↓
Collect unique answers
↓
Convert to required format
```

This is my first HashSet-based problem-solving pattern.

---

### Constraint-Based Thinking

From LeetCode 877 (Stone Game), I learned:

```text
Sometimes the entire solution
comes from understanding the constraints.
```

Not every accepted solution requires a complex algorithm.

Sometimes:

```java
return true;
```

is enough.

## Important Concepts Learned Today

### 1. Binary Search Is Not Only For Finding a Target

Before today:

```text
Binary Search = Find Target
```

After today:

```text
Binary Search = Find Position
```

It can be used for:

- First Bad Version
- Search Insert Position
- Smallest Greater Element
- Lower Bound
- Upper Bound

---

### 2. Smallest Greater Element Pattern

Learned how to find:

```text
The first element greater than target
```

using Binary Search.

Pattern:

```java
if(arr[mid] > target)
{
    end = mid - 1;
}
else
{
    start = mid + 1;
}
```

---

### 3. Wrap-Around Logic

Learned a very clever trick:

```java
start % length
```

Example:

```java
4 % 4 = 0
```

Used when the answer should return to the beginning of the array.

---

### 4. Final Position Binary Search

A new realization:

```text
Sometimes we don't need an answer variable.
```

After Binary Search finishes:

```java
start
```

itself can represent the answer position.

---

### 5. Recursion Basics

First proper understanding of recursion.

Core idea:

```text
Solve smaller versions
of the same problem.
```

---

### 6. Base Case

Most important part of recursion.

Example:

```java
if(n <= 1)
{
    return n;
}
```

Without a base case:

```text
Recursion never stops.
```

---

### 7. Recursive Thinking

Learned to think:

```text
What is the smallest version
of this problem?
```

instead of trying to understand the entire recursion tree at once.

---

### 8. Fibonacci Pattern

Learned:

```java
fib(n) = fib(n-1) + fib(n-2)
```

Current problem depends on:

```text
Previous two answers.
```

This is an early introduction to Dynamic Programming thinking.

---

### 9. Growth Observation

Today's shift:

```text
Earlier:
Focus on syntax

Now:
Focus on logic and patterns
```

Examples:

```text
Why move left?
Why move right?
Why recursion stops?
Why Binary Search works?
```

This is an important improvement in problem-solving ability.

# Day 19 – Important Concepts

## 1. Fast Power / Binary Exponentiation

### Core Idea

Instead of:

```text
x × x × x × x × x ...
```

Use:

```text
x^n = (x^(n/2)) × (x^(n/2))
```

### Pattern

```text
Solve Half
Reuse Half
```

### Complexity

```text
Normal Power  → O(n)
Fast Power    → O(log n)
```

---

## 2. Divide & Conquer Recursion

Break a large problem into a smaller version of itself.

Example:

```text
2^16
↓
2^8
↓
2^4
↓
2^2
↓
2^1
```

Problem size reduces by half every call.

---

## 3. Even vs Odd Exponent Logic

### Even

```text
x^8
=
x^4 × x^4
```

```java
return half * half;
```

### Odd

```text
x^5
=
x × x^2 × x^2
```

```java
return x * half * half;
```

---

## 4. Negative Exponent Formula

```text
x^-n = 1/(x^n)
```

Examples:

```text
2^-2 = 1/4
2^-3 = 1/8
```

---

## 5. Integer Overflow Edge Case

### Dangerous Value

```java
Integer.MIN_VALUE
```

```text
-2147483648
```

### Problem

```java
-n
```

causes overflow.

### Solution

```java
long N = n;
```

Convert first, then negate.

---

## 6. Base Case Importance

Without a base case:

```java
if(n == 0)
    return 1;
```

recursion never stops.

---

## 7. Recursive Reduction Pattern

Used in Power of Four:

```text
16
↓
4
↓
1
```

General form:

```text
Base Case
↓
Invalid Case
↓
Reduce Problem
↓
Recursive Call
```

---

## 8. Power of Four Observation

All powers of four:

```text
1
4
16
64
256
1024
...
```

can repeatedly divide by:

```text
4
```

and eventually reach:

```text
1
```

---

## 9. Mathematical Thinking Before Coding

Before writing code, identify:

```text
What is the smallest valid case?
How can the problem be reduced?
What condition makes the answer impossible?
```

This made both today's problems much easier.

---

## Most Important Concept Of The Day

```text
Recursion is not repeating work.

Good recursion reduces the problem size and reuses previous results.
```

This idea is the foundation of:

* Fast Power
* Divide & Conquer
* Merge Sort
* Binary Search
* Many Dynamic Programming optimizations

# 📌 Day 20 – Important Concepts (08-05-2026)

## 🔹 Character Frequency Array

When a problem involves only lowercase English letters (`a-z`), use:

```java
int[] count = new int[26];
```

instead of a `HashMap`.

Mapping:

```java
'a' - 'a' = 0
'b' - 'a' = 1
...
'z' - 'a' = 25
```

Pattern:

```java
// Count frequency
count[ch - 'a']++;

// Use character
count[ch - 'a']--;

// Invalid
if(count[ch - 'a'] < 0)
    return false;
```

---

## 🔹 Character to Index Mapping

Convert a lowercase character into an array index:

```java
int index = ch - 'a';
```

Examples:

```text
'a' → 0
'b' → 1
'c' → 2
...
'z' → 25
```

---

## 🔹 Word Detection Pattern

Don't count spaces.

Count **the beginning of every word**.

A new word starts when:

```java
current != ' '
&&
(i == 0 || previous == ' ')
```

Pattern:

```java
if(s.charAt(i) != ' ' &&
   (i == 0 || s.charAt(i-1) == ' '))
{
    count++;
}
```

---

## 🔹 Operator Precedence

Remember:

```java
A && B || C
```

is evaluated as:

```java
(A && B) || C
```

If your logic is:

```java
A && (B || C)
```

always use parentheses.

---

## 🔹 ASCII Character Checking

Uppercase:

```java
ch >= 'A' && ch <= 'Z'
```

Lowercase:

```java
ch >= 'a' && ch <= 'z'
```

Equivalent Java methods:

```java
Character.isUpperCase(ch);
Character.isLowerCase(ch);
```

---

## 🔹 Pattern Before Code

Before writing code, identify the pattern.

Ask:

* What are the valid cases?
* What are the invalid cases?
* Can I divide the problem into separate scenarios?

Good logic makes coding much easier.

---

## 🔹 Verify, Don't Assume

Instead of returning inside the first iteration of a loop:

* Verify every required character.
* Return `false` immediately when an invalid case is found.
* Return `true` only after the entire loop finishes successfully.

Pattern:

```java
for(...)
{
    if(invalid)
        return false;
}

return true;
```

---

# ⭐ Patterns Learned Today

* Character Frequency Array
* Character → Array Index Mapping
* Count Start of Words Pattern
* Case-Based Problem Solving
* ASCII Character Comparison
* Operator Precedence (`&&` vs `||`)
* Validate Entire Input Before Returning

---

**Day 20 Concepts Added ✅**

# 🧠 Day 21 – Important Concepts (06-08-2026)

## 🔹 Two Pointer Technique

* Two pointers **do not mean two nested loops**.
* Each pointer has a different responsibility.
* Commonly used for arrays and strings.
* Helps reduce time complexity from **O(n²)** to **O(n)**.

---

## 🔹 Two Pointer Roles

* **Scanning Pointer:** Traverses every element.
* **Placement Pointer:** Tracks where the next valid element should be placed.

---

## 🔹 Swapping Elements

```java
int temp = nums[i];
nums[i] = nums[j];
nums[j] = temp;
```

Used when elements need to exchange positions in-place.

---

## 🔹 Digit Extraction Pattern

Extract digits of a number:

```java
while (copy != 0) {
    int digit = copy % 10;
    copy /= 10;
}
```

### Key Operations

```java
digit = number % 10;   // Last digit
number /= 10;          // Remove last digit
```

---

## 🔹 Copy Variable

Always preserve the original number:

```java
int copy = n;
```

Modify `copy` instead of the original variable.

---

## 🔹 Product of Digits Pattern

```java
int product = 1;

while(copy != 0){
    int digit = copy % 10;
    product *= digit;
    copy /= 10;
}
```

---

## 🔹 Brute Force Search Pattern

```text
Start from n
↓
Check condition
↓
If false → n++
↓
Repeat
```

Useful when constraints are small.

---

## 🔹 Infinite Loop with Exit Condition

```java
while(true){
    if(condition){
        return answer;
    }
}
```

Safe to use when the loop has a guaranteed exit using `return` or `break`.

---

## 🔹 Unreachable Statement (Java)

Java reports an **Unreachable Statement** when it can prove a line of code will never execute.

Example:

```java
while(true){
    return value;
}

return 1; // Unreachable
```

---

## 🔹 Time Complexity

### Move Zeroes

* **Time:** `O(n)`
* **Space:** `O(1)`

### Smallest Divisible Digit Product I

* **Time:** `O(k × d)`

  * `k` = numbers checked
  * `d` = number of digits
* **Space:** `O(1)`

---

## ⭐ Patterns Learned Today

* Two Pointer Technique
* In-place Swapping
* Digit Extraction
* Product of Digits
* Brute Force Search
* Infinite Loop with Exit Condition
* Java Program Flow (Unreachable Statement)

# 🧠 Day 22 – Important Concepts (07-08-2026)

## 📌 Problems Covered

* 389. Find the Difference
* 476. Number Complement (Concept Learning)

---

# 🔹 Frequency Array Pattern

A frequency array stores how many times each character appears.

```java
int[] count = new int[26];
```

### Character → Index

```java
ch - 'a'
```

Example:

```text
'a' → 0
'b' → 1
'c' → 2
...
'z' → 25
```

### Index → Character

```java
(char)(index + 'a')
```

---

# 🔹 Frequency Array Workflow

1. Increment frequency for the first string.
2. Decrement frequency for the second string.
3. If any frequency becomes negative, that character is the answer.

Pattern:

```java
count[ch - 'a']++;

count[ch - 'a']--;

if(count[ch - 'a'] < 0)
    return ch;
```

---

# 🔹 Early Return

Instead of processing the entire array after finding the answer:

```java
if(condition)
    return answer;
```

Returning immediately keeps the solution simple and efficient.

---

# 🔹 Binary Numbers

Computers store numbers in binary.

Examples:

| Decimal | Binary |
| ------: | :----: |
|       1 |    1   |
|       2 |   10   |
|       3 |   11   |
|       4 |   100  |
|       5 |   101  |
|       6 |   110  |
|       7 |   111  |
|       8 |  1000  |

---

# 🔹 Bitwise Operators

## AND (`&`)

Both bits must be **1**.

```text
1 & 1 = 1
1 & 0 = 0
0 & 1 = 0
0 & 0 = 0
```

---

## OR (`|`)

At least one bit must be **1**.

```text
1 | 1 = 1
1 | 0 = 1
0 | 1 = 1
0 | 0 = 0
```

---

## XOR (`^`)

Different bits → **1**

Same bits → **0**

```text
1 ^ 1 = 0
0 ^ 0 = 0
1 ^ 0 = 1
0 ^ 1 = 1
```

### Important Properties

```text
a ^ a = 0
a ^ 0 = a
```

---

## NOT (`~`)

Flips every bit.

```text
1 → 0
0 → 1
```

---

# 🔹 Java Uses 32-bit Integers

Example:

```text
5

00000000000000000000000000000101
```

Using `~`:

```text
11111111111111111111111111111010
```

`~` flips **all 32 bits**, not just the meaningful bits.

---

# 🔹 Mask

A mask is used to affect only the required bits.

Example:

```text
Number

101

Mask

111
```

Using XOR:

```text
101
111
---
010
```

Only the meaningful bits are flipped.

---

# 🔹 Finding Significant Bits

Java utility:

```java
Integer.numberOfLeadingZeros(num)
```

Used to calculate the number of meaningful bits in an integer.

---

# 🔹 Pattern Recognition

Today's biggest realization:

Different problems can use the **same underlying algorithm**.

Example:

* 383. Ransom Note
* 389. Find the Difference

Both use the **Frequency Array Pattern**, even though the problem statements are different.

---

# ⭐ Key Takeaways

* Frequency Array Pattern
* Character ↔ Index Mapping
* Early Return
* Binary Representation
* Bitwise Operators (`&`, `|`, `^`, `~`)
* XOR Properties
* Java 32-bit Integer Representation
* Mask Concept
* Pattern Recognition over Memorization


# 🧠 Day 23 — Important Concepts

**Date:** 08-08-2026

## 1. Minimum So Far + Best Result So Far

Used in **121. Best Time to Buy and Sell Stock**.

Instead of finding the overall minimum and maximum, track the minimum value **while traversing**.

```java
int minPrice = prices[0];
int maxProfit = 0;
```

For every element:

```text
minimum so far → possible current result → best result
```

### Key Idea

> When the order matters, don't calculate minimum and maximum independently.

---

## 2. Order Matters

In stock problems:

```text
BUY → SELL
```

The buying day must come before the selling day.

Example:

```text
[7, 6, 4, 3, 1]
```

Overall:

```text
max = 7
min = 1
```

But `1` occurs after `7`, so `7 - 1` is not a valid profit.

### Lesson

Always consider **position/order**, not just values.

---

## 3. Two Pointer Pattern

Used in **392. Is Subsequence**.

Two variables can track two different things:

```text
i → scans through t
j → tracks the next required character of s
```

When characters match:

```java
if (s.charAt(j) == t.charAt(i)) {
    j++;
}
```

`i` continues scanning `t`.

---

## 4. Meaning of a Pointer

A pointer becomes easier to use when its meaning is clearly defined.

For today's problem:

```text
i = current index in t
j = number of characters from s already matched
```

Therefore:

```java
j == s.length()
```

means:

> Every character of `s` has been successfully matched.

---

## 5. Boundary Checking

Before:

```java
s.charAt(j)
```

make sure:

```java
j < s.length()
```

Otherwise, if `j == s.length()`, accessing `s.charAt(j)` causes an index error.

---

## 6. One-Pass Thinking

Both problems can be solved with a single traversal.

### Stock

```text
Scan → update minimum → calculate profit → update maximum
```

### Subsequence

```text
Scan t → compare → move pointer when matched
```

This gives:

```text
Time Complexity → O(n)
Space Complexity → O(1)
```

---

# ⭐ Patterns Added Today

```text
1. Minimum So Far
2. Best Result So Far
3. Two Pointers
4. Ordered Traversal
5. Pointer Meaning
6. Boundary Checking
7. One-Pass Array/String Processing
```

## 🔥 Most Important Lesson

> **Don't just ask "What value do I need?" Ask "What information do I need to remember while traversing?"**

# 🧠 Day 24 — Important Concepts

**Date:** 09-08-2026

## 1. Minimum Tracking

Instead of sorting everything, keep track of the smallest value while traversing.

```java
int min = Integer.MAX_VALUE;
```

Update when:

```java
if (value < min)
```

---

## 2. Minimum + Multiple Answers

When multiple elements can have the same minimum:

```text
value < min → clear old answers + add new answer
value == min → add another answer
value > min → ignore
```

This is an important pattern for problems where the answer is **not necessarily unique**.

---

## 3. Stack — Push / Pop / Peek

A stack follows:

**LIFO — Last In, First Out**

Important operations:

```text
push()     → add
pop()      → remove top
peek()     → view top
isEmpty()  → check empty
```

---

## 4. Stack for Adjacent Cancellation

For **1047. Remove All Adjacent Duplicates**:

```text
current == stack.peek()
        ↓
      pop()

current != stack.peek()
        ↓
      push()
```

This is the main DSA pattern from today.

---

## 5. "Most Recently Kept" Pattern

A stack is useful when the current element needs to interact with the **last element that survived**.

Example:

```text
"a b b a"
    ↓
remove bb
    ↓
"a a"
    ↓
remove aa
```

The stack automatically exposes the previous surviving character.

---

## 6. StringBuilder

Use `StringBuilder` when constructing a String character-by-character.

```java
StringBuilder ans = new StringBuilder();

ans.append(ch);
```

Finally:

```java
return ans.toString();
```

---

## 7. Java Generics

Instead of:

```java
Stack stack = new Stack();
```

prefer:

```java
Stack<Character> stack = new Stack<>();
```

This tells Java exactly what type the collection stores.

---

## 8. String Comparison

For Java Strings:

```java
str1.equals(str2)
```

not:

```java
str1 == str2
```

---

# ⭐ Most Important Concepts Today

```text
1. Minimum Tracking
2. Handling Equal Minimums
3. Stack / LIFO
4. Push, Pop, Peek
5. Adjacent Cancellation
6. Most Recently Kept Element
7. StringBuilder
8. Java Generics
9. String.equals()
```

### 🔥 Biggest Concept

> **If a problem repeatedly compares the current element with the most recently surviving element, think STACK.**

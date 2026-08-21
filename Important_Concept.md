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


# 🧠 Day 25 — Important Concepts

**Date:** 10-08-2026
**Problem:** 49. Group Anagrams

## ⭐ Most Important Concepts

### 1. HashMap Grouping

Use a `HashMap` when you want to group multiple elements based on a common property.

```text
Common Key → Group of Values
```

---

### 2. Common Key / Representative Key

The biggest concept today.

Different strings can be converted into the same representation.

```text
eat → aet
tea → aet
ate → aet
```

So `"aet"` becomes the **common key**.

---

### 3. HashMap + List

A single key can have multiple values:

```java
HashMap<String, List<String>>
```

Example:

```text
"aet" → ["eat", "tea", "ate"]
```

This is an important data-structure combination.

---

### 4. Sorting to Create a Key

For anagrams:

```text
String
  ↓
char[]
  ↓
sort
  ↓
String key
```

Important Java methods:

```java
str.toCharArray();
Arrays.sort(chars);
new String(chars);
```

---

### 5. `putIfAbsent()`

Useful when creating groups:

```java
map.putIfAbsent(key, new ArrayList<>());
```

Meaning:

> Create the list only if this key doesn't already exist.

---

### 6. `map.get(key).add(value)`

Once the group exists:

```java
map.get(key).add(str);
```

This adds the original string to its corresponding group.

---

### 7. `map.values()`

When the keys were only used for grouping, we can retrieve all groups using:

```java
map.values()
```

---

### 8. Reusing Previous Patterns

Today's problem is an extension of **Valid Anagram**.

```text
Valid Anagram
→ identify same character pattern

Group Anagrams
→ use that pattern as a key
→ group all matching strings
```

This is an important skill: **recognizing when an old pattern can solve a new problem.**

---

# 🔥 Pattern to Remember

```text
Element
   ↓
Create common representation
   ↓
Use representation as HashMap key
   ↓
Group elements with same key
```

### For Anagrams:

```text
Sort characters → Common Key → HashMap Group
```

## 🎯 Most Important Concept Today

> **When different elements share a common property, try converting that property into a key and use a HashMap to group them.**

**Day 25 — Important Concepts Complete ✅**


# 🧠 Day 26 — Important Concepts

**Date:** 11-08-2026

### 1. Sequential Prefix

A prefix is sequential when:

```java
nums[i] == nums[i - 1] + 1
```

When this becomes false, the sequential prefix ends.

---

### 2. HashSet — Membership Checking

Use:

```java
set.contains(value)
```

when the main question is:

> "Does this value exist?"

---

### 3. Search to the Right

For problems where `j > i`:

```java
for (int j = i + 1; j < n; j++)
```

This automatically guarantees:

```text
i < j
```

---

### 4. First Valid Element → `break`

When a problem asks for the **first** valid element:

```text
Search → Find → Use → break
```

This was important in **1475. Final Prices**.

---

### 5. Default Answer + Update

Initialize with the value that should be returned if no special condition occurs:

```java
ans[i] = prices[i];
```

Then update only when a valid discount is found.

---

### 6. Good Pair Pattern

A good pair requires:

```text
nums[i] == nums[j]
i < j
```

Using:

```java
j = i + 1
```

automatically satisfies `i < j`.

---

### 7. Frequency → New Pairs

If a number has appeared `k` times before, the next occurrence creates exactly `k` new pairs.

```text
frequency = 0 → +0 pairs
frequency = 1 → +1 pair
frequency = 2 → +2 pairs
frequency = 3 → +3 pairs
```

This is the key **HashMap frequency-counting pattern**.

---

### ⭐ Most Important Concept

> **Previous frequency tells you how many new pairs the current element creates.**

Remember this pattern:

```text
See number
   ↓
Check previous frequency
   ↓
Add frequency to answer
   ↓
Increase frequency
```

**Day 26 Important Concepts — Done ✅**

# 🧠 Day 27 — Important Concepts

**Date:** 12-08-2026

## 1. 2D Array Traversal

```java
array[i][j]
```

```text
i → row
j → column
```

---

## 2. Row vs Element

```java
array[i]       // entire row
array[i][j]    // individual element
```

This is a **recurring mistake** I need to remember.

---

## 3. `length` in 2D Arrays

```java
array.length
```

→ number of rows

```java
array[i].length
```

→ number of elements in row `i`

Correct traversal:

```java
for (int i = 0; i < array.length; i++) {
    for (int j = 0; j < array[i].length; j++) {
        // array[i][j]
    }
}
```

---

## 4. Row Sum

```java
sum += array[i][j];
```

Use this when each row represents one object or customer and we need its total.

---

## 5. Maximum Value Pattern

```java
if (value > max) {
    max = value;
}
```

Pattern:

```text
Calculate current value
        ↓
Compare with max
        ↓
Update max
```

---

## 6. Main Diagonal

For a square matrix:

```java
mat[i][i]
```

Example:

```text
[1 2 3]
[4 5 6]
[7 8 9]

1 → 5 → 9
```

---

## 7. Secondary Diagonal

```java
mat[i][n - 1 - i]
```

Example:

```text
[1 2 3]
[4 5 6]
[7 8 9]

3 → 5 → 7
```

---

## 8. Center Element Double Counting

For an odd-sized matrix, the center belongs to both diagonals.

```java
if (n % 2 == 1) {
    sum -= mat[n / 2][n / 2];
}
```

---

## 9. HashMap Frequency

```text
element → frequency
```

Use a `HashMap` when we need to track how many times an element appears.

---

## 10. Sliding Window — Introduction

Basic idea:

```text
right → expand window
left  → shrink window
```

Useful for contiguous subarray or substring problems.

For `2958`:

```text
frequency of every element <= k
```

---

## 11. TLE Recognition

The brute-force approach for `2958` used nested loops:

```text
O(n²)
```

and resulted in **TLE**.

Important lesson:

> A solution can be logically correct but still too slow.

When the same elements are repeatedly checked, look for an optimization such as **Sliding Window**.

---

# ⭐ Most Important Concept

> **In a 2D array, always identify exactly what each index represents before writing the loop.**

```text
array[i]       → row
array[i][j]    → element
i              → row index
j              → column index
```

**Day 27 — Important Concepts Complete ✅**


3. Single Number Pattern

When every number appears twice except one:

duplicate ^ duplicate = 0

so the duplicates disappear and the unique value remains.

General pattern:
int ans = 0;

for (int num : nums) {
    ans ^= num;
}

# 🧠 Day 29 — Important Concepts

**Date:** 14-08-2026

## 1. Sliding Window

Used in `3090. Maximum Length Substring With Two Occurrences`.

Basic idea:

```text
right → expand the window
left  → shrink the window when invalid
```

The goal is to maintain a valid continuous substring while finding the maximum length.

---

## 2. Frequency Tracking

Keep track of how many times each character appears inside the current window.

```text
character → frequency
```

For this problem:

```text
frequency <= 2
```

If a character becomes `3`, the window is invalid.

---

## 3. Shrinking the Window

When the current window becomes invalid:

```text
frequency > 2
        ↓
remove the character at left
        ↓
decrease its frequency
        ↓
left++
```

Important:

> Moving `left` means an element is leaving the window, so its frequency must also be decreased.

---

## 4. Window Length

For a window from `left` to `right`:

```text
length = right - left + 1
```

This gives the number of characters currently inside the window.

---

## 5. Prefix

A **prefix** must start from the beginning of a string.

Example:

```text
"attention"

"at"   → prefix ✅
"att"  → prefix ✅
"tion" → prefix ❌
```

Java method:

```java
word.startsWith(pref)
```

---

## 6. Substring

A **substring** can appear anywhere inside a string, but it must be continuous.

Example:

```text
"abcdef"

"abc" → substring ✅
"cde" → substring ✅
"def" → substring ✅
"ace" → substring ❌
```

Java method:

```java
word.contains(pattern)
```

---

## 7. `startsWith()` vs `contains()`

```text
startsWith() → checks only the beginning
contains()   → checks anywhere
```

This was an important distinction between problems `2185` and `1967`.

---

## 8. Array vs Element

A recurring mistake:

```java
words       // entire String array
words[i]    // one String
```

So String methods such as:

```java
startsWith()
contains()
```

must be called on:

```java
words[i]
```

when working with an array of strings.

---

## 9. `charAt()`

Java String character access:

```java
s.charAt(i)
```

Not:

```java
s.countAt(i)
```

---

## 10. Frequency Array for Lowercase Letters

For lowercase English letters:

```java
int[] freq = new int[26];
```

Character index:

```java
s.charAt(i) - 'a'
```

Example:

```text
'a' - 'a' = 0
'b' - 'a' = 1
'c' - 'a' = 2
```

---

# ⭐ Most Important Concepts Today

```text
1. Sliding Window
2. Expand with right
3. Shrink with left
4. Frequency tracking
5. Window length = right - left + 1
6. Prefix → startsWith()
7. Substring → contains()
8. Array vs individual element
9. charAt()
10. Frequency array
```

## 🎯 Day 29 Takeaway

> **Prefix means beginning. Substring means anywhere but continuous.**

And for frequency-limited substring problems:

```text
expand → check frequency → shrink → update maximum
```

**Day 29 — Important Concepts Complete ✅**

# 🧠 Day 30 — Important Concepts

**Date:** 15-08-2026

## 1. Total Sum + Left Sum

For pivot/middle-index problems:

```text
total = leftSum + current + rightSum
```

Therefore:

```text
rightSum = total - leftSum - current
```

This avoids repeatedly calculating the right side.

---

## 2. Running Sum

Instead of storing every left sum, keep one variable:

```java
leftSum += nums[i];
```

The left sum is updated **after checking the current index** because the current element does not belong to either side.

---

## 3. Pattern Reuse

Similar problems can use the same approach.

```text
724 → Find Pivot Index
1991 → Find Middle Index
```

Both use:

```text
total sum
    ↓
left sum
    ↓
calculate right sum
    ↓
compare
```

Important habit:

> Before creating a new solution, check whether the problem resembles something already solved.

---

## 4. Index vs Value

Keep these separate:

```text
maxIndex       → position
nums[maxIndex] → actual value
```

Never confuse an index with the value stored at that index.

---

## 5. Finding Maximum With Its Index

Use the index of the current maximum:

```java
if (nums[i] > nums[maxIndex]) {
    maxIndex = i;
}
```

This lets you keep both the largest value and its position.

---

## 6. Validate the Maximum Against Other Values

For problems like `747`, first find the maximum, then check:

```text
maximum >= 2 × every other value
```

A simple second loop is completely fine when the total complexity is still `O(n)`.

---

## 7. Triplet Brute Force

For problems requiring three indexes:

```text
choose i
choose j
choose k
check conditions
count if valid
```

When the problem requires:

```text
i < j < k
```

use:

```java
j = i + 1
k = j + 1
```

This automatically maintains the correct order.

---

## 8. `Math.abs()`

Absolute difference in Java:

```java
Math.abs(x - y)
```

Useful when a condition depends on the distance between two values.

---

## 9. Brute Force Depends on Constraints

Brute force is not automatically bad.

If the input size is small, even:

```text
O(n³)
```

can be acceptable.

Important habit:

> Check the constraints before deciding that brute force is too slow.

---

## 10. Don't Force Fewer Loops

Using fewer loops does not automatically mean a better solution.

For example:

```text
2 loops → O(n)
1 loop  → O(n)
```

Both are linear.

A clear and understandable solution is often better than a complicated one-loop solution.

---

# ⭐ Most Important Concepts Today

```text
1. Total Sum + Running Left Sum
2. Right Sum = Total - Left - Current
3. Pattern Reuse
4. Index vs Value
5. Finding Maximum + Index
6. Validating Maximum Against Others
7. Triplet Brute Force
8. i < j < k
9. Math.abs()
10. Choosing Brute Force Using Constraints
11. Don't Force Fewer Loops
```

## 🎯 Day 30 Takeaway

> **Understand the pattern and complexity instead of focusing on how many loops the code has.**

```text
Recognize → Reuse → Simplify → Optimize only when necessary
```

**Day 30 — Important Concepts Complete ✅**

# 🧠 Day 31 — Important Concepts

**Date:** 16-08-2026

## 1. Odd-Length Subarray

A subarray is **odd-length** when:

```java
length % 2 == 1
```

For a subarray from `i` to `j`:

```java
length = j - i + 1;
```

---

## 2. Running Subarray Sum

Instead of using a third loop to calculate every subarray's sum:

```java
subsum += arr[j];
```

As `j` moves forward, `subsum` keeps the current subarray's sum.

---

## 3. 2D Array Traversal

```text
grid.length       → number of rows
grid[i].length    → number of columns
grid[i][j]        → individual element
```

Remember:

```text
i → row
j → column
```

This is still a **recurring mistake** and needs attention.

---

## 4. Digit Extraction

To get the last digit:

```java
n % 10
```

To remove the last digit:

```java
n /= 10;
```

General pattern:

```text
get digit → process digit → remove digit → repeat
```

---

## 5. Binary Tree Node Access

For a tree node:

```java
root.val
```

→ current node value

```java
root.left.val
```

→ left child value

```java
root.right.val
```

→ right child value

---

## 6. Simulation Pattern

Some problems simply require following the rules repeatedly:

```text
Read current state
      ↓
Perform operation
      ↓
Update state
      ↓
Repeat
      ↓
Check final state
```

Used in problems like `2169` and `657`.

---

## 7. State Tracking

Instead of storing every step, maintain only the information needed to describe the current state.

For the robot problem:

```text
leftright → horizontal position
updown     → vertical position
```

At the end:

```text
leftright == 0
updown == 0
```

means the robot returned to the origin.

---

## 8. `while` Loop for Unknown Number of Operations

When you don't know beforehand how many operations will happen:

```java
while (condition) {
    // perform operation
}
```

Example:

```java
while (num1 != 0 && num2 != 0)
```

The loop continues until the required stopping condition is reached.

---

## 9. Pattern Recognition

Today's problems reinforced several patterns:

```text
Subarray → running sum
2D array → row + column traversal
Number → digit extraction
Tree → node/child access
Repeated operation → simulation
Movement → state tracking
```

The important skill is recognizing the underlying pattern even when the problem statement looks different.

---

# ⭐ Most Important Concepts Today

```text
1. Odd subarray length = j - i + 1
2. Running subarray sum
3. 2D array indexing
4. Digit extraction using % 10 and / 10
5. Binary tree node access
6. Simulation
7. State tracking
8. while loop for repeated operations
9. Pattern recognition
```

## 🎯 Day 31 Takeaway

> **Different problems can use the same basic idea: maintain the right information, update it as you traverse, and check the final condition.**

**Day 31 — Important Concepts Complete ✅**

# 🧠 Day 32 — Important Concepts

**Date:** 17-08-2026

## 1. Difference Array / Change Tracking

Instead of calculating the population from scratch for every year, track only when the population changes.

```text
Birth year  → +1
Death year  → -1
```

Then scan through the years and keep a running population.

```java
current += change[i];
```

---

## 2. Birth Year Is Included

For a person:

```text
[birth, death]
```

they are counted starting from the birth year.

Condition:

```text
birth <= year
```

---

## 3. Death Year Is Not Included

The person is **not** counted in their death year.

Full condition:

```text
birth <= year < death
```

For:

```text
[1993, 1999]
```

the person is counted in:

```text
1993 → 1998
```

but not `1999`.

---

## 4. Population as a Running Total

After recording the changes:

```text
current population = previous population + change
```

Example:

```text
1950 → +1
1960 → +1
1961 → -1
1971 → -1
```

Scanning these changes gives the population for each year.

---

## 5. Mapping Years to Array Indexes

The years are limited to:

```text
1950 → 2050
```

So there are:

```text
2050 - 1950 + 1 = 101
```

possible years.

Convert a year to an array index using:

```java
year - 1950
```

Examples:

```text
1950 → index 0
1960 → index 10
2050 → index 100
```

---

## 6. Earliest Maximum

The problem asks for the **earliest** year when the population is maximum.

So update the answer only when:

```java
current > maxPopulation
```

not:

```java
current >= maxPopulation
```

Why?

If:

```text
1960 → population 2
1970 → population 2
```

we keep `1960`.

---

## 7. Constraint-Based Thinking

The small year range is important.

Because there are only `101` possible years, we can safely build an array representing those years.

General lesson:

> Always look at the constraints before deciding how to represent the problem.

---

## 8. Overlapping Ranges

The population of a year is determined by how many people's alive ranges include that year.

Think:

```text
Person A: [1950,1961)
Person B: [1960,1971)

1960:
A → alive ✅
B → alive ✅

Population = 2
```

The half-open range notation `[birth, death)` is a useful way to remember that birth is included but death is excluded.

---

# ⭐ Most Important Concepts Today

```text
1. Difference Array / Change Tracking
2. Birth → +1
3. Death → -1
4. Alive condition = birth <= year < death
5. Running population
6. Year → index using year - 1950
7. Earliest maximum → use >
8. Constraints can simplify the solution
9. Population comes from overlapping alive ranges
```

## 🎯 Day 32 Takeaway

> **When something changes at specific points in time, track the changes and build the running state instead of recalculating everything repeatedly.**

**Day 32 — Important Concepts Complete ✅**

# Important Concepts & Patterns — Day 36
**Date:** August 20, 2026  
**Day Number:** Day 36

---

## 1. Key Algorithmic Concepts & Patterns

### 1. Reverse Iteration / Suffix Accumulation Pattern
* **Concept:** When a problem requires computing a property across all elements to the right of each position, traversing backwards (from right to left) allows maintaining a running state in $O(1)$ auxiliary space and $O(n)$ time.
* **Mental Rule:** Whenever you find yourself re-scanning the remainder of a list inside a loop, ask: *"If I walk backward from the end, do I already have the answer ready for the current position?"*

### 2. Independent Dynamic Buffers with Pointers
* **Concept:** When splitting a stream into multiple growing collections using primitive arrays:
  * Allocate buffer space to the theoretical maximum size (`n`).
  * Maintain an isolated pointer/counter for each buffer (`idx1`, `idx2`).
  * **Pointer Invariants:**
    * Write target: `buffer[idx] = val; idx++;`
    * Tail inspection (last appended element): `buffer[idx - 1]`
    * Active length / slice boundary: `0` to `idx - 1`

### 3. Array Copy Semantics (`System.arraycopy` vs. Manual Loops)
* When working with pre-allocated buffers that are only partially filled:
  * Only transfer elements in the range `[0, active_size)`.
  * For destination offsets: the second partition must start at destination index equal to `size1`, not a static constant.

---

## 2. Summary of Questions Solved

* **Total Questions Solved:** 2
  1. LeetCode 1299 — *Replace Elements with Greatest Element on Right Side*
  2. LeetCode 3069 — *Distribute Elements Into Two Arrays I*

---

*See you on Day 37*

# Important Concepts & Patterns — Day 37
**Date:** August 21, 2026  
**Day Number:** Day 37

---

## 1. Key Algorithmic Concepts & Patterns

### 1. Lookahead Invariant in Greedy String Processing
* **Concept:** When processing sequences where an item's semantic value depends on future context, a 1-step lookahead (`peek(i + 1)`) simplifies parsing without requiring a full sliding window or state machine.
* **Pattern Template:**
  ```java
  if (i + 1 < length && value(s[i]) < value(s[i + 1])) {
      total -= value(s[i]);
  } else {
      total += value(s[i]);
  }
  ```

### 2. General Carry-Sum Simulation (Base-K Arithmetic)
* **Concept:** Adding numbers represented as strings without numeric overflow.
* **Invariant:** Traverse both strings right-to-left. Continue as long as either string has remaining digits OR a carry is nonzero.
* **Formulas for Base-$K$:**
  * $	ext{Digit to Append} = (	ext{digit}_A + 	ext{digit}_B + 	ext{carry}) \pmod K$
  * $	ext{Next Carry} = (	ext{digit}_A + 	ext{digit}_B + 	ext{carry}) / K$

### 3. Primitive Lookup vs. Object Map Overhead
* In micro-benchmarks and high-frequency checks:
  * `HashMap<Character, Integer>` introduces boxing (`char` $	o$ `Character`, `int` $	o$ `Integer`), hashing, and heap lookups.
  * A `switch` expression or fixed ASCII array `int[128]` provides true $O(1)$ zero-allocation lookups with direct cache locality.

---

## 2. Summary of Questions Solved

* **Total Questions Solved:** 2
  1. LeetCode 13 — *Roman to Integer*
  2. LeetCode 67 — *Add Binary*

---

*See you on Day 38*

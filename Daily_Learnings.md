# LeetCode Daily Progress 🚀

---

## 📅 2026-07-16

### Problems Solved Today: 5

- LeetCode 2235 — Add Two Integers
- LeetCode 1480 — Running Sum of 1D Array
- LeetCode 1929 — Concatenation of Array
- LeetCode 2011 — Final Value of Variable After Performing Operations
- LeetCode 2114 — Maximum Number of Words Found in Sentences

### What I Learned Today

- Traversing arrays using loops.
- Traversing an array of strings.
- Traversing characters of a string using `charAt()`.
- Creating and returning values from functions.
- Passing parameters to methods.
- Performing basic arithmetic operations.
- Understanding and implementing Running Sum (Prefix Sum).
- Creating and working with new arrays.
- Using array indexing effectively.
- Comparing strings using `.equals()`.
- Using conditional statements (`if-else`).
- Incrementing and decrementing variables.
- Counting occurrences of a character.
- Converting spaces to words (`words = spaces + 1`).
- Finding the maximum value using comparison logic.
- Using nested loops to process strings and arrays.
- Improving problem-solving by breaking problems into smaller steps.

### Important Patterns

#### Running Sum Pattern

```java
// Add previous cumulative sum to current element
arr[i] = arr[i] + arr[i - 1];
```

#### Maximum Value Pattern

```java
// Update maximum value when a larger value is found
if(current > max)
{
    max = current;
}
```

#### String Comparison

```java
// Compare string contents
str.equals("text");
```

#### Character Access

```java
// Access character at index i
str.charAt(i);
```

### Day Summary

- Problems Solved: **5**
- Main Topics: **Arrays, Strings, Loops, Nested Loops, Prefix Sum**
- Difficulty: **Easy**
- Status: **Completed ✅**

---

# 🚀 LeetCode Daily Progress — 18 July 2026

## Problems Solved Today: 6

1. LeetCode 2114 — Maximum Number of Words Found in Sentences
2. LeetCode 2942 — Find Words Containing Character
3. LeetCode 412 — Fizz Buzz
4. LeetCode 2469 — Convert the Temperature
5. LeetCode 2652 — Sum Multiples
6. LeetCode 1528 — Shuffle String


# 📚 What I Learned Today (Overall)


## 🔹 Array Traversal

- Traversing arrays using loops.
- Accessing elements using index.
- Understanding array length.

Pattern:

```java
for(int i = 0; i < arr.length; i++)
{

}
```


---

# 🔹 String Traversal

Learned how to traverse characters inside a string.

Example:

```java
String s = "hello";

s.charAt(0); // h
```

Important:

```java
String length  → str.length()

Array length   → arr.length
```


Used in:
- LeetCode 2114
- LeetCode 2942


---

# 🔹 Nested Loop Pattern

Used when working with:

```
Array of Strings
        |
        ↓
Individual String
        |
        ↓
Each Character
```


Pattern:

```java
for(int i = 0; i < words.length; i++)
{
    for(int j = 0; j < words[i].length(); j++)
    {

    }
}
```


Used in:

- Finding characters inside words.
- Counting spaces.
- String searching.


---

# 🔹 String Comparison

Learned that Java strings should be compared using:

```java
.equals()
```

Wrong:

```java
str == "text"
```

Correct:

```java
str.equals("text")
```


---

# 🔹 Counting Pattern

## Counting spaces

LeetCode 2114:

Logic:

```
Words = Spaces + 1
```


Pattern:

```java
if(sentence.charAt(i) == ' ')
{
    count++;
}
```


---

# 🔹 Maximum Value Pattern

Used in LeetCode 2114.

Pattern:

```java
if(current > max)
{
    max = current;
}
```


Used to find:
- Maximum words
- Maximum values
- Best answer


---

# 🔹 List Usage

Learned how to create and use lists.

## String List

```java
List<String> ans = new ArrayList<>();
```

Adding:

```java
ans.add("Fizz");
```


## Integer List

```java
List<Integer> ans = new ArrayList<>();
```

Adding:

```java
ans.add(i);
```


Used in:

- LeetCode 2942
- LeetCode 412


---

# 🔹 String Conversion

## Integer → String

Learned:

```java
String.valueOf(number)
```


Example:

```java
String.valueOf(5);
```

Output:

```
"5"
```


Used in:

- LeetCode 412 Fizz Buzz


---

# 🔹 Character Array

Learned:

```java
char[] ans = new char[size];
```


Why?

Because Strings are immutable.

When changing/rearranging characters:

```
String
 ↓
char[]
 ↓
String
```


Conversion:

```java
new String(charArray)
```


Used in:

- LeetCode 1528 Shuffle String


---

# 🔹 Returning Different Data Types


## Integer

```java
return value;
```


## Array

```java
return ans;
```


## List

```java
return list;
```


## Double Array

```java
double[] ans = new double[2];

return ans;
```


---

# 🔹 Modulus Operator (%)


Used for divisibility checking.


Pattern:

```java
number % divisor == 0
```


Meaning:

```
Number is completely divisible by divisor
```


Examples:

```java
i % 3 == 0

i % 5 == 0

i % 7 == 0
```


Used in:

- LeetCode 412
- LeetCode 2652


---

# 🔹 FizzBuzz Pattern (LeetCode 412)


Condition order is important:


```
Check 3 and 5 first

Then check 3

Then check 5

Else number
```


Because:

```
15 is divisible by 3 and 5
```

Output:

```
FizzBuzz
```


---

# 🔹 Temperature Conversion (LeetCode 2469)


Learned:

- Using double data type.
- Returning double arrays.
- Storing multiple answers.


Pattern:

```java
double[] ans = new double[2];

ans[0] = value1;
ans[1] = value2;

return ans;
```


---

# 🔹 Index Mapping Pattern (LeetCode 1528)


Most important learning today.


Problem:

```
Move characters according to given indexes
```


Example:

```
s = "abc"

indices = [2,1,0]
```


Mapping:

```
a → index 2
b → index 1
c → index 0
```


Pattern:

```java
ans[indices[i]] = s.charAt(i);
```


Meaning:

```
Current character
        |
        ↓
New position
```


---

# ❌ Mistakes I Made Today


## Java Syntax Mistakes

### String comparison

Wrong:

```java
str == "abc"
```

Correct:

```java
str.equals("abc")
```


---

### Array vs String length

Array:

```java
arr.length
```

String:

```java
str.length()
```


---

### char vs char[]

char:

```
single character
```

Example:

```java
char ch = 'a';
```


char array:

```
multiple characters
```

Example:

```java
char[] ch;
```


---

### Wrong array creation

Wrong:

```java
char arr[size];
```

Correct:

```java
char[] arr = new char[size];
```


---

### Returning wrong type

Example:

Method:

```java
public String function()
```

Cannot return:

```java
char[]
```

Need:

```java
new String(charArray)
```


---

# 🧠 Biggest Learning Today


The logic of the problem is usually simple.

The main challenge is:

- Choosing correct data structure.
- Remembering Java syntax.
- Understanding return type.
- Converting logic into code.
- Thinking with indexes and positions.


---

# ⭐ Important Patterns To Revise


## Character Access

```java
str.charAt(i)
```


## String Comparison

```java
str.equals("text")
```


## Convert Integer to String

```java
String.valueOf(i)
```


## Character Array to String

```java
new String(charArray)
```


## Index Mapping

```java
result[newIndex] = value;
```


## Maximum Pattern

```java
if(current > max)
{
    max = current;
}
```


---

# 📊 Daily Summary

Problems Solved: **6**

Topics:

- Arrays
- Strings
- Character Arrays
- ArrayList
- Nested Loops
- String Methods
- Modulus Operator
- Conditions
- Type Conversion
- Index Mapping
- Returning Arrays


## Progress 🚀

Today I improved my ability to convert problem logic into Java code and learned how small syntax details affect the final solution.

# 📅 Day 3 — Understanding Mapping, Counting, and Digit Processing

## Problems Solved Today

- LeetCode 1920 — Build Array from Permutation
- LeetCode 1365 — How Many Numbers Are Smaller Than the Current Number
- LeetCode 1295 — Find Numbers with Even Number of Digits

---

# 🧠 Overall Learning From Today

Today was different from previous days.

Earlier, most of my mistakes were syntax-related:

- length vs length()
- char vs char[]
- Returning wrong data types
- Creating arrays incorrectly

Today, I started facing more logic-oriented problems.

The biggest lesson was:

> Understanding what exactly needs to be counted, mapped, or processed before writing code.

---

# 🚀 LeetCode 1920 — Build Array from Permutation

## My First Thought

I understood that a new array needed to be created.

But I struggled with array creation syntax.

## Mistakes I Made

### Incorrect Array Creation

Wrong:

```java
int ans[] = new ans;
```

Learned:

```java
int[] ans = new int[nums.length];
```

### Loop Boundary Confusion

Initially:

```java
for(int i = 1; i <= nums.length; i++)
```

Learned:

Arrays are 0-indexed.

Correct:

```java
for(int i = 0; i < nums.length; i++)
```

### Assignment Without Index

Wrong:

```java
ans[] = nums[i];
```

Learned:

```java
ans[i] = value;
```

Every array assignment needs an index.

## Biggest Concept Learned

### Index Mapping

```java
ans[i] = nums[nums[i]];
```

This was my second major mapping problem after Shuffle String.

I learned:

> One index can lead to another index.

Example:

```text
nums[1] = 2

ans[1] = nums[2]
```

## Pattern Learned

```java
ans[i] = nums[nums[i]];
```

## Thinking Improvement

Before:

> Copy values directly.

After:

> Use indexes to locate another position.

---

# 🚀 LeetCode 1365 — How Many Numbers Are Smaller Than the Current Number

## My First Thought

For every number:

Compare it with every other number.

If another number is smaller:

Increase the count.

## Mistakes I Made

### Loop Boundary Mistake

Initially:

```java
i <= nums.length
```

Learned:

```java
i < nums.length
```

### Incrementing Whole Array

Wrong:

```java
count++;
```

Learned:

```java
count[i]++;
```

because count is an array.

## Biggest Concept Learned

### Counting Pattern

I learned that:

```java
count[i]
```

stores the answer for:

```java
nums[i]
```

Every position in the answer array can represent the answer for the corresponding input position.

## Pattern Learned

```java
for(int i = 0; i < nums.length; i++)
{
    for(int j = 0; j < nums.length; j++)
    {
        if(nums[i] > nums[j])
        {
            count[i]++;
        }
    }
}
```

## Runtime

```text
7 ms
Beats 82.27%
```

This showed me that a simple brute-force solution can still perform quite well.

## Thinking Improvement

Before:

> I knew how to compare numbers.

After:

> I understood where the result should be stored.

---

# 🚀 LeetCode 1295 — Find Numbers With Even Number of Digits

## My First Thought

I knew division by 10 was related to digits.

But I struggled to convert that idea into code.

## Mistakes I Made

### Treated Array As A Number

Wrong:

```java
while(nums != 0)
```

I forgot that nums is an array.

### Tried Dividing Entire Array

Wrong:

```java
nums /= 10;
```

Arrays cannot be divided.

Learned:

```java
int num = nums[i];
```

Process the element, not the entire array.

### Checked Wrong Thing

Wrong:

```java
if(nums[i] % 2 == 0)
```

I was checking whether the number was even.

The problem asks whether the number of digits is even.

### Counter Scope Mistake

Initially:

```java
int digits = 0;
```

was outside the loop.

So digit counts from previous numbers continued accumulating.

Learned:

```java
for(...)
{
    int digits = 0;
}
```

Each number needs its own digit counter.

## Biggest Concept Learned

### Digit Counting Pattern

```java
while(num != 0)
{
    num /= 10;
    digits++;
}
```

Every division removes one digit.

## Pattern Learned

```java
for(each number)
{
    digits = 0;

    while(number != 0)
    {
        number /= 10;
        digits++;
    }
}
```

## Thinking Improvement

Before:

> I was trying to process the entire array.

After:

> First select one element. Then process that element.

---

# 🐛 Mistake Database Added Today

## Arrays vs Elements

Wrong Thinking:

```java
nums
```

Correct Thinking:

```java
nums[i]
```

Always ask:

> Am I working with the entire array or one element?

## Array Counter vs Integer Counter

Wrong:

```java
count++;
```

Correct:

```java
count[i]++;
```

when count is an array.

## Variable Scope

Wrong:

```java
int digits = 0;
```

outside processing loop.

Correct:

Reset counters for every new element when required.

---

# 🔥 New Patterns Learned Today

## Mapping Pattern

```java
ans[i] = nums[nums[i]];
```

## Counting Pattern

```java
count[i]++;
```

## Digit Counting Pattern

```java
while(num != 0)
{
    num /= 10;
    digits++;
}
```

## Nested Comparison Pattern

```java
for(int i = 0; i < n; i++)
{
    for(int j = 0; j < n; j++)
    {
        if(nums[i] > nums[j])
        {
            count[i]++;
        }
    }
}
```

---

# 📈 Progress After Day 3

## Problems Solved So Far

- LeetCode 2235
- LeetCode 1480
- LeetCode 1929
- LeetCode 2011
- LeetCode 2114
- LeetCode 2942
- LeetCode 412
- LeetCode 2469
- LeetCode 2652
- LeetCode 1528
- LeetCode 1920
- LeetCode 1365
- LeetCode 1295

**Total Solved: 13 Problems**

---

# 🌟 Biggest Realization Today

Earlier, I thought my biggest weakness was syntax.

Now I realize that many mistakes come from understanding:

- What exactly should be counted.
- What exactly should be stored.
- Whether I am working on an array or a single element.
- Where variables should be reset.

These are problem-solving skills that improve only through practice.

Every problem is making my thinking more structured.

I am no longer just writing code.

I am learning how to think like a programmer. 🚀



# 📅 Day 4 — From Syntax Thinking to Problem-Solving Thinking

## Problems Solved

- LeetCode 1470 — Shuffle the Array
- LeetCode 1431 — Kids With the Greatest Number of Candies
- LeetCode 1732 — Find the Highest Altitude

---

# 🎯 Day 4 Overview

Day 4 was different from previous days.

In earlier problems, most of my mistakes were related to Java syntax:

- Arrays
- Return types
- Loops
- ArrayList
- String conversions

Today, most mistakes came from:

```text
Thinking about the problem incorrectly
```

Instead of syntax errors, I spent more time understanding:

```text
How should data move?

Do I need a new array?

Do I need one loop or two loops?

Should I store information first?

What pattern is hidden in the problem?
```

This was an important shift from coding to problem-solving.

---

# LeetCode 1470 — Shuffle the Array

## Problem Understanding

Input:

```java
[x1,x2,x3,y1,y2,y3]
```

Output:

```java
[x1,y1,x2,y2,x3,y3]
```

The challenge was to take values from two halves of the array and merge them alternately.

---

# My Initial Thinking

I kept thinking:

```text
Can I directly place both values into the same position?
```

I wrote ideas like:

```java
array[i] = nums[i];
array[i] = nums[i+n];
```

Then realized:

```text
Second assignment overwrites the first one.
```

One position can store only one value.

---

# Mistake 1

```java
array[i] = nums[i];
array[i] = nums[i+n];
```

Learning:

```text
The second value replaces the first value.

Data gets lost.
```

---

# Mistake 2

I tried using:

```java
i++
```

inside the loop.

Example:

```java
array[i] = nums[i];
i++;
array[i] = nums[i+n];
```

Learning:

```text
The loop already updates i.

Manually changing i inside the loop can create confusion.
```

---

# Mistake 3

I thought:

```text
Maybe I don't need another variable.
```

But then I learned:

```text
The output array position
and input array position
are different things.
```

---

# Biggest Learning

I learned the concept of a separate pointer.

Pattern:

```java
array[k] = nums[i];
k++;

array[k] = nums[i+n];
k++;
```

Learning:

```text
A separate index can control
where data is stored.
```

This was one of the biggest lessons of the day.

---

# LeetCode 1431 — Kids With the Greatest Number of Candies

## Problem Understanding

For every kid:

```text
Current Candies

↓

Add Extra Candies

↓

Can this kid become the kid
with the greatest candies?
```

---

# My Initial Thinking

I immediately started adding:

```java
candies[i] + extraCandies
```

without first knowing:

```text
What is the current maximum?
```

---

# Mistake 1

I created:

```java
int[] ans = new int[candies.length];
```

Learning:

```text
Not every problem requires
an answer array.
```

---

# Mistake 2

I compared:

```java
ans[i] >= extraCandies
```

Learning:

```text
The comparison should be
against the maximum candies,
not against extraCandies.
```

---

# Mistake 3

I accidentally compared:

```java
if(i >= total)
```

Learning:

```text
i = index

total = candy value

Position and value
are completely different things.
```

---

# Mistake 4

I tried solving the entire problem in one pass.

Then I realized:

```text
I cannot know if a child can become
the greatest until I know
who currently has the greatest candies.
```

---

# Biggest Learning

This problem taught me:

## Two-Pass Thinking

Pass 1:

```text
Find Maximum
```

Pass 2:

```text
Build Answer
```

Pattern:

```text
Gather Information

↓

Use Information
```

This pattern will appear many times in future LeetCode problems.

---

# LeetCode 1732 — Find the Highest Altitude

## Problem Understanding

The biker starts at:

```java
0
```

Every gain changes the current altitude.

Goal:

```text
Find the highest altitude reached.
```

---

# My Initial Thinking

I decided to build an altitude array.

Example:

```java
[0,-5,-4,1,1,-6]
```

Then find the maximum.

This was a valid approach.

---

# Mistake 1

I wrote:

```java
alt[i] = altitude + gain[i];
alt[i] += gain[i];
```

Learning:

```text
Gain was added twice.
```

---

# Mistake 2

I wrote:

```java
alt += gain[i];
```

Learning:

```text
alt is an array.

Arrays cannot be updated using +=.
```

---

# Mistake 3

I forgot to update:

```java
altitude
```

Learning:

```text
Altitude changes after every move.
```

Pattern:

```java
altitude += gain[i];
```

---

# Mistake 4

I used:

```java
for(int j=0;j<altitude;j++)
```

Learning:

```text
Altitude is a value.

Array traversal requires array length.
```

Correct thinking:

```java
for(int j=0;j<alt.length;j++)
```

---

# Biggest Learning

This problem connected two patterns I already knew.

## Running Sum

```java
current += value;
```

## Maximum Pattern

```java
if(current > max)
{
    max = current;
}
```

This was my first experience combining multiple previously learned patterns into one solution.

---

# 🐛 Day 4 Mistake Database

## Shuffle Array

### Mistakes

- Overwriting values.
- Trying to use same position for two values.
- Confusion about needing a separate pointer.
- Trying to modify loop variable manually.

### Learning

```text
Output position and input position
can be different.
```

---

## Kids With Candies

### Mistakes

- Created unnecessary array.
- Compared with extraCandies.
- Compared index with value.
- Tried solving before finding maximum.

### Learning

```text
Sometimes information must be gathered
before the answer can be built.
```

---

## Highest Altitude

### Mistakes

- Added gain twice.
- Tried += on an array.
- Forgot to update altitude.
- Used altitude as loop boundary.

### Learning

```text
Running Sum + Maximum Tracking
can solve many problems.
```

---

# 🔥 New Patterns Added Today

## Separate Pointer Pattern

```java
array[k] = value;
k++;
```

---

## Maximum Pattern

```java
if(current > max)
{
    max = current;
}
```

---

## Running Sum Pattern

```java
current += value;
```

---

## Two-Pass Processing

```text
Pass 1

↓

Gather Information

↓

Pass 2

↓

Build Answer
```

---

# 📈 Progress Reflection

Today I noticed a major improvement.

Earlier I mostly struggled with:

```text
How do I write Java syntax?
```

Today I struggled with:

```text
How should I think?
```

That is actually progress.

Because syntax can be memorized.

Problem-solving must be developed.

I am slowly moving from:

```text
Learning Java
```

to

```text
Learning how to solve problems.
```

And that is the real purpose of LeetCode.

🚀


## 📅 2026-07-20

# 📚 Learning Notes — LeetCode 977 & LeetCode 485

---

# LeetCode 977 — Squares of a Sorted Array

## Problem Understanding

Given a sorted array, square every element and return the squares in sorted order.

Example:

```java
Input:  [-4,-1,0,3,10]

Square:
[16,1,0,9,100]

Sorted:
[0,1,9,16,100]
```

---

## My Initial Thinking

I manually decoded the problem in my notebook.

My thought process:

```text
Step 1:
Square all numbers

↓

Step 2:
Sort the squared values

↓

Step 3:
Return the sorted array
```

This was a valid brute-force approach.

---

## My First Mistakes

### Mistake 1

Tried using only one loop for sorting.

Example:

```java
if(sqr[j] > sqr[j+1])
{
    ans[j] = sqr[j];
}
```

### Learning

```text
Comparing values is not sorting.

Sorting requires swapping.
```

---

### Mistake 2

Array index out of bounds.

Example:

```java
sqr[k+1]
```

while

```java
k < sqr.length
```

### Learning

```text
Whenever using k+1,
the loop must stop before the last index.
```

---

### Mistake 3

Created an unnecessary array.

Example:

```java
int[] ans = new int[nums.length];
```

but later sorted directly in:

```java
sqr[]
```

### Learning

```text
Do not create extra arrays unless needed.
```

---

### Mistake 4

Forgot swapping logic.

Initially I was only comparing values.

### Learning

Bubble Sort requires:

```text
Compare

↓

Swap

↓

Repeat
```

---

## New Pattern Learned

### Bubble Sort

```java
for(int i = 0; i < n - 1; i++)
{
    for(int j = 0; j < n - i - 1; j++)
    {
        if(arr[j] > arr[j+1])
        {
            int temp = arr[j];
            arr[j] = arr[j+1];
            arr[j+1] = temp;
        }
    }
}
```

---

## Complexity Understanding

My solution:

```text
Square Array  → O(n)

Bubble Sort   → O(n²)

Total         → O(n²)
```

### Learning

```text
O(n) + O(n²)

↓

O(n²)
```

The largest term dominates.

---

## Biggest Learning

I solved the problem myself without looking at the solution.

Even though the runtime was slower than optimal solutions, I learned:

- Bubble Sort
- Swapping
- Loop boundaries
- Sorting logic
- Time complexity

---

# LeetCode 485 — Max Consecutive Ones

## Problem Understanding

Find the maximum number of consecutive 1s.

Example:

```java
Input:
[1,1,0,1,1,1]

Output:
3
```

---

## My Initial Wrong Thinking

I tried comparing neighboring elements.

Example:

```java
if(nums[i] == nums[current])
```

### Learning

```text
This problem is NOT about comparing elements.

It is about counting streaks.
```

---

## Mistake 1

Confused count variables with indexes.

Example:

```java
nums[current]
nums[max]
```

### Learning

```text
current and max are counters.

They are not array positions.
```

---

## Mistake 2

Used return inside loop.

Example:

```java
return max;
```

### Learning

```text
Returning inside the loop
stops checking the remaining elements.
```

---

## Mistake 3

Thought max should reset.

My thinking:

```java
else
{
    max = 0;
}
```

### Learning

Wrong.

Because:

```text
max = best streak ever found
```

A new zero should only break the current streak.

---

## Huge Learning

When a streak breaks:

```java
current = 0;
```

NOT

```java
max = 0;
```

---

## Most Important Pattern Learned

### Current vs Maximum

```java
current = current streak

max = best streak found so far
```

---

## The Biggest Realization

I discovered why two if statements are needed.

Before:

```text
I thought one if should solve everything.
```

Now:

```text
Question 1:
Is this a 1?

↓

Question 2:
Did current become greater than max?
```

Which leads to:

```java
if(nums[i] == 1)
{
    current++;

    if(current > max)
    {
        max = current;
    }
}
else
{
    current = 0;
}
```

---

## Tiny Mistakes I Want To Remember

### 1. Confusing Value and Index

Wrong thinking:

```java
nums[current]
```

when current was actually a counter.

---

### 2. Returning Too Early

Wrong:

```java
return max;
```

inside the loop.

---

### 3. Resetting Wrong Variable

Wrong:

```java
max = 0;
```

Correct:

```java
current = 0;
```

---

## Personal Improvement

For the past few days I was mentally decoding problems and immediately writing code.

Today I spent more time manually decoding the problem in my notebook before coding.

New process:

```text
Read Problem

↓

Create Example

↓

Write Logic in Words

↓

Identify Variables

↓

Trace Example

↓

Write Code
```

Benefits noticed:

- Fewer mistakes
- Faster debugging
- Better understanding
- More confidence while coding

This habit helped me solve problems with much less confusion.

---

# Key Patterns Added To My Library

## Bubble Sort

```java
if(arr[j] > arr[j+1])
{
    swap
}
```

---

## Current vs Maximum

```java
current++;

if(current > max)
{
    max = current;
}
```

---

## Reset Current Streak

```java
else
{
    current = 0;
}
```

---

# Final Reflection

These two problems taught me that writing code is not the first step.

The real first step is:

```text
Understand

↓

Decode

↓

Trace

↓

Code
```

The more time I spend understanding the problem manually, the fewer mistakes I make while coding.

This is becoming one of the biggest improvements in my LeetCode journey.

# Day 4 Learnings & Mistakes (Last 2 Problems)
📅 21/07/2026

---

# 1. LeetCode 414 — Third Maximum Number

⏱️ Time Spent: ~1 to 1.2 Hours

## What I Learned

- Difference between maximum number and third distinct maximum number.
- Duplicate values should not be counted multiple times.
- Bubble Sort can be used to sort an array before processing.
- Counting distinct values and finding the answer are two different things.
- Edge cases are important.
- Manual tracing in a notebook helps understand logic better.

## Mistakes I Made

### Bubble Sort Mistakes

- Initially forgot proper comparison and swapping logic.
- Needed revision of Bubble Sort implementation.

### Distinct Counting Mistakes

- Counted duplicates incorrectly.
- Confused "count of distinct values" with the actual answer.

### Variable Mistakes

Tried things like:

```java
ans = count[k];
```

Even though:

```java
count
```

was not an array.

### Return Mistakes

- Tried returning count instead of the actual third maximum value.
- Forgot that helper variables help find the answer but are not always the answer.

### Edge Case Mistakes

Forgot:

```text
If the third distinct maximum does not exist,
return the maximum number.
```

## Biggest Learning

```text
Helper variables help find the answer.

They are not necessarily the answer themselves.
```

Example:

```java
count
```

helped locate the third distinct maximum but was not the final answer.

---

# 2. LeetCode 26 — Remove Duplicates from Sorted Array

## What I Learned

- My first proper Two Pointer problem.
- Difference between Read Pointer and Write Pointer.
- Arrays can be modified in-place.
- Not every problem requires creating a new array.
- Sorted arrays make duplicate detection easier.

## Mistakes I Made

### Wrong Understanding

Initially thought:

```text
I only need to count unique elements.
```

But the actual task was:

```text
Move unique elements to the beginning of the same array.
```

### Unnecessary Array

Tried creating:

```java
expectedNums
```

even though the problem required modifying:

```java
nums
```

itself.

### Index Mistakes

Used:

```java
nums[i-1]
```

without considering the first index.

Used:

```java
nums[i+1]
```

which caused boundary issues.

### Value vs Count Confusion

Tried:

```java
nums[k] = unique;
```

instead of:

```java
nums[k] = nums[i];
```

### Return Mistakes

- Returned inside the loop.
- Tried returning an array when the function expected an integer.

### Variable Understanding

Initially did not understand what:

```java
k
```

represented.

Later learned:

```text
k = next position where a unique value should be stored.
```

## Biggest Learning

```text
i = Read Pointer
k = Write Pointer
```

Read Pointer scans the array.

Write Pointer stores valid unique values.

This is a very important LeetCode pattern.

---

# Day 4 Reflection

These two problems felt much harder than my previous Easy problems.

The main reason was not syntax.

The difficulty was understanding:

- What each variable represents.
- What the actual answer is.
- How to handle duplicates.
- How to think about edge cases.
- How to modify arrays in-place.

## Biggest Improvement Today

Instead of immediately writing code, I started:

```text
Reading the problem

↓

Manually tracing examples in my notebook

↓

Understanding the logic

↓

Writing code
```

This reduced many mistakes and helped me debug faster.

🚀 Day 4 Completed
✅ 20 LeetCode Problems Solved
✅ Learned Two Pointers
✅ Improved Manual Problem Decoding

# DAILY LEARNING LOG

## Day 5 (21-07-2026)

Problems Solved:
- LeetCode 344 - Reverse String
- LeetCode 125 - Valid Palindrome
- LeetCode 58 - Length of Last Word

Concepts Learned:
- Two Pointers
- String Cleaning
- Character.toLowerCase()
- Character.isLetterOrDigit()
- Reverse Traversal
- Early Return
- Counting Pattern

Common Mistakes Today:
- Using s.length instead of s.length - 1.
- Mixing array syntax and string syntax.
- Using = instead of ==.
- Forgetting charAt() returns a char.
- Initializing variables before required data was prepared.
- Returning wrong values at end of method.

Patterns Reinforced:
1. Two Pointer Pattern
2. Reverse Traversal Pattern
3. Clean Data → Process Data Pattern
4. Count Until Boundary Pattern

Time Spent:
- Reverse String: ~15 min
- Valid Palindrome: ~45 min
- Length of Last Word: ~20 min

Total Learning Time:
~1.5 hours

Confidence Level:
8/10

Notes to Future Me:
Focus less on syntax mistakes and more on trusting the pattern. Most bugs today came from Java syntax, not logic.

# DAY 6 LEARNING LOG (22-07-2026)

## Problems Solved

1. LeetCode 28 - Find the Index of the First Occurrence in a String
2. LeetCode 796 - Rotate String
3. LeetCode 242 - Valid Anagram

---

# LeetCode 28 - Find the Index of the First Occurrence in a String

## Difficulty

Easy

## Concepts Used

- Nested Loops
- String Traversal
- Character Comparison
- Brute Force Search
- Break Statement
- Early Return
- Boundary Conditions

## Final Approach

1. Choose every possible starting position in `haystack`.
2. Compare every character of `needle`.
3. If mismatch occurs, stop checking current position.
4. If all characters match, return starting index.
5. If no match exists, return `-1`.

## Mistakes I Made

- Compared `haystack[i]` with every character of `needle`.
- Returned `-1` immediately on mismatch.
- Didn't know how to detect a complete match.
- Forgot boundary condition for outer loop.
- Returned `0` instead of `-1` when substring wasn't found.
- Didn't initially understand why `i + j` was needed.
- Mixed up `break` and `return`.

## Biggest Learning

When matching strings:

```java
haystack.charAt(i + j)
needle.charAt(j)
```

The haystack moves using `i + j`, while the pattern moves using `j`.

## Pattern Learned

Choose Start Position
↓
Compare Entire Pattern
↓
Mismatch → Break
↓
Complete Match → Return Start Index

## Time Complexity

O(n × m)

## Space Complexity

O(1)

## Confidence

Solved mostly by myself after understanding boundary conditions.

---

# LeetCode 796 - Rotate String

## Difficulty

Easy

## Concepts Used

- String Rotation
- String Concatenation
- Length Check
- contains()
- Pattern Recognition

## Final Approach

1. Check if lengths are equal.
2. Concatenate:

```java
s + s
```

3. Check if `goal` exists inside `(s + s)`.
4. Return result.

## Key Observation

All rotations of a string exist inside:

```java
s + s
```

Example:

```text
abcdeabcde
```

Contains:

```text
abcde
bcdea
cdeab
deabc
eabcd
```

## Mistakes I Made

- First thought about manually shifting characters.
- Wanted to use loops unnecessarily.
- Added a loop around `contains()` without using the loop variable.
- Forgot equal length check.
- Focused on simulation before finding the pattern.

## Biggest Learning

Sometimes one observation removes all complex logic.

For rotation problems:

```java
(s + s).contains(goal)
```

is the key idea.

## Pattern Learned

Length Check
↓
Concatenate String
↓
Use contains()
↓
Return Result

## Useful Functions

```java
length()
contains()
```

## Time Complexity

O(n²)

## Space Complexity

O(n)

## Confidence

Solved after understanding the hidden rotation pattern.

---

# LeetCode 242 - Valid Anagram

## Difficulty

Easy

## Concepts Used

- Frequency Array
- Character Counting
- String Traversal
- Length Check
- Character to Index Mapping

## Final Approach

1. Check if lengths are equal.
2. Create:

```java
int[] freq = new int[26];
```

3. Traverse `s` and increase counts.
4. Traverse `t` and decrease counts.
5. Check if every frequency becomes 0.
6. Return result.

## Character Mapping Learned

```java
'a' - 'a' = 0
'b' - 'a' = 1
'c' - 'a' = 2
...
'z' - 'a' = 25
```

Pattern:

```java
freq[s.charAt(i) - 'a']++;
freq[t.charAt(i) - 'a']--;
```

## Mistakes I Made

### Logic Mistakes

- Thought checking character presence was enough.
- Didn't realize frequencies must also match.
- Didn't understand what frequency arrays store.
- Tried comparing counts directly with characters.

### Syntax Mistakes

- Tried:

```java
freq[i] == s[i]
```

- Forgot to use:

```java
s.charAt(i)
```

- Mixed character values and frequency counts.

### Frequency Array Mistakes

- Didn't understand character-to-index conversion.
- Thought frequency array stores characters.
- Returned `true` when finding the first zero frequency.
- Forgot all frequencies must become zero.

## Biggest Learning

Frequency arrays store counts, not characters.

Example:

```java
freq[0]
```

means:

```text
Count of 'a'
```

not the character `'a'`.

## Pattern Learned

Length Check
↓
Count Characters (+)
↓
Remove Characters (-)
↓
Verify All Counts Are Zero

## Time Complexity

O(n)

## Space Complexity

O(1)

## Confidence

Learned frequency arrays for the first time and understood the complete counting pattern.

---

# DAY 6 OVERALL LESSONS

## Major Patterns Learned

### 1. Brute Force String Matching

```text
Choose Start
↓
Compare Pattern
↓
Break on Mismatch
↓
Return on Match
```

### 2. String Rotation Pattern

```text
Length Check
↓
s + s
↓
contains()
```

### 3. Frequency Array Pattern

```text
Count
↓
Subtract
↓
Verify Zero
```

---

## Most Common Mistakes Today

- Returning too early.
- Missing boundary conditions.
- Using loops when a pattern already solved the problem.
- Confusing counts with characters.
- Not understanding what data structures store.
- Thinking about implementation before finding the pattern.

---

## Biggest Day 6 Takeaway

```text
Look for patterns before writing code.
```

Today I learned that many string problems become much easier after identifying the underlying pattern rather than immediately starting with loops.

---

## Day 6 Reflection

Today was a strong learning day.

I learned:

- String Matching
- String Rotation
- Frequency Arrays

The most valuable concept was Frequency Arrays because it introduced a completely new way of solving string problems efficiently.

Confidence: 8.5/10 🚀

Total Problems Solved: 3
LeetCode Journey Day: 6
Date: 22-07-2026


# DAY 7 LEARNING LOG
Date: 23-07-2026

## Problems Solved

1. LeetCode 709 - To Lower Case
2. LeetCode 771 - Jewels and Stones
3. LeetCode 1108 - Defanging an IP Address

---

# LeetCode 709 - To Lower Case

## Difficulty

Easy

## Concepts Used

- String Traversal
- Character Comparison
- ASCII Values
- Character Conversion
- String Building

## Final Approach

1. Traverse the string.
2. Check whether the current character is uppercase.
3. If uppercase, convert it to lowercase using ASCII difference.
4. Add the character to a new string.
5. Return the final string.

## Key Observation

```java
'A' = 65
'a' = 97
```

Difference:

```java
32
```

Conversion:

```java
ch = (char)(ch + 32);
```

## Mistakes I Made

- Declared `char ch` twice.
- Tried using `ch(i)` as if it were a function.
- Forgot that String is immutable.
- Initially added characters only inside the uppercase `if` block.
- Forgot lowercase characters also need to be added to the answer string.
- Didn't know where to store converted characters.

## Biggest Learning

```text
Convert if needed
↓
Always add character to answer
```

The placement of a line inside or outside an `if` block can completely change the result.

## Pattern Learned

Traverse String
↓
Check Condition
↓
Modify Character
↓
Build New String
↓
Return Result

## Time Complexity

O(n)

## Space Complexity

O(n)

---

# LeetCode 771 - Jewels and Stones

## Difficulty

Easy

## Concepts Used

- Nested Loops
- Character Comparison
- Searching
- Break Statement
- Counting Pattern

## Final Approach

1. Traverse every stone.
2. Check whether it exists in jewels.
3. If found:
   - Increase count.
   - Break inner loop.
4. Return count.

## Final Pattern

```text
For each stone
↓
Search all jewels
↓
Found?
↓
count++
↓
break
```

## Mistakes I Made

- Returned `0` immediately on first mismatch.
- Thought one failed comparison means the answer is zero.
- Added unnecessary `else` block.
- Forgot that a mismatch only means:
  
```text
Try the next jewel
```

- Needed reminder about when to use `break`.

## Biggest Learning

```text
One comparison fails
↓
Try next possibility

NOT

One comparison fails
↓
Return immediately
```

This was similar to mistakes I previously made in string matching problems.

## Pattern Learned

Nested Loop Search Pattern

```text
Outer Loop
↓
Thing being counted

Inner Loop
↓
Place being searched
```

## Time Complexity

O(n × m)

## Space Complexity

O(1)

---

# LeetCode 1108 - Defanging an IP Address

## Difficulty

Easy

## Concepts Used

- String Traversal
- Character Comparison
- Conditional Replacement
- String Building

## Final Approach

1. Traverse the IP address.
2. If current character is '.':
   
```java
"[.]"
```

is added.

3. Otherwise add the original character.
4. Return final string.

## Mistakes I Made

- None major.
- Correctly identified the pattern before writing code.
- Immediately recognized that only one loop and one condition were required.

## Biggest Learning

Sometimes the simplest approach is already the correct solution.

Not every string problem requires complicated logic.

## Pattern Learned

Traverse String
↓
Check Character
↓
Replace If Needed
↓
Build Answer String

## Time Complexity

O(n)

## Space Complexity

O(n)

---

# DAY 7 OVERALL LESSONS

## Major Patterns Reinforced

### String Building Pattern

```java
String ans = "";
```

```java
ans = ans + ch;
```

Used in:
- Valid Palindrome
- To Lower Case
- Defanging IP Address

---

### Nested Loop Search Pattern

```text
Item
↓
Search Collection
↓
Found?
↓
Process
↓
break
```

Used in:
- Jewels and Stones

---

### Conditional Character Processing

```java
if(condition)
{
    modify
}
```

```java
add to answer
```

Used in:
- To Lower Case
- Defanging IP Address

---

# Biggest Day 7 Observation

Today I noticed that I am starting to recognize patterns before writing code.

Examples:

- Immediately identified one-loop solution for Defanging IP Address.
- Understood Nested Loop Search for Jewels and Stones.
- Already knew ASCII conversion logic for To Lower Case.

Most of my mistakes are now implementation mistakes rather than logic mistakes.

---

# Day 7 Reflection

Today I felt more comfortable identifying the correct approach before coding.

I still make small syntax and implementation mistakes, but I am increasingly able to recognize the underlying pattern of a problem.

The biggest improvement today was confidence in choosing the correct logic without needing much guidance.

Confidence: 9/10

Total Problems Solved Today: 3

LeetCode Journey Day: 7 🚀


# DAY 8 LEARNING LOG

**Date:** 24-07-2026

## Problems Solved

1. LeetCode 69 - Sqrt(x)
2. LeetCode 231 - Power of Two
3. LeetCode 326 - Power of Three

---

# LeetCode 69 - Sqrt(x)

## Difficulty

Easy

## Concepts Used

- Binary Search
- Search Space
- Mid Calculation
- Floor Value
- Overflow Handling

## Initial Approach

### Brute Force

```text
Try numbers one by one
↓
Square them
↓
Stop when square exceeds x
↓
Return previous number
```

Example:

```text
x = 8

1² = 1
2² = 4
3² = 9 ❌

Answer = 2
```

## Final Approach

Use Binary Search.

```text
low = 0
high = x
```

Find:

```text
mid
```

Check:

```text
mid²
```

Cases:

```text
mid² == x
↓
Return mid
```

```text
mid² < x
↓
Store answer
↓
Search right side
```

```text
mid² > x
↓
Search left side
```

## Mistakes I Made

- Started with brute force only.
- Did not initially think about large inputs.
- Needed help understanding why Binary Search works.
- Learned why `long` is used for:

```java
(long)mid * mid
```

to prevent overflow.

## Biggest Learning

Binary Search is not only for finding elements.

It can also be used to find an answer inside a sorted numeric range.

## Pattern Learned

```text
Search Space
↓
Middle Value
↓
Condition Check
↓
Move Left or Right
↓
Store Best Answer
```

## Time Complexity

```text
O(log n)
```

## Space Complexity

```text
O(1)
```

---

# LeetCode 231 - Power of Two

## Difficulty

Easy

## Concepts Used

- Repeated Division
- Modulus Operator
- Loop Conditions
- Mathematical Pattern

## Initial Thinking

At first I thought:

```java
n % 2 == 0
```

would be enough.

Then I realized:

```text
6
10
12
18
```

are even but not powers of two.

## Final Approach

Keep dividing by 2 while divisible.

Example:

```text
16
↓
8
↓
4
↓
2
↓
1
```

If final value becomes:

```text
1
```

Return:

```text
true
```

Otherwise:

```text
false
```

## Mistakes I Made

### Attempt 1

Thought:

```java
n % 2 == 0
```

alone proves power of two.

### Attempt 2

Used:

```java
while(n != 0)
```

which divided too long.

Example:

```text
16
↓
8
↓
4
↓
2
↓
1
↓
0
```

Then answer became incorrect.

### Final Fix

Changed stopping condition to:

```java
while(n % 2 == 0)
```

which correctly stops at:

```text
1
```

## Biggest Learning

The operation may be correct.

The stopping condition can still be wrong.

## Pattern Learned

```text
Repeated Division
↓
Stop At Boundary
↓
Check Final Value
```

## Thought Process Growth

```text
Check even number
↓
Realize that's not enough
↓
Repeated division
↓
Wrong stopping condition
↓
Correct stopping condition
↓
Accepted logic
```

## Time Complexity

```text
O(log n)
```

## Space Complexity

```text
O(1)
```

---

# LeetCode 326 - Power of Three

## Difficulty

Easy

## Concepts Used

- Pattern Reuse
- Repeated Division
- Mathematical Verification

## Key Observation

This problem is almost identical to Power of Two.

Instead of:

```text
Divide by 2
```

we:

```text
Divide by 3
```

Example:

```text
27
↓
9
↓
3
↓
1
```

Final value:

```text
1
```

Therefore:

```text
true
```

## Mistakes I Made

Accidentally checked:

```java
n % 2
```

instead of:

```java
n % 3
```

Accidentally checked:

```java
if(n == 2)
```

instead of:

```java
if(n == 1)
```

Forgot that the pattern should end at:

```text
1
```

just like Power of Two.

## Biggest Learning

Once a pattern is learned, many new problems become small modifications of the same idea.

Power of Three is basically:

```text
Power of Two Pattern
+
Replace 2 with 3
```

## Pattern Learned

```text
Repeated Division
↓
While Divisible
↓
Reduce Number
↓
Reach 1
↓
Valid Power
```

## Time Complexity

```text
O(log₃ n)
```

## Space Complexity

```text
O(1)
```

---

# DAY 8 OVERALL LESSONS

## Major Patterns Reinforced

### Binary Search On Answer

```text
Search Space
↓
Middle
↓
Condition
↓
Move Left / Right
↓
Store Best Answer
```

Used In:

- LeetCode 69

---

### Repeated Division Pattern

```text
While divisible
↓
Divide
↓
Stop
↓
Check final value
```

Used In:

- LeetCode 231
- LeetCode 326

---

## Biggest Day 8 Observation

Today I noticed that I am becoming much better at recognizing patterns from previously solved problems.

For Power of Three, I immediately connected it with Power of Two.

Instead of learning a completely new solution, I only had to modify an existing pattern.

This is the first time I strongly felt that solving previous problems is helping me solve new ones faster.

## Personal Reflection

Today I learned an important difference:

```text
Knowing the operation
≠
Knowing the stopping condition
```

In Power of Two, my division logic was correct from the beginning.

The real bug was deciding when to stop.

I also learned that Binary Search is much more powerful than I originally thought.

It is not just for searching elements.

It can also search for answers.

## Confidence

- Logic Understanding: 9/10
- Pattern Recognition: 9/10
- Java Syntax Confidence: 7/10
- Binary Search Understanding: 7.5/10
- Overall Progress: Strong

## Final Day 8 Reflection

Earlier I focused mostly on solving one problem at a time.

Today I started recognizing relationships between problems.

I am beginning to build a library of patterns in my mind:

- Two Pointers
- Frequency Arrays
- Reverse Traversal
- String Building
- Nested Loop Search
- Binary Search
- Repeated Division

This makes new problems feel less like completely new challenges and more like variations of patterns I already know.

**Total Problems Solved Today: 3**

**LeetCode Journey Day: 8 🚀**


# DAY 9 LEARNING LOG

**Date:** 25-07-2026

## Problems Solved

1. LeetCode 507 - Perfect Number
2. LeetCode 202 - Happy Number
3. LeetCode 263 - Ugly Number
4. LeetCode 367 - Valid Perfect Square

---

# LeetCode 507 - Perfect Number

## Difficulty

Easy

## Concepts Used

- Factors / Divisors
- Loops
- Accumulation Pattern
- Mathematical Verification

## Initial Thinking

Check every number from:

```text
1 to num
```

and add divisors.

## Mistakes I Made

### Mistake 1

Tried:

```java
num.length
```

on an integer.

### Mistake 2

Used:

```java
else
{
    return false;
}
```

inside loop.

I assumed one non-divisor means the number is not perfect.

### Mistake 3

Checked:

```java
if(sum == num)
```

inside loop before processing all divisors.

### Mistake 4

Included:

```java
i <= num
```

which also adds the number itself.

Perfect numbers use:

```text
Proper Divisors
=
All divisors except the number itself
```

## Final Approach

```text
Traverse from 1 to num-1
↓
If divisor
↓
Add to sum
↓
After loop
↓
Compare sum with num
```

Example:

```text
28

1 + 2 + 4 + 7 + 14
=
28
```

## Biggest Learning

Just because one condition fails inside a loop does not mean the final answer is false.

Sometimes the answer can only be decided after processing everything.

## Pattern Learned

```text
Initialize Sum
↓
Check Divisors
↓
Accumulate
↓
Final Comparison
```

## Time Complexity

O(n)

## Space Complexity

O(1)

---

# LeetCode 202 - Happy Number

## Difficulty

Easy

## Concepts Used

- Digit Extraction
- Modulus Operator
- Nested Loops
- State Transformation
- HashSet
- Cycle Detection

## Initial Thinking

Extract digits.

Square them.

Add them.

Check if sum becomes 1.

## Progress Journey

### Attempt 1

Incorrect digit extraction.

### Attempt 2

Correctly extracted digits using:

```java
n % 10
```

### Attempt 3

Built square sum correctly.

### Attempt 4

Realized process must repeat.

```text
19
↓
82
↓
68
↓
100
↓
1
```

### Attempt 5

Built:

```text
Outer Loop
↓
Repeat Process

Inner Loop
↓
Process Digits
```

### Final Problem

TLE.

Because some numbers never reach 1.

Example:

```text
2
↓
4
↓
16
↓
37
↓
58
↓
89
↓
145
↓
42
↓
20
↓
4
```

Cycle detected.

## New Concept Learned

HashSet

Purpose:

```text
Store already visited numbers
↓
If number appears again
↓
Cycle detected
↓
Return false
```

## Biggest Learning

This is my first cycle detection problem.

Not every repeated process eventually ends.

Sometimes we must remember previous states.

## Pattern Learned

```text
Current State
↓
Generate Next State
↓
Store State
↓
Check Repetition
↓
Cycle Detection
```

## Time Complexity

O(log n) per transformation cycle

## Space Complexity

O(k)

(k = number of unique values encountered)

---

# LeetCode 263 - Ugly Number

## Difficulty

Easy

## Concepts Used

- Repeated Division
- Modulus Operator
- Mathematical Pattern
- Prime Factors

## Key Observation

Ugly numbers only contain:

```text
2
3
5
```

as prime factors.

## Final Approach

```text
While divisible by 2
↓
Divide by 2

While divisible by 3
↓
Divide by 3

While divisible by 5
↓
Divide by 5

Final value == 1
↓
Ugly Number
```

Example:

```text
30
↓
15
↓
5
↓
1
```

Return:

```text
true
```

## Mistakes I Made

Initially treated it similarly to Power of Two.

Needed to realize there are three allowed factors:

```text
2
3
5
```

instead of one.

## Biggest Learning

Many problems are extensions of previous patterns.

Ugly Number is basically:

```text
Power of Two Pattern
+
Multiple Valid Divisors
```

## Pattern Learned

```text
Repeated Division
↓
Remove Allowed Factors
↓
Check Remaining Number
```

## Time Complexity

O(log n)

## Space Complexity

O(1)

---

# LeetCode 367 - Valid Perfect Square

## Difficulty

Easy

## Concepts Used

- Binary Search
- Search Space
- Mid Calculation
- Overflow Handling
- Pattern Recognition

## Biggest Realization

This problem looked new.

But after reading it, I immediately recognized:

```text
Perfect Square
↓
Sqrt(x)
↓
Same Binary Search Pattern
```

This was the biggest achievement of today.

## Initial Thought

Instead of checking every number:

```text
1²
2²
3²
...
```

Use Binary Search.

## Final Approach

```text
low
high
↓
mid
↓
mid²

Equal?
↓
true

Too Small?
↓
Right Side

Too Large?
↓
Left Side
```

## Mistakes I Avoided

Because I already solved:

```text
LeetCode 69 - Sqrt(x)
```

I already knew:

```java
long square = (long) mid * mid;
```

to avoid overflow.

## Biggest Learning

Not every new problem needs a new algorithm.

Sometimes it is the same pattern hidden inside a different question.

## Pattern Learned

```text
Binary Search On Answer
↓
Check Candidate
↓
Move Left / Right
↓
Find Exact Match
```

## Time Complexity

O(log n)

## Space Complexity

O(1)

---

# DAY 9 OVERALL LESSONS

## Major Patterns Reinforced

### Repeated Division Pattern

```text
While Divisible
↓
Reduce Number
↓
Check Final Value
```

Used In:

```text
Power of Two
Power of Three
Ugly Number
```

---

### Binary Search On Answer

```text
Search Space
↓
Middle
↓
Condition
↓
Move Left / Right
```

Used In:

```text
Sqrt(x)
Valid Perfect Square
```

---

### State Transformation Pattern

```text
Current State
↓
Generate New State
↓
Repeat
↓
Detect Cycle
```

Used In:

```text
Happy Number
```

---

## Personal Reflection

Today I had a very important realization.

Earlier, every new LeetCode problem looked completely different.

Now I am starting to recognize patterns.

The biggest example was:

```text
LeetCode 367
↓
Immediately connected it to
LeetCode 69
↓
Applied Binary Search without learning a new algorithm
```

I still make syntax mistakes sometimes, but my ability to recognize logic and patterns is becoming much stronger.

My bottleneck is slowly shifting from:

```text
Understanding Logic
```

to:

```text
Expressing Logic Correctly In Code
```

which is a sign of progress.

signing off ,
seeya on day 10.

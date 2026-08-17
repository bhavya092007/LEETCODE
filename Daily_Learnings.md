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


# DAY 10 LEARNING LOG

**Date:** 26-07-2026

## Problems Solved

- LeetCode 3658 — GCD of Odd and Even Sums

---

# LeetCode 3658 - GCD of Odd and Even Sums

## Difficulty

Easy

## Concepts Used

- GCD (Greatest Common Divisor)
- Odd Numbers
- Even Numbers
- Mathematical Observation
- Pattern Recognition

## Initial Thinking

At first, the problem looked like it would require:

```text
Generate odd numbers
↓
Generate even numbers
↓
Calculate both sums
↓
Find GCD
```

which seemed longer than necessary.

---

## Key Observation

After analyzing the pattern:

```text
First n odd numbers
=
n²

First n even numbers
=
n(n + 1)
```

The problem becomes:

```text
GCD(n² , n(n+1))
```

Factor out:

```text
GCD(n² , n(n+1))

=
n × GCD(n , n+1)
```

Since consecutive numbers always have:

```text
GCD(n , n+1) = 1
```

The final answer becomes:

```text
n
```

---

## Final Approach

```java
return n;
```

---

## Biggest Learning

Not every math problem requires simulation.

Sometimes the entire problem collapses into a mathematical identity.

Instead of:

```text
Build values
↓
Calculate
↓
Find answer
```

it became:

```text
Observe pattern
↓
Simplify expression
↓
Direct answer
```

---

## Mistakes I Made

None in implementation.

The challenge was understanding why:

```java
return n;
```

works.

The important part was proving the mathematics behind it.

---

## Pattern Learned

```text
Look For Formula
↓
Replace Repeated Computation
↓
Simplify Expression
↓
Return Direct Result
```

---

## Time Complexity

```text
O(1)
```

## Space Complexity

```text
O(1)
```

---

# DAY 10 OVERALL LESSONS

## Major Learning

Today reinforced an important idea:

```text
Not every problem needs loops.
Not every problem needs arrays.
Not every problem needs simulation.
```

Sometimes:

```text
Math Observation
>
Implementation
```

---

## Personal Reflection

Compared to my earlier days:

```text
Read Problem
↓
Think About Loops
```

I am slowly developing a new habit:

```text
Read Problem
↓
Look For Pattern
↓
Look For Formula
↓
Then Think About Code
```

Today's problem was a reminder that recognizing a mathematical pattern can completely eliminate the need for complex code.

---

## Growth Observation

Recently I have started recognizing:

```text
Binary Search Patterns
Repeated Division Patterns
Frequency Array Patterns
Mathematical Formula Patterns
```

This means my focus is shifting from:

```text
How do I write code?
```

to:

```text
What pattern is hidden in this problem?
```

That is one of the biggest improvements in my problem-solving journey so far.

---

## Biggest Learning Of Day 10

```text
The shortest solution is often the result of
the deepest observation.
```

Today's accepted solution:

```java
return n;
```

looked trivial,

but the real challenge was understanding *why* it works.



signing off 
seeya on day 11


# DAY 11 LEARNING LOG

**Date:** 27-07-2026

## Problems Solved

- LeetCode 217 — Contains Duplicate
- LeetCode 20 — Valid Parentheses

---

# LeetCode 217 - Contains Duplicate

## Difficulty

Easy

## Concepts Used

- HashSet
- Duplicate Detection
- Enhanced For Loop
- Seen Before Pattern

## Initial Thinking

The goal was:

```text
Check whether any number appears more than once.
```

At first, the natural approach is:

```text
Compare every element with every other element
↓
Find duplicate
```

which leads to:

```text
Nested Loops
O(n²)
```

---

## Better Observation

The problem can be simplified to:

```text
Have I seen this number before?
```

If yes:

```text
Duplicate exists
↓
Return true
```

Otherwise:

```text
Store it
↓
Continue
```

---

## HashSet Pattern Learned

```java
HashSet<Integer> set = new HashSet<>();
```

Operations learned:

```java
set.add(num);
set.contains(num);
```

---

## Biggest Learning

HashSet is useful when we need:

```text
Fast lookup
↓
Seen Before?
```

instead of repeatedly searching the entire array.

---

## New Concepts Reinforced

```java
for(int num : nums)
```

Expanded version:

```java
for(int i = 0; i < nums.length; i++)
{
    int num = nums[i];
}
```

---

## Pattern Learned

```text
Traverse
↓
Already Seen?
↓
Yes → Return
↓
No → Store
```

---

## Time Complexity

```text
O(n)
```

## Space Complexity

```text
O(n)
```

---

# LeetCode 20 - Valid Parentheses

## Difficulty

Easy

## Concepts Used

- Stack
- LIFO
- Push
- Pop
- Matching Pairs

---

## Initial Understanding

The problem looked like:

```text
Opening Brackets
Closing Brackets
Matching Them
```

But the important observation was:

```text
Last Opened
↓
First Closed
```

which is exactly:

```text
LIFO
(Last In First Out)
```

and therefore:

```text
Stack
```

---

## Stack Operations Learned

### Push

```java
stack.push(ch);
```

Store opening brackets.

---

### Pop

```java
char top = stack.pop();
```

Retrieve the most recently opened bracket.

---

### Empty Check

```java
stack.isEmpty()
```

Used to prevent invalid closing brackets.

---

## Example

```text
([{}])

Push (
Push [
Push {

Pop {
Pop [
Pop (

Valid
```

---

## Biggest Learning

Not every problem is about loops.

Sometimes the real challenge is identifying:

```text
Which Data Structure Fits?
```

For this problem:

```text
Stack
```

was the correct answer.

---

## Pattern Learned

```text
Opening Bracket
↓
Push

Closing Bracket
↓
Pop

Match?
↓
Continue

Mismatch?
↓
False
```

---

## New Data Structure Learned

```java
Stack<Character> stack = new Stack<>();
```

Operations:

```java
stack.push()
stack.pop()
stack.isEmpty()
```

---

## Time Complexity

```text
O(n)
```

## Space Complexity

```text
O(n)
```

---

# DAY 11 OVERALL LESSONS

## Major Concepts Learned

### HashSet

```text
Store Unique Values
↓
Fast Lookup
↓
Seen Before Pattern
```

Used In:

```text
LeetCode 217
```

---

### Stack

```text
Last Opened
↓
First Closed
```

Used In:

```text
LeetCode 20
```

---

## Personal Reflection

Today was an important day because I worked with two completely different data structures:

```text
HashSet
Stack
```

Earlier, most problems were solved using:

```text
Loops
Conditions
Arrays
```

Today introduced a new level of thinking:

```text
Problem
↓
Identify Pattern
↓
Choose Data Structure
↓
Implement Solution
```

---

## Growth Observation

My journey is slowly moving from:

```text
How do I write the code?
```

towards:

```text
Which pattern does this problem belong to?
```

Patterns learned so far:

```text
Frequency Array
Binary Search
Repeated Division
HashSet
Stack
Mathematical Observation
```

---

## Biggest Learning Of Day 11

```text
A problem becomes much easier
once the correct data structure is identified.
```

Today reinforced that:

```text
Contains Duplicate
→ HashSet

Valid Parentheses
→ Stack
```
# DAY 11 ADDITIONAL LEARNING LOG

## Problem Solved

- LeetCode 1464 — Maximum Product of Two Elements in an Array

---

## Difficulty

Easy

## Concepts Used

- Brute Force
- Optimization
- Largest Element Tracking
- Second Largest Element Tracking
- Single Pass Traversal

---

## Initial Thinking

My first instinct was:

```text
Choose every possible pair
↓
Calculate product
↓
Keep the maximum
```

This naturally led to:

```java
for(i)
{
    for(j)
    {
        ...
    }
}
```

which is the classic:

```text
Brute Force
```

approach.

---

## Mistakes I Made

### Mistake 1

I initially used:

```java
max = nums[i] * nums[j];
```

and then checked:

```java
if(nums[i] * nums[j] > max)
```

which can never become true because I had already assigned the same value to `max`.

---

### Mistake 2

I forgot that the problem asks for:

```java
(nums[i] - 1) * (nums[j] - 1)
```

and not:

```java
nums[i] * nums[j]
```

This is a common mistake where I understand the idea but miss a small detail from the formula.

---

## Brute Force Pattern

```text
Try every pair
↓
Compute answer
↓
Keep maximum
```

Example:

```text
[3,4,5,2]

(3-1)*(4-1)
(3-1)*(5-1)
(4-1)*(5-1)
...
```

Complexity:

```text
Time  : O(n²)
Space : O(1)
```

---

## Important Observation

After thinking more carefully, I realized:

```text
To maximize

(nums[i]-1)*(nums[j]-1)

I only need the two largest numbers.
```

Nothing else matters.

---

## Optimized Approach

Track:

```text
Largest Number
Second Largest Number
```

while traversing the array only once.

Pattern:

```text
Current Number
↓
Bigger than Largest?
↓
Update Largest
↓
Old Largest becomes Second Largest
```

Otherwise:

```text
Bigger than Second Largest?
↓
Update Second Largest
```

---

## Optimized Pattern Learned

```text
Find Largest
↓
Find Second Largest
↓
Compute Answer
```

Code idea:

```java
max1 = largest
max2 = second largest
```

Answer:

```java
(max1 - 1) * (max2 - 1)
```

---

## Biggest Learning

Today I learned that many brute-force problems can be simplified by asking:

```text
What information actually matters?
```

For this problem:

```text
Every pair does NOT matter.
Only the two largest values matter.
```

This observation reduced:

```text
O(n²)
```

to:

```text
O(n)
```

---

## New Pattern Added To My Collection

### Largest + Second Largest Tracking

```text
Traverse Once
↓
Maintain Largest
↓
Maintain Second Largest
↓
Compute Answer
```

Common Uses:

```text
Maximum Product
Maximum Sum Pair
Best Two Elements
Maximum Difference
```

---

## Personal Reflection

I noticed that my first solution is usually becoming correct logically.

The next step I am improving on is:

```text
Finding observations
↓
Reducing unnecessary work
↓
Optimizing
```

This is a sign that my problem-solving mindset is improving from:

```text
Can I solve it?
```

to:

```text
Can I solve it better?
```

seeya on day 12

# LeetCode Journey Log - Day 12

Date: 28-07-2026

## Problems Solved

1. 278 - First Bad Version
2. 374 - Guess Number Higher or Lower
3. 852 - Peak Index in a Mountain Array


## Today's Main Topic

Binary Search Pattern

Today I learned how Binary Search is not only used for searching elements,
but also for finding answers in problems where we can eliminate half of
the search space.


## Concepts Learned

- Binary Search
- Search Space Reduction
- Monotonic Pattern Recognition
- Finding Boundaries
- Mountain Array Pattern


## Important Realization

Before today, I thought Binary Search means:

"Search a number in a sorted array"

But today I learned:

Binary Search is a technique where:

"If one comparison can remove half of the possible answers,
Binary Search can be applied."


## Problems Pattern

### 278 - First Bad Version

Pattern:
Binary Search on Answer

Learning:
- We don't search an element.
- We search the first position where condition becomes true.

Concept:

False False False True True True

Need to find first True.


---

### 374 - Guess Number Higher or Lower

Pattern:
Binary Search with API condition

Learning:
- Compare mid with target.
- According to result, eliminate half.

Conditions:

Too High → Search Left

Too Low → Search Right

Correct → Answer


---

### 852 - Peak Index in Mountain Array

Pattern:
Binary Search on Mountain Array

Learning:
- Compare arr[mid] and arr[mid+1]
- Decide whether peak is left or right.

Increasing side:

arr[mid] < arr[mid+1]

Peak is on right.


Decreasing side:

arr[mid] > arr[mid+1]

Peak is on left or mid.


## Time Complexity

All three problems:

O(log n)


## Progress

Day 12 completed.

Binary Search pattern recognition improved.

seeya on day 13🚀


# DAY 13 LEARNING LOG

**Date:** 29-07-2026

## Problems Solved

- LeetCode 1539 — Kth Missing Positive Number

---

## Difficulty

Easy

## Concepts Used

- Missing Number Pattern
- Pointer Traversal
- Counting Technique
- Simulation
- Observation-Based Problem Solving

---

## Why Only One Problem Today?

Today was a travel day, so I had limited time available for problem solving.

Instead of forcing multiple problems, I focused on understanding one problem properly and extracting as much learning as possible from it.

Current mindset:

```text
Consistency > Quantity
```

Even one problem solved with understanding is better than many problems solved mechanically.

---

## Initial Thinking

My first idea was:

```text
Compare array elements with indices
↓
Store missing numbers in a new array
↓
Return kth missing number
```

While trying to implement this approach, I realized:

```text
arr[i] and i are not directly related.
```

The problem is not asking about indices.

The problem is asking about:

```text
Positive numbers that are missing.
```

---

## Important Realization

Instead of focusing on:

```text
Array Index
```

I needed to focus on:

```text
Expected Positive Numbers

1,2,3,4,5,6,7...
```

and compare them against the array.

Example:

```text
arr = [2,3,4,7,11]
```

Checking numbers:

```text
1 → Missing
2 → Present
3 → Present
4 → Present
5 → Missing
6 → Missing
7 → Present
8 → Missing
9 → Missing
...
```

Missing sequence:

```text
1,5,6,8,9,...
```

---

## Final Approach

Use two variables:

```java
current
count
```

Where:

```text
current → Number being checked

count → Missing numbers found so far
```

Also maintain:

```java
i
```

to track position inside the array.

Logic:

```text
If current exists in array
↓
Move array pointer

Else
↓
Missing number found
↓
Increase count

If count == k
↓
Return current
```

---

## Biggest Learning

I learned that:

```text
Not every problem is about array indices.
```

Sometimes the real task is to simulate a sequence and compare it with the given data.

I also learned that:

```text
Creating an extra array
```

is often unnecessary.

Instead:

```text
Count while traversing
```

can solve the same problem with less memory.

---

## New Pattern Learned

### Missing Number Counting Pattern

```text
Generate Expected Number
↓
Check Presence
↓
If Missing
    Increase Count
↓
When Count == k
    Return Answer
```

---

## Mistakes I Made

### Mistake 1

Tried:

```java
arr[i] == i
```

which does not represent missing positive numbers.

---

### Mistake 2

Tried storing missing numbers in another array before understanding the pattern completely.

---

### Mistake 3

Focused on indices instead of focusing on:

```text
Expected Positive Numbers
```

---

## Thought Process Growth

```text
Compare Index
↓
Realize Problem Is About Missing Positives
↓
Generate Positive Numbers
↓
Check Presence
↓
Count Missing Numbers
↓
Return kth Missing
```

---

## Personal Reflection

Even though I solved only one problem today because of travelling, I still learned something valuable:

```text
A productive day is not measured by
the number of questions solved.

It is measured by how much understanding
I gained from the questions I attempted.
```

This problem improved my observation skills and reinforced the idea that understanding the pattern is often more important than writing code immediately.

---

## Day 13 Final Thought

```text
Today was a low-volume day.

But I stayed consistent.

Consistency during busy days is what builds long-term progress.
```

SEEYA ON DAY 14🚀

# DAY 14 LEARNING LOG

**Date:** 30-07-2026

## Problems Solved

- LeetCode 206 — Reverse Linked List
- LeetCode 315 — Count of Smaller Numbers After Self (Brute Force Understanding)

---

## Additional Learning

Today I also spent time learning the basics of LinkedIn.

Topics explored:

- What LinkedIn is used for
- Professional networking basics
- Importance of building an online professional profile
- Understanding how recruiters and professionals use LinkedIn

Although this was not coding-related, it is an important skill for future internships, networking, and career growth.

---

## LeetCode 206 — Reverse Linked List

### Initial Challenge

This was my first serious Linked List problem.

My biggest confusion was:

```text
I was trying to think about Linked Lists like arrays.
```

I initially tried concepts such as:

```text
length
index access
head[i]
```

but quickly realized:

```text
Linked Lists do not support indexing.
```

---

## New Concepts Learned

### What is a Linked List?

A node contains:

```java
value
next
```

Example:

```text
1 -> 2 -> 3 -> null
```

Each node points to the next node.

---

### Linked List vs Array

Array:

```java
arr[2]
arr.length
```

Linked List:

```java
node.next
```

No direct indexing.

---

### Most Important Learning

The Three Pointer Pattern:

```java
prev
curr
next
```

Roles:

```text
prev = reversed portion

curr = current node

next = remaining nodes
```

---

### Reverse Linked List Pattern

```text
Save next
↓
Reverse current link
↓
Move prev
↓
Move curr
↓
Repeat
```

Code pattern:

```java
next = curr.next;
curr.next = prev;
prev = curr;
curr = next;
```

---

### Biggest Breakthrough

Understanding:

```java
curr.next = prev;
```

At first this line looked confusing.

Today I learned:

```text
This line changes the direction of the link.
```

Example:

Before:

```text
1 -> 2 -> 3
```

After:

```text
1 -> null
```

which is the actual reversal process.

---

## LeetCode 315 — Count of Smaller Numbers After Self

### Understanding Achieved

I successfully understood the problem and created a correct brute-force solution.

Approach:

```text
For every element
↓
Check every element on its right
↓
Count smaller values
↓
Store count
```

---

### Learning

I learned:

```text
A solution can be logically correct
but still fail due to efficiency.
```

My brute-force solution:

```text
Time Complexity:
O(n²)
```

Result:

```text
TLE (Time Limit Exceeded)
```

---

### Important Realization

Not every correct solution passes LeetCode.

Sometimes:

```text
Correct Logic
≠
Accepted Solution
```

because efficiency matters.

I learned that this problem typically requires advanced techniques such as:

```text
Merge Sort Counting
Fenwick Tree
Segment Tree
```

which I have not studied yet.

---

## Problem Solving Growth

Today I improved my ability to:

```text
Understand unfamiliar data structures
↓
Break down pointer movement
↓
Visualize memory references
↓
Distinguish between correctness and efficiency
```

---

## Personal Reflection

Today was not about solving many problems.

Instead, it was about learning a completely new topic:

```text
Linked Lists
```

I also explored LinkedIn basics to prepare for future professional growth.

Although I solved fewer questions than some previous days, I gained deeper understanding of:

```text
Data Structures
Professional Development
Problem Solving Mindset
```

---

## Day 14 Final Thought

```text
Today I learned that every problem
does not require more coding.

Sometimes the biggest progress comes from
understanding a new concept deeply.

Linked Lists felt confusing at first,
but by breaking the process into small steps,
I was able to understand one of the most important
pointer patterns in Data Structures.
```

SSEYA ON DAY 15...🚀

# DAY 15 LEARNING LOG

**Date:** 31-07-2026

## Problems Attempted

### LeetCode 21 — Merge Two Sorted Lists

### Initial Understanding

This was another Linked List problem after learning Reverse Linked List.

Initially, I was unsure how to create a completely new merged list while simultaneously traversing two existing linked lists.

The main challenge was understanding:

```text
How to build a new linked list while comparing nodes from two different lists.
```

---

### New Concepts Learned

#### Dummy Node Pattern

Today I learned the concept of a:

```java
ListNode dummy = new ListNode(-1);
```

A dummy node acts as a temporary starting point that makes linked list construction easier.

Instead of handling special cases for the first node, I can always attach new nodes after the dummy node.

---

#### Tail Pointer

I learned the purpose of:

```java
ListNode tail = dummy;
```

Role:

```text
tail always points to the last node
of the merged linked list.
```

Whenever a new node is attached:

```java
tail.next = node;
tail = tail.next;
```

---

### Pattern Learned

```text
Compare
↓
Attach Smaller Node
↓
Move Corresponding Pointer
↓
Move Tail
↓
Repeat
```

This is essentially the merge step of Merge Sort applied to Linked Lists.

---

### Biggest Learning

Today I realized that:

```text
Linked List problems are mostly about
moving references correctly.
```

The actual values are often less important than understanding where pointers are pointing.

---

## LeetCode 33 — Search in Rotated Sorted Array

### Initial Thought Process

At first, I tried approaching the problem using normal binary search.

My thinking was:

```java
nums[mid] < target
```

However, I quickly realized that the array is not completely sorted because of rotation.

Example:

```text
4 5 6 7 0 1 2
```

This breaks the assumptions of standard binary search.

---

### Key Observation

I learned that:

```text
Even if the entire array is not sorted,
at least one half is always sorted.
```

Example:

```text
4 5 6 7 | 0 1 2
```

The left half:

```text
4 5 6 7
```

is sorted.

---

### New Binary Search Pattern

Today I learned a modified binary search strategy:

```text
Find mid
↓
Identify which half is sorted
↓
Check if target lies inside that half
↓
Search there
↓
Otherwise search the other half
```

---

### Important Conditions Learned

Determine sorted half:

```java
nums[start] <= nums[mid]
```

Target inside left sorted half:

```java
target >= nums[start]
&&
target < nums[mid]
```

Target inside right sorted half:

```java
target > nums[mid]
&&
target <= nums[end]
```

---

### Biggest Learning

This problem taught me that:

```text
Binary Search is not limited to
completely sorted arrays.
```

By identifying sorted regions, binary search can still be applied efficiently.

---

## Concepts Strengthened Today

### Linked Lists

```text
Dummy Node
Tail Pointer
Merging Two Sorted Lists
Pointer Manipulation
```

### Binary Search

```text
Rotated Array Search
Sorted Half Detection
Range-Based Decisions
Modified Binary Search
```

---

## Personal Reflection

Today was a concept-heavy day.

I did not simply solve problems; instead, I learned two important patterns that frequently appear in interviews:

```text
Linked List Merge Pattern
+
Rotated Binary Search Pattern
```

Both problems required understanding the underlying idea rather than memorizing code.

I spent more time understanding why the solutions work instead of blindly implementing them.

---

## Day 15 Final Thought

```text
Today reinforced an important lesson:

Good programmers do not memorize solutions.
They recognize patterns.

The more patterns I learn,
the easier it becomes to solve unfamiliar problems.

Today I added two valuable patterns to my toolkit:

1. Merge Two Sorted Linked Lists
2. Search in Rotated Sorted Array
```

SEEYA ON DAY 16..🚀


# DAY 16 LEARNING LOG

**Date:** 01-08-2026

## Today's Reality

Today was a very busy day.

I was outside for work and did not get much time for coding practice.

Because of that, I intentionally decided not to force myself into solving multiple problems or difficult questions.

Instead, my goal was simple:

```text
Protect the streak.
Stay connected with coding.
Do at least one problem.
```

---

## Problem Solved

### LeetCode 1688 — Count of Matches in Tournament

### My Approach

This was a straightforward simulation problem.

The problem required understanding how matches are played in a tournament and tracking the total number of matches until a winner remains.

The logic itself was not difficult, but today the challenge was not the problem.

The challenge was:

```text
Finding time and energy to sit down and code.
```

---

## What I Learned

Even simple problems serve a purpose.

Today reminded me that:

```text
Consistency beats intensity.
```

Not every day will be:

```text
3 Problems
4 Problems
New Data Structures
Complex Algorithms
```

Some days will simply be:

```text
One small problem.
One small win.
Keep moving forward.
```

---

## Personal Reflection

Today I was tired and busy because of work outside.

For a moment I thought:

```text
Maybe I'll skip today.
```

But then I remembered that building discipline means showing up even on low-energy days.

So instead of breaking the streak, I chose a smaller goal:

```text
Solve one question.
Learn something.
Move on.
```

And I completed it.

---

## Important Lesson From Today

```text
Progress is not only measured by
the number of questions solved.

Sometimes progress means:

Showing up when you don't feel like it.
```

---

## Small Wins

✅ Maintained coding streak

✅ Solved one LeetCode problem despite a busy schedule

✅ Stayed consistent with learning

✅ Avoided the "I'll do it tomorrow" mindset

---

## Challenges Faced

```text
Limited time
Physical tiredness
Low energy after work
```

---

## Day 16 Final Thought

```text
Today was not about learning a new algorithm.

Today was about discipline.

Anyone can code when they have free time and motivation.

The real challenge is coding when you're tired,
busy, and tempted to skip.

Today I proved to myself that even a small step
is better than no step at all.
```

# DAY 17 LEARNING LOG

**Date:** 02-08-2026

---

## Today's Situation

Today was another very busy day.

I spent most of the day outside and did not have enough time for a long coding session. Because of this, I focused on maintaining my consistency rather than trying to solve multiple problems.

My primary goal was:

```text
Do not break the streak.
```

---

# Problems Worked On

## LeetCode 349 — Intersection of Two Arrays

### Initial Understanding

At first, I understood the problem as:

```text
Find all numbers that appear in both arrays.
Return only unique values.
```

I was able to identify the uniqueness requirement early.

---

### New Concept Learned: HashSet

Today was one of my first practical uses of HashSet.

I learned:

```java
HashSet<Integer> set = new HashSet<>();
```

Important functions:

```java
set.add()
set.contains()
set.size()
```

---

### Mistakes Made

#### Mistake 1

Initially I wrote:

```java
set.add(i);
```

Instead of:

```java
set.add(nums1[i]);
```

I accidentally stored indices instead of values.

---

#### Mistake 2

I wanted to directly:

```java
return set;
```

But learned:

```text
HashSet<Integer> ≠ int[]
```

The return type must exactly match the method signature.

---

#### Mistake 3

I did not initially think about how to return the answer.

I learned that after collecting values inside a HashSet, I must:

```text
Convert HashSet → int[]
```

before returning.

---

### Important Concepts Learned

#### HashSet Pattern

```text
Store first array in HashSet
↓
Traverse second array
↓
contains()
↓
Store common elements
↓
Convert to array
```

---

#### Collection vs Array

Today I learned:

```text
HashSet<Integer>
ArrayList<Integer>

are not the same as

int[]
```

Java requires exact return types.

---

#### Why HashSet?

Because it provides:

```text
Fast lookup
Unique elements
```

which perfectly matched the problem requirements.

---

## Bonus Problem

### LeetCode 877 — Stone Game

This was one of the funniest LeetCode experiences so far.

Initially I expected:

```text
DP
Recursion
Game Theory
```

But after understanding the constraints, I learned:

```text
Alex always wins.
```

Therefore the accepted solution is:

```java
return true;
```

---

### Lesson Learned

```text
Not every accepted solution requires
a complicated algorithm.

Sometimes understanding the constraints
is the entire solution.
```

This was a surprising and memorable learning moment.

---

# Challenges Faced Today

- Very limited time.
- Entire day spent outside.
- Physical tiredness.
- Low energy for coding.

---

# Personal Reflection

Today was not about solving many problems.

It was about maintaining consistency.

Even though I was busy, I still sat down and solved a problem instead of skipping the day completely.

I also learned my first practical HashSet pattern, which will be useful in many future problems.

---

# Important Learnings of Day 17

```text
HashSet basics

add()

contains()

Unique elements

Fast lookup

HashSet → Array conversion

Collection vs Array types

Understanding constraints can sometimes
be more important than coding complexity.
```

---

# Day 17 Final Thought

```text
Some days are for grinding.

Some days are for learning new concepts.

And some days are simply for protecting the streak.

Today I protected the streak,
learned HashSet,
and discovered that one accepted solution
can literally be:

return true;
```

🚀 Streak Continues.

OUT....DAY 18


# DAY 18 LEARNING LOG

**Date:** 03-08-2026

---

## Problems Worked On

### LeetCode 744 — Find Smallest Letter Greater Than Target

Today I solved a Binary Search problem that looked different from the standard "find target" questions.

Initially, my instinct was to search for the target itself, but while discussing the problem I realized that the actual goal was:

```text
Find the smallest element greater than the target.
```

This changed my thinking completely.

I learned that Binary Search is not only used for finding an exact value.

It can also be used to find:

- First valid position
- Smallest greater element
- Search insertion position
- First bad version

While solving the problem, I understood why:

```java
if(letters[mid] > target)
```

means we should move left after finding a possible answer.

I also learned the wrap-around trick:

```java
return letters[st % letters.length];
```

This was the most interesting part of the problem because it elegantly handled cases where no greater letter exists.

### Key Learning

```text
Binary Search is often about finding positions,
not finding exact values.
```

---

### LeetCode 509 — Fibonacci Number

Today I also solved Fibonacci using recursion.

My solution:

```java
if(n <= 1)
{
    return n;
}

return fib(n - 1) + fib(n - 2);
```

This was a very important recursion problem because it helped me understand how a large problem can be broken into smaller versions of itself.

I learned the importance of:

```text
Base Case
+
Recursive Calls
```

Without the base case, recursion would continue forever.

I also visualized how:

```text
fib(4)
```

creates multiple recursive calls underneath it.

This was one of my first proper recursion experiences.

### Key Learning

```text
Trust recursion.

Solve smaller versions of the same problem
and combine the answers.
```

---

## Concepts Learned Today

### Binary Search Patterns

```text
Search Target
Search Position
First Valid Element
Smallest Greater Element
```

---

### Wrap Around Logic

```java
st % length
```

can bring an index back to the beginning of an array.

Example:

```text
4 % 4 = 0
```

---

### Recursion Basics

```text
Base Case
↓
Recursive Call
↓
Smaller Subproblem
↓
Combine Result
```

---

## Mistakes / Corrections

### Binary Search

Initially I wanted to store an answer variable unnecessarily.

Later I understood that:

```java
st
```

already points to the answer position after Binary Search finishes.

This simplified the solution significantly.

---

### Recursion

At first, recursion feels like magic.

Today I focused on understanding:

```text
What is the smallest problem?
```

instead of trying to understand the entire recursion tree at once.

This made recursion much easier to follow.

---

## Overall Progress

Today I strengthened two important DSA areas:

```text
Binary Search
Recursion
```

Both of these topics appear repeatedly in LeetCode and interviews, so today's learning feels valuable for the future.

---

## Day 18 Summary

```text
Problems Solved:
✓ 744. Find Smallest Letter Greater Than Target
✓ 509. Fibonacci Number

Concepts Learned:
✓ Binary Search on answer position
✓ Wrap-around indexing
✓ Recursion basics
✓ Base case and recursive calls
```

🚀 Day 18 Complete.


OUT...DAY 19...🚀

# Day 19 Technical Learning Log

**Date:** 04-Aug-2026

## Problems Covered

### 50. Pow(x, n)

* Explored recursion-based power calculation.
* Learned Fast Power / Binary Exponentiation.
* Understood how to reduce exponent by half instead of reducing by one.
* Learned handling of:

  * Base case (`n == 0`)
  * Even exponents
  * Odd exponents
  * Negative exponents
* Discovered integer overflow issue with `Integer.MIN_VALUE`.
* Learned why accepted solutions use `long` instead of directly negating an `int`.

### 342. Power of Four

* Solved using recursion.
* Practiced recursive reduction:

  * `16 → 4 → 1`
  * `64 → 16 → 4 → 1`
* Strengthened understanding of:

  * Base case
  * Invalid case
  * Recursive call
  * Problem reduction

---

## Important Concepts Learned

### 1. Fast Power (Binary Exponentiation)

Normal approach:

```text
x × x × x × x × ...
```

Time Complexity:

```text
O(n)
```

Optimized approach:

```text
x^n = (x^(n/2)) × (x^(n/2))
```

Time Complexity:

```text
O(log n)
```

Core idea:

```text
Solve Half
Reuse Half
```

---

### 2. Even vs Odd Exponents

For even exponent:

```text
x^8 = x^4 × x^4
```

For odd exponent:

```text
x^5 = x × x^2 × x^2
```

Pattern:

```java
if(n % 2 == 0)
    half * half;
else
    x * half * half;
```

---

### 3. Negative Exponents

Mathematical identity:

```text
x^-n = 1/(x^n)
```

Examples:

```text
2^-2 = 1/4
2^-3 = 1/8
5^-1 = 1/5
```

---

### 4. Integer Overflow Edge Case

Problem:

```java
-intMinValue
```

Example:

```text
-2147483648
```

cannot become:

```text
2147483648
```

inside an `int`.

Solution:

```java
long N = n;
```

Convert to `long` before negating.

---

### 5. Recursive Reduction Pattern

Used in Power of Four:

```text
n
↓
n/4
↓
n/4
↓
...
```

General recursion structure:

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

## Java Concepts Reinforced

* Recursive function calls
* Return value propagation through recursion
* Modulus operator for divisibility checks
* Integer vs Long data types
* Importance of edge cases
* Method return flow

---

## Mistakes & Fixes

### Mistake

Tried writing:

```java
1/x^n
```

### Fix

Learned that:

```java
^
```

is XOR, not exponentiation.

---

### Mistake

Mixed negative-power logic and recursion logic together.

### Fix

Handle negative exponent separately before recursion.

---

### Mistake

Forgot that after:

```java
n = -n;
```

the condition:

```java
n < 0
```

can never be true.

### Fix

Understand execution flow step-by-step before adding conditions.

---

## Patterns Added To DSA Toolbox

### Pattern 1

```text
Fast Power
```

Reduce exponent by:

```text
n/2
```

---

### Pattern 2

```text
Recursive Reduction
```

Reduce problem repeatedly:

```text
n → n/4 → n/16 → ...
```

until base case.

---

## Today's Technical Takeaway

Today was my first deep exposure to Divide & Conquer recursion.

I learned that recursion is not only about calling the same function repeatedly; it is also about reducing a problem efficiently and reusing previously computed results to drastically improve performance.

OUT...DAY 20...🚀

# 📅 Day 20 — Technical Learning Log (08-05-2026)

## ✅ Problems Solved

* 383. Ransom Note
* 434. Number of Segments in a String
* 520. Detect Capital

---

# 📚 What I Learned Today

## 1. Character Frequency Array (Hashing)

Today I learned one of the most common string patterns on LeetCode.

Instead of checking whether a character exists, I learned to count **how many times** each character appears.

```java
int[] count = new int[26];
```

This array stores the frequency of every lowercase letter.

```
a → index 0
b → index 1
...
z → index 25
```

While traversing the magazine:

* Increase frequency.

While traversing the ransom note:

* Decrease frequency.

If any frequency becomes negative, it means I tried to use a character that wasn't available anymore.

This pattern is much faster than checking every character repeatedly.

---

## 2. Character Mapping

Today I finally understood why people write:

```java
ch - 'a'
```

Example:

```
'a' - 'a' = 0
'b' - 'a' = 1
'c' - 'a' = 2
...
'z' - 'a' = 25
```

This lets me directly map every lowercase letter to an array index.

---

## 3. Word Detection Pattern

The Number of Segments problem taught me something interesting.

I first thought about counting spaces.

Later I realized that spaces don't matter.

Instead, I should count **the beginning of every word**.

A new word starts only when:

* Current character is **not** a space.
* Previous character is a space **or** current index is 0.

This is a completely different way of thinking compared to simply counting separators.

---

## 4. Operator Precedence

Today I made a logical mistake because of operator precedence.

I wrote something similar to:

```java
A && B || C
```

But Java evaluates it as:

```java
(A && B) || C
```

My intended logic was:

```java
A && (B || C)
```

I learned that parentheses are extremely important whenever multiple logical operators are used.

---

## 5. ASCII Character Comparison

Instead of immediately using Java library methods, I practiced comparing characters manually.

Uppercase:

```java
ch >= 'A' && ch <= 'Z'
```

Lowercase:

```java
ch >= 'a' && ch <= 'z'
```

This helped me understand how characters are actually stored.

---

## 6. Breaking Problems into Cases

The Detect Capital problem taught me to stop coding immediately and first identify different cases.

Instead of checking every character randomly, I divided the problem into patterns:

* All uppercase
* All lowercase
* First uppercase, remaining lowercase

Breaking the problem into cases made the implementation much easier.

---

# 🧠 Biggest Realization

Today I realized that many string problems are actually **pattern recognition problems**, not coding problems.

Once I identify the correct pattern, the code becomes much simpler.

Instead of asking:

> "How do I code this?"

I started asking:

> "What pattern does this problem follow?"

That mindset is helping me solve problems more confidently.

---

# 🚀 Progress Reflection

Compared to my earlier days, I noticed a change in my thinking.

Earlier:

* I focused mainly on syntax.
* I often wanted to start coding immediately.

Today:

* I spent more time understanding the pattern first.
* I divided problems into logical cases.
* I understood *why* a solution works before implementing it.

I feel like my problem-solving approach is improving, even if I still make small logical mistakes.

Those mistakes are becoming easier to identify and fix.

---

**Day 20 Complete ✅**

SEE YA ON DAY 21....🚀

# 📅 Day 21 — Technical Learning Log (06-08-2026)

## ✅ Problems Solved

* 283. Move Zeroes
* 3345. Smallest Divisible Digit Product I

---

# 📚 What I Learned Today

## 1. Two Pointer Pattern

Today I learned one of the most important array patterns in DSA.

Initially, I thought **two pointers meant two nested loops**, but I realized that isn't true.

A two-pointer solution usually means:

* One pointer scans the array.
* Another pointer keeps track of the position where the next valid element should be placed.

For the **Move Zeroes** problem:

* `j` scans every element.
* `i` points to the position where the next non-zero element belongs.

This allows the problem to be solved in a single traversal.

---

## 2. Two Pointers ≠ Two Loops

One of the biggest misconceptions I had today was thinking:

```text
Two Pointers = Two Nested Loops
```

I learned that this is completely wrong.

Nested loops restart the inner loop every iteration, resulting in **O(n²)** complexity.

Two pointers simply mean two variables moving through the array together, usually resulting in **O(n)** complexity.

---

## 3. Swapping vs Copying

While solving Move Zeroes, I first wanted to solve it entirely using swapping.

Then I understood there are actually two valid approaches:

* Copy non-zero elements forward and fill the remaining positions with zero.
* Swap non-zero elements whenever needed using two pointers.

Both are valid, but the interview-preferred solution is the optimized two-pointer approach.

---

## 4. Digit Extraction Pattern

While solving **Smallest Divisible Digit Product I**, I practiced extracting digits from a number.

Pattern:

```java
digit = copy % 10;
copy /= 10;
```

This processes digits from right to left until the number becomes zero.

I also learned why a separate `copy` variable is important instead of modifying the original number.

---

## 5. Brute Force with Validation

The problem also taught me a simple brute-force strategy.

Instead of trying to directly calculate the answer:

* Start from `n`.
* Check if it satisfies the condition.
* If not, increment the number.
* Repeat until a valid answer is found.

Sometimes the simplest approach is perfectly acceptable.

---

## 6. Infinite Loop with Exit Condition

I used:

```java
while(true)
```

for the first time in a problem.

I learned that an infinite loop is acceptable when there is a guaranteed exit condition.

In this problem, the loop always exits using:

```java
return n;
```

once the correct answer is found.

---

## 7. Unreachable Statement

Today I encountered the Java compiler error:

```text
Unreachable statement
```

I understood why this happened.

Since my program always returns from inside an infinite loop, any statement written after the loop can never execute.

Example:

```java
while(true)
{
    return value;
}

return 1; // Unreachable
```

This helped me understand how Java analyzes program flow before execution.

---

# 🧠 Biggest Realization

Today I realized that **patterns are more important than syntax**.

Instead of thinking:

> "Which loop should I write?"

I started thinking:

> "What role should each pointer play?"

Once I assigned a responsibility to each pointer, writing the code became much easier.

---

# 🚀 Progress Reflection

Today's progress felt different.

Earlier, I would immediately think about nested loops whenever two indices were involved.

Today, I understood the actual philosophy behind the Two Pointer technique.

I also noticed that I now spend more time designing the algorithm before writing code.

That habit is making debugging much easier because most mistakes now happen during the planning stage instead of after writing the entire solution.

I feel much more confident solving array and digit-based problems than I did a week ago.

---

**Day 21 Complete ✅**

SEEYA ON DAY 22...🚀

# 📅 Day 22 — Learning Log (07-08-2026)

## ✅ Problems Solved

* 389. Find the Difference
* 476. Number Complement (Concept Learned)

---

# 📚 What I Learned Today

## 1. Frequency Array Pattern Becomes Reusable

Today's **Find the Difference** problem reinforced the frequency array pattern.

Instead of thinking about the problem differently, I recognized that it is almost identical to **Ransom Note**.

Approach:

* Count every character from the first string.
* Decrease the count while traversing the second string.
* As soon as any frequency becomes negative, that character is the extra character.

I realized that many string problems are actually the same pattern with a different story.

---

## 2. Return Immediately When the Answer Is Found

Instead of scanning the frequency array after both loops, I learned that I can immediately return the answer.

Example:

```java
count[index]--;

if(count[index] < 0)
    return t.charAt(j);
```

This makes the code cleaner and avoids unnecessary work.

---

## 3. Character ↔ Index Conversion

I revised one of the most important mappings in string problems.

Character to Index:

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

Index to Character:

```java
(char)(index + 'a')
```

---

## 4. Introduction to Bit Manipulation

Today I started learning Bit Manipulation from scratch.

I learned that every integer is stored internally as binary bits.

Example:

```text
5 = 101
6 = 110
8 = 1000
```

---

## 5. Bitwise Operators

I learned the meaning of the four basic bitwise operators.

### AND (&)

Both bits must be 1.

```text
1 & 1 = 1
1 & 0 = 0
0 & 1 = 0
0 & 0 = 0
```

---

### OR (|)

At least one bit must be 1.

```text
1 | 1 = 1
1 | 0 = 1
0 | 1 = 1
0 | 0 = 0
```

---

### XOR (^)

Different bits produce 1.

Same bits produce 0.

```text
1 ^ 1 = 0
0 ^ 0 = 0
1 ^ 0 = 1
0 ^ 1 = 1
```

Important properties:

```text
a ^ a = 0
a ^ 0 = a
```

---

### NOT (~)

Flips every bit.

```text
1 → 0
0 → 1
```

---

## 6. Why ~ Doesn't Directly Solve Number Complement

Initially I thought:

```java
~num
```

would directly give the complement.

I learned that Java stores integers using **32 bits**.

Example:

```text
5

00000000000000000000000000000101
```

Applying `~` flips every bit:

```text
11111111111111111111111111111010
```

The problem only wants to flip the meaningful bits.

This introduced me to the idea of a **mask**.

---

## 7. Mask Concept

To flip only the useful bits, we create a mask containing all 1s.

Example:

```text
Number

101

Mask

111
```

Then:

```text
101
111
---
010
```

using XOR.

---

## 8. Useful Built-in Java Method

I learned about:

```java
Integer.numberOfLeadingZeros(num)
```

which helps determine the number of significant bits in an integer.

Although I still want to understand the manual approach first, I now know this built-in method exists.

---

# 🧠 Biggest Takeaway

Today's biggest realization was that many LeetCode problems are not about learning new algorithms every time.

Instead, they are about recognizing an already known pattern.

The **Find the Difference** problem looked completely different from **Ransom Note**, but internally they used the exact same frequency array technique.

I also began learning Bit Manipulation, which initially looked complicated, but after understanding bits as binary switches, the operators started making much more sense.

Today felt like the beginning of a completely new topic in DSA.

---

**Day 22 Progress Complete ✅**
SEEYA ON DAY 23...🚀

# 📅 Day 23 — LeetCode Learning Log

**Date:** 08-08-2026

## ✅ Problems Solved

1. **121. Best Time to Buy and Sell Stock**
2. **392. Is Subsequence**

---

# 1️⃣ 121. Best Time to Buy and Sell Stock

### 🧠 Approach Learned

The main idea was to track:

* The **minimum price seen so far**
* The **maximum profit seen so far**

Instead of finding the overall minimum and maximum of the array, I learned that the order matters.

We must:

> Buy first → Sell later.

So while traversing from left to right, I keep the cheapest buying price available before the current day.

```java
int minPrice = prices[0];
int maxProfit = 0;
```

For every price:

```java
if (prices[i] < minPrice) {
    minPrice = prices[i];
}
```

Otherwise, calculate the possible profit:

```java
int tprofit = prices[i] - minPrice;
```

Then update the best profit:

```java
if (tprofit > maxProfit) {
    maxProfit = tprofit;
}
```

### 🔑 Important Pattern

**Minimum-so-far + Best-result-so-far**

This pattern can be useful in many array problems where we need the best result while maintaining an ordering constraint.

### ❌ Mistake I Made

Initially, I tried to track a `max` and `min` value and calculate:

```java
max - min
```

But that doesn't work because the maximum price could appear **before** the minimum price.

Example:

```text
[7, 6, 4, 3, 1]
```

The overall maximum is `7` and minimum is `1`, but buying at `1` and selling at `7` is impossible because `7` occurred first.

### 💡 Lesson

Don't just look at the values.

Look at their **order in the array**.

---

# 2️⃣ 392. Is Subsequence

### 🧠 Approach Learned

This problem introduced/reinforced the **Two Pointer Pattern**.

I used:

```java
int j = 0;
```

to track the current character required from `s`.

Then I used `i` to scan through `t`.

```java
for (int i = 0; i < t.length(); i++) {
    if (j < s.length() && s.charAt(j) == t.charAt(i)) {
        j++;
    }
}
```

Whenever the characters match:

```text
s[j] == t[i]
```

I move `j` forward.

The pointer `i` always continues through `t`.

### Example

```text
s = "abc"
t = "ahbgdc"
```

Process:

```text
a → match → j = 1
h → skip
b → match → j = 2
g → skip
d → skip
c → match → j = 3
```

Since:

```java
j == s.length()
```

the entire `s` was found.

Therefore:

```java
return j == s.length();
```

### 🔑 Important Understanding

`j` represents:

> **How many characters of `s` have been successfully matched.**

Therefore:

```text
j == s.length()
```

means:

> All characters of `s` were found in the correct order.

### ❌ Mistake I Made

Initially, I returned:

```java
return false;
```

at the end.

I learned that the final answer should depend on whether `j` reached the end of `s`.

I also learned why this check is important:

```java
j < s.length()
```

before:

```java
s.charAt(j)
```

Otherwise, once `j == s.length()`, accessing `s.charAt(j)` would cause an index error.

---

# 🧠 Important Concepts Learned Today

## 1. Minimum So Far

Track the smallest value encountered while traversing.

```java
if (current < min) {
    min = current;
}
```

---

## 2. Best Result So Far

Keep updating the best answer found so far.

```java
if (currentResult > best) {
    best = currentResult;
}
```

---

## 3. Order Matters

For problems involving:

* Buy → Sell
* Before → After
* Earlier → Later

we cannot simply find the minimum and maximum independently.

The traversal order matters.

---

## 4. Two Pointer Pattern

Use two variables/pointers to process data without unnecessary nested loops.

For subsequence:

```text
i → scans t
j → tracks s
```

---

## 5. Pointer Meaning

A pointer becomes much easier to use when I clearly define what it represents.

In today's problem:

```text
i = current position in t
j = number of characters matched from s
```

---

## 6. Character Comparison

I reinforced:

```java
s.charAt(j) == t.charAt(i)
```

and the importance of using:

```java
charAt()
```

when accessing individual characters of a Java `String`.

---

## 7. Boundary Checking

Before accessing:

```java
s.charAt(j)
```

make sure:

```java
j < s.length()
```

This prevents index-out-of-bounds errors.

---

# ⭐ Today's Biggest Takeaways

### Array Pattern

**Minimum so far + maximum result so far**

### String Pattern

**Two pointers + ordered matching**

### Problem-Solving Mindset

Today I learned that I should not immediately think about complicated algorithms.

First ask:

1. What exactly does each variable represent?
2. Does order matter?
3. Can I solve it with one traversal?
4. Is there a known pattern?
5. Can I maintain the answer while traversing?

---

# 📊 Day 23 Progress

| Problem                              | Pattern                         | Status |
| ------------------------------------ | ------------------------------- | ------ |
| 121. Best Time to Buy and Sell Stock | Minimum So Far + Maximum Profit | ✅      |
| 392. Is Subsequence                  | Two Pointers                    | ✅      |

### 🔥 Patterns Added to My DSA Toolkit

* Minimum So Far
* Maximum Result So Far
* Two Pointers
* Ordered Traversal
* Boundary Checking
* Character Matching
* Pattern Recognition

**Day 23 complete. 🚀**
SEEYA ON 24..🚀

# 📖 Day 24 — LeetCode Learning Log

**Date:** 09-08-2026

## ✅ Problems Solved

1. **599. Minimum Index Sum of Two Lists**
2. **1047. Remove All Adjacent Duplicates In String**

---

# 1️⃣ 599. Minimum Index Sum of Two Lists

### 🧠 My Initial Thought

I thought of using **two loops**:

```text
for every string in list1
    compare with every string in list2
```

When two strings match, calculate:

```text
indexSum = i + j
```

Then find the smallest index sum.

This was the correct basic approach.

### 🔑 Main Logic

I learned to maintain:

```java
int min = Integer.MAX_VALUE;
List<String> ans = new ArrayList<>();
```

When a common string is found:

```text
indexSum < min
        ↓
new minimum
        ↓
update min
clear old answers
add current string
```

If:

```text
indexSum == min
```

then the current string is another valid answer, so simply add it.

### Important Pattern

```text
Smaller → replace
Equal   → add
Larger  → ignore
```

### ❌ Mistake

Initially I used:

```java
int min = 0;
```

That doesn't work because index sums are non-negative.

For example:

```text
indexSum = 1
min = 0
```

`1 < 0` is false.

So I learned to initialize a minimum-search variable with:

```java
Integer.MAX_VALUE
```

### Java Concepts Reinforced

* `String.equals()`
* `List<String>`
* `ArrayList`
* `clear()`
* `add()`
* `toArray(new String[0])`
* Nested loops

---

# 2️⃣ 1047. Remove All Adjacent Duplicates In String

### 🧠 Initial Understanding

At first, the example:

```text
"abbaca"
```

was confusing.

I understood it step-by-step:

```text
abbaca
  ↓ remove bb
aaca
  ↓ remove aa
ca
```

The important thing is that after removing characters, previously separated characters can become adjacent.

### 🔑 Pattern Learned

This problem is a classic:

**Stack + Adjacent Cancellation**

For every character:

```text
current == stack top
        ↓
      POP

current != stack top
        ↓
      PUSH
```

### Example

For:

```text
"abbaca"
```

The stack changes like:

```text
a     → [a]
b     → [a,b]
b     → [a]       ← bb cancelled
a     → []        ← aa cancelled
c     → [c]
a     → [c,a]
```

Final result:

```text
"ca"
```

### 🧠 My Initial Coding Mistakes

I initially tried to use:

```java
s.empty()
s.top()
s.pop()
push()
```

directly on the `String`.

I learned that a `String` is not a stack.

For:

```java
Stack<Character> stack
```

the correct methods are:

```text
isEmpty() → check whether stack is empty
peek()    → look at top
pop()     → remove top
push()    → add to top
```

I also initially confused:

```java
stack.push(i)
```

with:

```java
stack.push(s.charAt(i))
```

Since the stack contains `Character`, I need to push the character, not the integer index.

### StringBuilder Learning

After processing the stack, I used:

```java
StringBuilder ans = new StringBuilder();
```

Then:

```java
ans.append(stack.get(j));
```

I learned the difference between:

```java
ans = something;
```

and:

```java
ans.append(something);
```

`=` replaces the value, while `append()` adds to the existing `StringBuilder`.

---

# 🧠 What I Learned Today

## 1. Minimum Search With Ties

When searching for a minimum and multiple answers are possible:

```text
New minimum → clear previous answers
Same minimum → keep previous answers + add current
```

---

## 2. Stack as a Cancellation Mechanism

A stack isn't only for brackets or traditional stack problems.

It can also be used when:

> The current element needs to interact with the most recently kept element.

For adjacent duplicates:

```text
same as top → cancel
different    → keep
```

---

## 3. `peek()` vs `pop()`

Important distinction:

```java
stack.peek()
```

looks at the top **without removing it**.

```java
stack.pop()
```

looks at and **removes** the top.

---

## 4. Generic Collections

Instead of:

```java
Stack stack = new Stack();
```

prefer:

```java
Stack<Character> stack = new Stack<>();
```

This tells Java exactly what type the stack contains.

---

## 5. `String.equals()`

For comparing Java strings:

```java
list1[i].equals(list2[j])
```

not:

```java
list1[i] == list2[j]
```

---

# ⭐ Patterns Added to My DSA Toolkit

```text
1. Minimum + Collect Ties
2. Nested Loop Comparison
3. Stack Pattern
4. Adjacent Cancellation
5. Push / Pop / Peek
6. StringBuilder
7. Generic Collections
8. Boundary / Type Awareness
```

# 📈 Day 24 Progress

| Problem                              | Main Pattern           | Status |
| ------------------------------------ | ---------------------- | ------ |
| 599. Minimum Index Sum of Two Lists  | Minimum + Collect Ties | ✅      |
| 1047. Remove All Adjacent Duplicates | Stack / Cancellation   | ✅      |

## 🔥 Biggest Lesson of Day 24

> **Don't just ask what code to write. First identify what data structure naturally represents the operation.**

For `1047`, repeatedly removing adjacent characters could look complicated with strings, but once I recognized **"compare with the last character I kept"**, the stack made the problem simple.

**Day 24 — Complete ✅**

SEEYA ON DAY 25...🧑‍🚀🚀

# 🧠 LeetCode Journey — Day 25 Learning Log

**Date:** 10-08-2026

## 🚀 Problem Solved

### 49. Group Anagrams

**Difficulty:** Medium
**Pattern:** HashMap + Sorting

---

# 💭 What I Learned

I realized that this problem is closely related to **Valid Anagram**.

In Valid Anagram, I check whether **two strings** contain the same characters.

In Group Anagrams, I have **many strings** and need to group the strings that have the same character pattern.

Example:

```text
eat → aet
tea → aet
ate → aet
```

Since all three produce the same sorted string, they belong to the same group.

---

# 🔑 Main Concept — Common Key

The most important idea I learned today is:

> **Create a common key for things that belong to the same group.**

For anagrams, the sorted string becomes the common key.

```text
eat → aet
tea → aet
ate → aet

tan → ant
nat → ant

bat → abt
```

Then the HashMap becomes:

```text
"aet" → ["eat", "tea", "ate"]
"ant" → ["tan", "nat"]
"abt" → ["bat"]
```

---

# 🧠 HashMap Pattern

I learned this general DSA pattern:

```text
Element
   ↓
Create a representative key
   ↓
HashMap[key]
   ↓
Group similar elements
```

This is more important than memorizing the exact solution.

---

# 💻 Important Java Concepts

### 1. `toCharArray()`

Converts a String into a character array.

```java
char[] chars = str.toCharArray();
```

Example:

```text
"eat"
 ↓
['e', 'a', 't']
```

---

### 2. `Arrays.sort()`

Sorts the characters:

```java
Arrays.sort(chars);
```

```text
['e','a','t']
      ↓
['a','e','t']
```

---

### 3. Convert Back to String

```java
String key = new String(chars);
```

So:

```text
['a','e','t']
      ↓
"aet"
```

---

### 4. `putIfAbsent()`

I learned this useful HashMap method:

```java
map.putIfAbsent(key, new ArrayList<>());
```

Meaning:

> If this key doesn't exist, create an empty list.

It does **not replace** the existing list if the key is already present.

---

### 5. `map.get(key).add(str)`

This gets the list belonging to the key and adds the original string.

```java
map.get(key).add(str);
```

Example:

```text
aet → ["eat"]

add "tea"

aet → ["eat", "tea"]
```

---

### 6. `map.values()`

After grouping, I only need the groups, not the keys.

```java
map.values()
```

gives:

```text
[
  ["eat","tea","ate"],
  ["tan","nat"],
  ["bat"]
]
```

---

# 🔥 Most Important DSA Pattern Today

## Grouping Using a Common Key

This is the main concept I should remember.

> **When multiple elements need to be grouped based on some common property, create a key representing that property and use a HashMap.**

For this problem:

```text
Common property = Anagram
Common key      = Sorted characters
Data structure  = HashMap
```

---

# 🔗 Connection With Previous Learning

### Valid Anagram

I already learned:

```text
Character frequencies
       ↓
Determine whether two strings are anagrams
```

### Group Anagrams

Today I extended that idea:

```text
Anagram property
       ↓
Create common key
       ↓
HashMap
       ↓
Group all anagrams
```

So this problem wasn't completely new — it was an **extension of a pattern I already knew**.

---

# 📌 Patterns Added To My DSA Toolkit

```text
1. HashMap Grouping
2. Common Key / Representative Key
3. Sorting as a Key
4. String → char[]
5. Arrays.sort()
6. putIfAbsent()
7. HashMap + ArrayList
8. map.values()
```

---

# ⭐ Biggest Lesson

> **Don't always compare every element with every other element. Sometimes you can transform each element into a common key and let a HashMap automatically group them.**

For anagrams:

```text
eat → aet ─┐
tea → aet ─┤
ate → aet ─┘
           ↓
       same group
```

## ✅ Day 25 — Problem 1 Complete

**49. Group Anagrams — SOLVED ✅**

**Main Pattern:** `HashMap + Common Key`

**Main Learning:**
**Transform → Create Key → Group using HashMap**


SEEYA ON DAY 26....🚀

# 🧠 LeetCode Learning Log — Day 26

**Date:** 11-08-2026

## Problems Solved

1. **2996 — Smallest Missing Integer Greater Than Sequential Prefix Sum**
2. **1475 — Final Prices With a Special Discount in a Shop**
3. **1512 — Number of Good Pairs**

---

## 🔥 Concepts Learned

### 1. Sequential Prefix

A prefix is sequential when every element is exactly `previous + 1`.

```text
[3, 4, 5, 1, 12]
 ↑   ↑   ↑
Sequential prefix
```

Important pattern:

```java
if (nums[i] == nums[i - 1] + 1)
```

Once this condition becomes false, the longest sequential prefix is finished.

---

### 2. HashSet for Fast Existence Checking

In **2996**, HashSet was used to answer:

> "Does this number exist in the array?"

Pattern:

```java
while (set.contains(sum)) {
    sum++;
}
```

Important idea:

**HashSet → fast membership/existence checking.**

---

### 3. Separating Logic Into Different Jobs

For 2996, we separated:

```text
Find sequential prefix
        ↓
Calculate sum
        ↓
Check whether sum exists
        ↓
Increase until missing
```

This is an important problem-solving habit: **don't mix unrelated logic into one loop.**

---

### 4. Nested Loops / Look-Ahead

In **1475**, we used:

```java
for (int j = i + 1; j < prices.length; j++)
```

This means:

> Look only at elements to the right of the current element.

Important pattern:

```text
Current element
      ↓
Search to the RIGHT
      ↓
Find first valid element
      ↓
Use it
      ↓
break
```

---

### 5. `break` After Finding the First Valid Answer

In 1475:

```java
if (prices[j] <= prices[i]) {
    ans[i] = prices[i] - prices[j];
    break;
}
```

The `break` is important because the problem asks for the **first** smaller/equal price.

---

### 6. Default Answer Initialization

Learned this useful pattern:

```java
ans[i] = prices[i];
```

Meaning:

> Assume there is no discount.

If a valid discount is found, update the answer.

This prevents the answer from staying at Java's default `0`.

---

### 7. Good Pairs

In **1512**, a good pair satisfies:

```text
nums[i] == nums[j]
i < j
```

Nested-loop pattern:

```java
for (int i = 0; i < nums.length; i++) {
    for (int j = i + 1; j < nums.length; j++) {
        if (nums[i] == nums[j]) {
            count++;
        }
    }
}
```

Important insight:

`j = i + 1` automatically guarantees:

```text
i < j
```

---

### 8. Frequency Counting Pattern

The bigger concept behind **1512** is:

```text
number → frequency seen so far
```

When a number appears again:

```text
new pairs = previous frequency
```

Example:

```text
1 → seen 0 times → +0
1 → seen 1 time  → +1
1 → seen 2 times → +2
1 → seen 3 times → +3
```

This leads to the important HashMap pattern:

```text
count += frequency
frequency++
```

---

# 🎯 Most Important Patterns From Day 26

### Pattern 1 — Sequential Prefix

```text
nums[i] == nums[i-1] + 1
```

### Pattern 2 — HashSet Membership

```text
set.contains(value)
```

### Pattern 3 — Search to the Right

```text
j = i + 1
```

### Pattern 4 — First Valid Element

```text
find → use → break
```

### Pattern 5 — Default + Update

```text
answer = original value
        ↓
update only if condition is satisfied
```

### Pattern 6 — Frequency → Pair Counting

```text
new pairs = previous frequency
```

---

## 💡 Day 26 Key Takeaway

> **Don't just learn the solution. Learn the pattern behind the solution.**

Today you worked with **sequential patterns, HashSet, nested loops, look-ahead searching, `break`, default initialization, and frequency counting**.

**Day 26 — Complete ✅**

SEEYA ON DAY 27....🚀

# 📖 DSA Journey Documentation --- Day 27

**Date:** 12-08-2026

## Problems Worked On

### 2958. Length of Longest Subarray With at Most K Frequency

**Difficulty:** Medium\
**Pattern:** HashMap + Sliding Window\
**Status:** ⏸️ Paused

------------------------------------------------------------------------

## 🧠 Problem Understanding

The problem gives an integer array `nums` and an integer `k`.

We need to find the **longest contiguous subarray** where every element
appears at most `k` times.

For example:

``` text
nums = [1,2,3,1,2,3,1,2]
k = 2
```

The longest valid subarray is:

``` text
[1,2,3,1,2,3]
```

because each number appears exactly two times.

------------------------------------------------------------------------

## 💭 My Initial Thinking

I first thought this was mainly a **HashMap / HashSet** problem because
the problem talks about frequency.

I tried a brute-force approach:

``` text
Choose starting index i
        ↓
Traverse using j
        ↓
Count frequency
        ↓
If frequency > k → break
        ↓
Calculate length
        ↓
Update maximum
```

The approach made sense logically, but it resulted in **TLE**.

------------------------------------------------------------------------

## ❌ Why I Got TLE

The nested loops repeatedly check many of the same elements.

The approximate complexity is:

``` text
O(n²)
```

For a large input, this becomes too slow.

------------------------------------------------------------------------

## 🔑 New Concept Introduced --- Sliding Window

The optimized pattern for this problem is:

``` text
HashMap + Sliding Window
```

Basic idea:

``` text
right → expand the window
left  → shrink the window when invalid
```

The HashMap stores:

``` text
element → frequency
```

When an element's frequency becomes greater than `k`, the current window
is invalid, so we move `left` forward and decrease the frequency of
removed elements.

I have **paused this problem** because I want to understand Sliding
Window properly instead of memorizing the solution.

------------------------------------------------------------------------

# 1672. Richest Customer Wealth

**Difficulty:** Easy\
**Pattern:** 2D Array Traversal + Maximum Value\
**Status:** ✅ Solved

------------------------------------------------------------------------

## 🧠 Problem Understanding

The problem gives a 2D array where:

``` java
accounts[i][j]
```

represents the money customer `i` has in bank `j`.

We need to calculate the total wealth of every customer and return the
maximum.

Example:

``` text
accounts = [
    [1,2,3],
    [3,2,1]
]
```

First customer:

``` text
1 + 2 + 3 = 6
```

Second customer:

``` text
3 + 2 + 1 = 6
```

Answer:

``` text
6
```

------------------------------------------------------------------------

## 💭 My Initial Thinking

I understood that this was a **2D array traversal** problem, so I needed
nested loops.

However, I initially confused:

``` java
accounts.length
```

with:

``` java
accounts[i].length
```

This was the same type of mistake I have made before with 2D arrays.

------------------------------------------------------------------------

## 🔑 Important 2D Array Concept

``` java
accounts.length
```

means:

``` text
Number of rows
```

while:

``` java
accounts[i].length
```

means:

``` text
Number of elements in row i
```

Therefore:

``` java
for (int i = 0; i < accounts.length; i++) {
    for (int j = 0; j < accounts[i].length; j++) {
        sum += accounts[i][j];
    }
}
```

------------------------------------------------------------------------

## ⚠️ Recurring Mistake --- Row vs Element

I noticed that I repeatedly confuse:

``` java
accounts[i]
```

and:

``` java
accounts[i][j]
```

Remember:

``` text
accounts[i]       → entire row
accounts[i][j]    → one element
```

And:

``` text
i → row
j → column
```

This is now a **recurring DSA mistake** that I should actively check
whenever I solve a 2D array problem.

------------------------------------------------------------------------

## 🔥 Maximum Value Pattern

After calculating each customer's wealth:

``` java
if (sum > max) {
    max = sum;
}
```

General pattern:

``` text
Calculate current value
        ↓
Compare with max
        ↓
Update max if current value is larger
```

This is the **Maximum Value Pattern**.

------------------------------------------------------------------------

# 1572. Matrix Diagonal Sum

**Difficulty:** Easy\
**Pattern:** 2D Array + Diagonal Indexing\
**Status:** ✅ Solved

------------------------------------------------------------------------

## 🧠 Problem Understanding

The problem gives a square matrix and asks for the sum of both
diagonals.

Example:

``` text
[1 2 3]
[4 5 6]
[7 8 9]
```

Main diagonal:

``` text
1 + 5 + 9 = 15
```

Secondary diagonal:

``` text
3 + 5 + 7 = 15
```

The center `5` is counted twice, so it must be subtracted once.

Final answer:

``` text
25
```

------------------------------------------------------------------------

## 🔑 Main Diagonal

The main diagonal follows:

``` java
mat[i][i]
```

Example:

``` text
mat[0][0] → 1
mat[1][1] → 5
mat[2][2] → 9
```

Pattern:

``` text
[i][i]
```

------------------------------------------------------------------------

## 🔑 Secondary Diagonal

The secondary diagonal follows:

``` java
mat[i][n - 1 - i]
```

Example:

``` text
mat[0][2] → 3
mat[1][1] → 5
mat[2][0] → 7
```

Pattern:

``` text
[i][n - 1 - i]
```

------------------------------------------------------------------------

## ⚠️ Center Element

If the matrix size is odd, the center element belongs to both diagonals.

Therefore:

``` java
if (n % 2 == 1) {
    sum -= mat[n / 2][n / 2];
}
```

This prevents counting the center twice.

------------------------------------------------------------------------

# 📚 Java / DSA Concepts Learned Today

-   2D array traversal
-   Nested loops
-   Rows and columns
-   `array[i]` vs `array[i][j]`
-   `accounts.length`
-   `accounts[i].length`
-   Row sum
-   Maximum value pattern
-   Main diagonal indexing
-   Secondary diagonal indexing
-   Handling duplicate center elements
-   HashMap frequency
-   Subarray concept
-   Sliding Window introduction
-   Recognizing TLE
-   Understanding `O(n²)` brute force

------------------------------------------------------------------------

# 🔥 Important Concepts --- Day 27

## 1. 2D Array Traversal

``` java
array[i][j]
```

``` text
i → row
j → column
```

## 2. Row vs Element

``` java
array[i]       // entire row
array[i][j]    // individual element
```

## 3. Correct Inner Loop

``` java
for (int j = 0; j < array[i].length; j++)
```

The inner loop should use the current row's length when traversing its
columns.

## 4. Row Sum

``` java
sum += accounts[i][j];
```

## 5. Maximum Value Pattern

``` java
if (sum > max) {
    max = sum;
}
```

## 6. Main Diagonal

``` java
mat[i][i]
```

## 7. Secondary Diagonal

``` java
mat[i][n - 1 - i]
```

## 8. Frequency Pattern

``` text
element → frequency
```

## 9. Sliding Window

``` text
right → expand
left  → shrink
```

## 10. TLE Recognition

A brute-force nested-loop solution can become:

``` text
O(n²)
```

and may cause TLE when the input size is large.

------------------------------------------------------------------------

# 🔗 Connection With Previous Problems

### HashMap

I previously used HashMap in problems such as:

``` text
49. Group Anagrams
```

Today I recognized that frequency-based problems can also use HashMap:

``` text
element → frequency
```

This is useful for problems where we need to know how many times an
element appears.

### Maximum Value Pattern

The same pattern appears again:

``` java
if (value > max) {
    max = value;
}
```

Used in:

``` text
1672. Richest Customer Wealth
```

### 2D Arrays

Today I practiced two different types of 2D array problems:

``` text
1672 → row traversal + row sum
1572 → diagonal indexing
```

This helped me understand that correct indexing is one of the most
important parts of working with matrices.

------------------------------------------------------------------------

# 📝 Recurring Mistake To Remember

## 2D Array Row vs Element Confusion

I repeatedly confuse:

``` java
array[i]
```

with:

``` java
array[i][j]
```

Remember:

``` text
array[i]
    ↓
entire row

array[i][j]
    ↓
one element
```

And:

``` text
i → row
j → column
```

Before writing a 2D array loop, I should first identify:

``` text
How many rows?
How many columns in the current row?
What does i represent?
What does j represent?
```

------------------------------------------------------------------------

# 📈 Growth / Improvement

Today I strengthened my understanding of **2D arrays, nested loops,
matrix indexing, row sums, and maximum-value patterns**.

I also started recognizing when a brute-force solution is too slow.

The 2958 problem was difficult because it introduced **Sliding Window**.
I understood the reason my nested-loop approach got TLE, but I decided
to pause the problem and learn the pattern properly before solving it.

Most importantly, I identified a recurring mistake:

> I sometimes confuse `array[i]` (the complete row) with `array[i][j]`
> (a single element).

I need to keep checking this whenever I work with 2D arrays.

------------------------------------------------------------------------

# 🎯 What I Should Remember

``` text
2D Array:
array[i][j]

i → row
j → column

Entire row:
array[i]

Individual element:
array[i][j]

Number of rows:
array.length

Number of columns:
array[i].length

Main diagonal:
mat[i][i]

Secondary diagonal:
mat[i][n - 1 - i]

Maximum pattern:
if (value > max)
    max = value;

Frequency:
element → frequency

Sliding Window:
right → expand
left → shrink
```

------------------------------------------------------------------------

# ✅ Day 27 Status

**Problems Solved:** 2\
**Problem Paused:** 1\
**Problems Worked On:** 2958, 1672, 1572\
**Main Topics:** 2D Arrays, HashMap, Frequency, Maximum Value, Matrix
Diagonals, Sliding Window

## 🚀 Day 27 --- Completed

Today I solved two Easy problems and strengthened my understanding of
**2D array traversal, row sums, maximum-value patterns, and matrix
diagonal indexing**.

I also attempted a Medium Sliding Window problem and understood why my
brute-force approach resulted in TLE.

I identified a recurring mistake in my DSA journey:

> **`array[i]` is a row, while `array[i][j]` is an individual element.**

This is something I need to remember in every future 2D array problem.

# 👋 See You on Day 28!

# 📖 DSA Journey Documentation — Day 28

**Date:** 13-08-2026

## Problems Solved

### 1. 1486. XOR Operation in an Array

**Difficulty:** Easy  
**Pattern:** XOR + Array Traversal  
**Status:** ✅ Solved

---

## 🧠 Problem Understanding

The problem defines an array using:

```text
nums[i] = start + 2 * i
```

So instead of creating the complete array first, I can directly generate each value while traversing.

For example:

```text
n = 5
start = 0
```

The generated values are:

```text
0, 2, 4, 6, 8
```

The task is to XOR all of them.

---

## 💭 My Approach

I used a variable:

```java
int ans = 0;
```

Then for every `i`:

```java
ans = ans ^ (start + 2 * i);
```

This avoids creating a separate array.

---

## 🔑 XOR Concepts Reinforced

Important XOR properties:

```text
x ^ x = 0
x ^ 0 = x
```

XOR is useful for problems where values can cancel each other.

---

# 2. 136. Single Number

**Difficulty:** Easy  
**Pattern:** XOR  
**Status:** ✅ Solved

---

## 🧠 Problem Understanding

The problem gives an array where every number appears twice except one number.

The goal is to find the number that appears only once.

For example:

```text
[4,1,2,1,2]
```

The answer is:

```text
4
```

---

## 💭 My Approach

I used XOR again:

```java
int ans = 0;

for (int num : nums) {
    ans = ans ^ num;
}
```

Because equal numbers cancel each other:

```text
1 ^ 1 = 0
2 ^ 2 = 0
```

So:

```text
0 ^ 4 ^ 1 ^ 2 ^ 1 ^ 2
```

becomes:

```text
4
```

---

## 🔥 Important XOR Pattern

```text
0 ^ duplicate ^ duplicate ^ unique
```

All duplicates cancel and the unique number remains.

---

# 3. 1859. Sorting the Sentence

**Difficulty:** Easy  
**Pattern:** String Manipulation + Index Placement  
**Status:** ✅ Solved

---

## 🧠 Problem Understanding

Each word contains its original position at the end.

Example:

```text
"is2 sentence4 This1 a3"
```

The numbers tell us where each word belongs:

```text
is2       → position 2
sentence4 → position 4
This1     → position 1
a3        → position 3
```

So the original sentence is:

```text
"This is a sentence"
```

---

## 💭 My Approach

I first understood the problem in Java, then tried the solution in Python.

The Python solution was:

```python
words = s.split()
ans = [""] * len(words)

for word in words:
    pos = int(word[-1])
    ans[pos - 1] = word[:-1]

return " ".join(ans)
```

---

## 🔑 Python Concepts Learned

### `split()`

```python
s.split()
```

Turns a sentence into a list of words.

```text
"is2 sentence4 This1 a3"
        ↓
["is2", "sentence4", "This1", "a3"]
```

### Negative Indexing

```python
word[-1]
```

gets the last character.

For:

```text
"This1"
```

it gives:

```text
"1"
```

### `int()`

```python
int(word[-1])
```

converts the number into an integer.

### Slicing

```python
word[:-1]
```

removes the final character.

```text
"This1" → "This"
```

### `join()`

```python
" ".join(ans)
```

combines the words with spaces.

---

## 🔗 Important Java/Python Connection

The algorithm is the same even when the language changes:

```text
Split
  ↓
Read position
  ↓
Place word
  ↓
Remove position number
  ↓
Join
```

Only the syntax changes.

This helped me realize that **DSA logic is more important than programming-language syntax**.

---

# 4. 1925. Count Square Sum Triples

**Difficulty:** Easy  
**Pattern:** Brute Force + Triplet Search  
**Status:** ✅ Solved

---

## 🧠 Problem Understanding

A square triple is a triplet:

```text
(a, b, c)
```

such that:

```text
a² + b² = c²
```

and:

```text
1 <= a,b,c <= n
```

For:

```text
n = 5
```

the valid triples are:

```text
(3,4,5)
(4,3,5)
```

Both count separately because `a` and `b` are ordered positions in the triplet.

---

## 💭 My Initial Thinking

At first, I was unsure how to decide what values should be used for `a`, `b`, and `c`.

I realized I don't need to guess special values.

I can simply try every possible value from `1` to `n`.

So:

```text
a → 1 to n
b → 1 to n
c → 1 to n
```

Then check:

```text
a² + b² == c²
```

---

## 💻 Final Approach

```java
int count = 0;

for (int i = 1; i <= n; i++) {
    for (int j = 1; j <= n; j++) {
        for (int k = 1; k <= n; k++) {

            if (i * i + j * j == k * k) {
                count++;
            }
        }
    }
}

return count;
```

Here:

```text
i → a
j → b
k → c
```

---

## 🔥 Important Concept

This is a classic **Brute Force Triplet Search**:

```text
Choose a
   ↓
Choose b
   ↓
Choose c
   ↓
Check condition
   ↓
Count if valid
```

Because `n` is small, the `O(n³)` solution is acceptable.

---

# 📚 Java / DSA Concepts Learned Today

- XOR operator
- XOR cancellation
- XOR accumulation
- Bitwise operations
- Enhanced `for` loop
- Formula-based array generation
- String splitting
- String indexing
- Negative indexing in Python
- Python slicing
- Python `join()`
- Brute force
- Triplet search
- Nested loops
- Condition-based counting
- Understanding when `O(n³)` is acceptable

---

# 🔥 Important Patterns From Day 28

### Pattern 1 — XOR Accumulation

```java
ans ^= value;
```

Useful when duplicate values should cancel.

### Pattern 2 — XOR Duplicate Cancellation

```text
x ^ x = 0
x ^ 0 = x
```

### Pattern 3 — Formula-Based Generation

Instead of creating an array:

```text
value = start + 2 * i
```

generate the value directly during the loop.

### Pattern 4 — Position-Based String Reconstruction

```text
word
 ↓
last character = position
 ↓
place word at position - 1
```

### Pattern 5 — Brute Force Triplets

```text
for a
    for b
        for c
            check condition
```

---

# 🔗 Connection With Previous Learning

### XOR

Earlier I learned what XOR means in Java.

Today I actually applied it to:

```text
1486. XOR Operation in an Array
136. Single Number
```

This helped me move from understanding the operator to recognizing when it is useful.

### String Handling

The `1859` problem reinforced the string concepts I have been learning in Java, while also giving me practice with Python string functions.

### Brute Force

The `1925` problem reinforced that brute force is not always bad.

The key is:

> **If the input constraints are small enough, a simple brute-force solution can be the best choice.**

---

# 📈 Growth / Improvement

Today I worked with several different patterns instead of focusing on only one data structure.

I practiced:

```text
XOR
Strings
Python syntax
Nested loops
Brute force
Formula-based generation
```

I also learned that the same DSA idea can be expressed in different programming languages.

The biggest improvement today was recognizing that I do not always need a complicated data structure. Sometimes the cleanest solution is simply:

```text
Generate
Traverse
Check
Count
```

---

# 🎯 What I Should Remember

```text
XOR:
x ^ x = 0
x ^ 0 = x

Single Number:
ans ^= num

XOR Operation:
ans ^= (start + 2 * i)

String Position:
word[-1] → position
word[:-1] → remove position

Brute Force Triplets:
a = 1..n
b = 1..n
c = 1..n

Check:
a² + b² = c²
```

---

# ✅ Day 28 Status

**Problems Solved:** 4

**Problems:**
- 1486. XOR Operation in an Array ✅
- 136. Single Number ✅
- 1859. Sorting the Sentence ✅
- 1925. Count Square Sum Triples ✅

**Main Topics:** XOR, Strings, Python Syntax, Brute Force, Nested Loops, Triplet Search

## 🚀 Day 28 — Completed

Today I strengthened my understanding of **XOR**, learned how to use it to cancel duplicate values, practiced **Python string operations**, and reinforced the idea of using **simple brute force when the constraints are small**.

The most important takeaway is:

> **First understand the pattern and constraints. Then choose the simplest solution that fits.**

# 👋 See You on Day 29!

# 📖 LeetCode Learning Log — Day 29

**Date:** 14-08-2026

## Problems Solved

### 1. 3090. Maximum Length Substring With Two Occurrences

**Difficulty:** Easy  
**Pattern:** Sliding Window + Frequency Array  
**Status:** ✅ Solved

---

## 🧠 Problem Understanding

The problem asks for the longest **substring** where every character appears at most two times.

For example:

```text
s = "aaaa"
```

Valid:

```text
"a"   ✅
"aa"  ✅
```

Invalid:

```text
"aaa"  ❌
"aaaa" ❌
```

because the character `a` appears more than two times.

---

## 💭 My Initial Thinking

At first, I was confused by the problem statement and wasn't sure what exactly "at most two occurrences" meant.

After breaking it down, I understood that I need to find the longest **continuous part of the string** where no character appears more than twice.

I initially wondered whether this was something like Binary Search, but then I understood that it is a **Sliding Window** problem.

---

## 🔑 Main Idea I Learned

The window has two ends:

```text
left  → starting position
right → ending position
```

The idea is:

```text
right → expand the substring
left  → shrink the substring when it becomes invalid
```

A frequency array keeps track of how many times each character appears inside the current window.

---

## ❌ My Coding Mistakes

I initially used:

```java
s.countAt(i)
```

but Java uses:

```java
s.charAt(i)
```

I also tried checking:

```java
if (freq > 2)
```

but `freq` is an entire array. I needed to check the frequency of the current character.

Another mistake was moving `left` without actually removing the character from the frequency array.

I learned that when `left` moves, the element leaving the window must also have its frequency decreased.

---

## ✅ Final Thinking

The flow became:

```text
Add current character
        ↓
Frequency becomes > 2?
        ↓
YES → remove characters from the left
        ↓
Continue until window is valid
        ↓
Calculate current window length
        ↓
Update maximum
```

This was the first time I properly understood the sliding-window process.

---

## 📈 Improvement

This was especially important because I had previously paused **2958. Length of Longest Subarray With at Most K Frequency** because I didn't understand Sliding Window.

Working through `3090` helped me understand the same idea in a simpler form using a string.

The main breakthrough was understanding:

> **Moving `left` means removing an element from the current window, not just changing the pointer.**

---

# 2. 2185. Counting Words With a Given Prefix

**Difficulty:** Easy  
**Pattern:** String Traversal + Prefix Checking  
**Status:** ✅ Solved

---

## 🧠 Problem Understanding

The problem asks how many words start with a given prefix.

For example:

```text
words = ["pay","attention","practice","attend"]
pref = "at"
```

Check:

```text
pay        → ❌
attention  → ✅
practice   → ❌
attend     → ✅
```

Answer:

```text
2
```

---

## 💭 My Initial Thinking

I understood that I only needed to check every word and count the ones that begin with the given prefix.

I initially made a small mistake by using:

```java
words.startsWith(pref)
```

But `words` is an array, not a String.

The correct object is the individual element:

```java
words[i].startsWith(pref)
```

---

## 🔑 Important Learning

I reinforced the difference between:

```text
words      → entire String array
words[i]   → one String
```

This is similar to the 2D-array row-vs-element mistake I have been tracking.

The method I learned here is:

```java
startsWith()
```

which checks only the beginning of a string.

---

## ✅ Final Logic

```text
For every word
      ↓
Check startsWith(pref)
      ↓
YES → count++
NO  → ignore
```

---

# 3. 1967. Number of Strings That Appear as Substrings in Word

**Difficulty:** Easy  
**Pattern:** String Traversal + Substring Checking  
**Status:** ✅ Solved

---

## 🧠 Problem Understanding

The problem gives:

```text
patterns
word
```

For every pattern, I need to check whether that pattern appears **anywhere continuously** inside `word`.

Example:

```text
patterns = ["a","abc","bc","d"]
word = "abc"
```

Results:

```text
"a"   → ✅
"abc" → ✅
"bc"  → ✅
"d"   → ❌
```

Answer:

```text
3
```

---

## 💭 My Initial Thinking

I first wanted to make sure I understood the difference between a **prefix** and a **substring**.

A prefix must be at the beginning:

```text
"abcdef"
"abc" ✅ prefix
"cde" ❌ prefix
```

A substring can appear anywhere as long as it is continuous:

```text
"abcdef"
"abc" ✅
"cde" ✅
"def" ✅
"ace" ❌
```

Once I understood this difference, the problem became very straightforward.

---

## 🔑 Java Method Learned

The method I used is:

```java
word.contains(patterns[i])
```

`contains()` checks whether the given string appears anywhere inside another string.

This is different from:

```java
startsWith()
```

because:

```text
startsWith() → beginning only
contains()   → anywhere
```

---

## ✅ Final Logic

```text
For every pattern
       ↓
Check whether word contains it
       ↓
YES → count++
NO  → ignore
```

---

# 📚 Java / DSA Concepts Learned Today

- Sliding Window
- Two pointers
- Frequency array
- Character frequency tracking
- `charAt()`
- `startsWith()`
- `contains()`
- String vs String array
- Prefix vs substring
- Contiguous substring
- Maximum length tracking
- Expanding and shrinking a window

---

# 🔥 Important Patterns From Day 29

### Pattern 1 — Sliding Window

```text
right → expand
left  → shrink when invalid
```

### Pattern 2 — Frequency Tracking

```text
character → frequency
```

### Pattern 3 — Prefix Checking

```java
word.startsWith(pref)
```

### Pattern 4 — Substring Checking

```java
word.contains(pattern)
```

### Pattern 5 — Count Valid Matches

```text
condition true → count++
```

---

# 🔗 Connection With Previous Learning

The biggest connection today was between:

```text
2958 → array + frequency limit
3090 → string + frequency limit
```

I had struggled with `2958` because Sliding Window was unfamiliar.

After solving `3090`, the pattern became much clearer because the problem was simpler and used a frequency array instead of a more complicated setup.

I also connected today's string problems:

```text
2185 → startsWith()
1967 → contains()
```

This helped me clearly understand the difference between a **prefix** and a **substring**.

---

# 📈 Growth / Improvement

Today I improved in two important areas.

First, I finally started understanding **Sliding Window** instead of just seeing it as a pattern to memorize.

Second, I became more comfortable identifying the exact Java operation needed for a string problem.

Instead of manually checking every character, I can recognize when Java already provides a useful method:

```text
startsWith()
contains()
```

This makes my solutions simpler and also helps me focus more on the actual problem logic.

---

# 🎯 What I Should Remember

```text
Sliding Window:
right → expand
left  → shrink

Frequency:
track how many times each character appears

Prefix:
startsWith()

Substring:
contains()

Array element:
words[i]

String:
words[i] is one String
```

## ⭐ Biggest Lesson of Day 29

> **Understand exactly what the problem is asking before choosing the code.**

A small difference in wording can completely change the method:

```text
prefix    → startsWith()
substring → contains()
```

And for frequency-limited substring problems:

```text
expand → check frequency → shrink → update answer
```

# ✅ Day 29 Status

**Problems Solved:** 3

**Problems:**

- `3090. Maximum Length Substring With Two Occurrences` ✅
- `2185. Counting Words With a Given Prefix` ✅
- `1967. Number of Strings That Appear as Substrings in Word` ✅

**Main Topics:** Sliding Window, Frequency Arrays, Strings, Prefixes, Substrings

## 🚀 Day 29 — Completed

Today I finally made progress on the **Sliding Window** pattern that I had struggled with earlier, and I also became more confident with Java String methods.

# 👋 See You on Day 30!

# 📖 LeetCode Learning Log — Day 30

**Date:** 15-08-2026

## Problems Solved

### 1. 724. Find Pivot Index

**Difficulty:** Easy  
**Pattern:** Total Sum + Running Left Sum  
**Status:** ✅ Solved

---

## 🧠 Problem Understanding

The problem asks for an index where the sum of all elements strictly to the left is equal to the sum of all elements strictly to the right.

For example:

```text
nums = [1,7,3,6,5,6]
```

At index `3`:

```text
Left  = 1 + 7 + 3 = 11
Right = 5 + 6 = 11
```

So the pivot index is `3`.

---

## 💭 My Initial Thinking

At first, I thought about creating two arrays:

```text
leftSum[]
rightSum[]
```

and then comparing them at every index.

That approach would work, but I realized I could avoid storing both arrays.

---

## 🔑 Main Idea I Learned

First calculate the total sum of the entire array.

Then maintain a running `leftSum`.

For the current index:

```text
total = leftSum + current element + rightSum
```

Therefore:

```text
rightSum = total - leftSum - nums[i]
```

Then compare:

```text
leftSum == rightSum
```

If they are equal, return the index.

---

## 💡 Important Insight

The total sum is not the answer itself.

It is used to calculate the right-side sum efficiently without traversing the right side again.

Instead of calculating both sides repeatedly, I can use:

```text
total sum
   ↓
left sum
   ↓
calculate right sum
```

---

## 💻 Final Approach

```java
int total = 0;

for (int num : nums) {
    total += num;
}

int leftSum = 0;

for (int i = 0; i < nums.length; i++) {
    int rightSum = total - leftSum - nums[i];

    if (leftSum == rightSum) {
        return i;
    }

    leftSum += nums[i];
}

return -1;
```

---

## 📊 Complexity

```text
Time: O(n)
Space: O(1)
```

---

# 2. 1991. Find the Middle Index in Array

**Difficulty:** Easy  
**Pattern:** Total Sum + Running Left Sum  
**Status:** ✅ Solved

---

## 🧠 Problem Understanding

This problem uses essentially the same idea as `724. Find Pivot Index`.

We need to find the leftmost index where:

```text
sum of elements on left = sum of elements on right
```

---

## 💭 My Approach

I recognized that I had already solved almost the same problem.

Instead of trying to invent a new approach, I reused the logic from `724`.

This was useful because it helped me understand that two different LeetCode problems can test the **same underlying pattern**.

---

## 🔗 Pattern Connection

```text
724 → Pivot Index
1991 → Middle Index
```

Both use:

```text
Total Sum
   ↓
Running Left Sum
   ↓
Right Sum = Total - Left - Current
   ↓
Compare
```

---

## 🎯 Main Learning

One of the biggest DSA skills is recognizing when a new problem is actually a variation of something I already know.

Instead of solving every problem from zero:

> **Look for patterns from previous problems.**

---

# 3. 747. Largest Number At Least Twice of Others

**Difficulty:** Easy  
**Pattern:** Find Maximum + Validate Against Others  
**Status:** ✅ Solved

---

## 🧠 Problem Understanding

We need to find the largest number and check whether it is at least twice every other number.

Example:

```text
nums = [3,6,1,0]
```

Largest:

```text
6
```

Check:

```text
6 >= 2*3 ✅
6 >= 2*1 ✅
6 >= 2*0 ✅
```

So return the index of `6`.

---

## 💭 My Initial Thinking

Initially, I tried to do everything in a single loop.

But I mixed up:

```text
index
```

and:

```text
value
```

For example, I used a variable like `maxIndex` and then compared an array value directly with that index.

That was incorrect.

---

## 🔑 Important Concept

I learned to keep these two ideas separate:

```text
maxIndex      → position of largest element
nums[maxIndex] → actual largest value
```

This distinction is important whenever a problem asks for both a value and its index.

---

## 💭 Improved Approach

I decided to make the problem into two clear steps:

```text
1. Find the largest element and its index.
2. Check the largest element against every other element.
```

This made the problem much easier to reason about.

---

## 💻 Final Approach

```java
int maxIndex = 0;

for (int i = 1; i < nums.length; i++) {
    if (nums[i] > nums[maxIndex]) {
        maxIndex = i;
    }
}

for (int j = 0; j < nums.length; j++) {
    if (j != maxIndex && nums[maxIndex] < 2 * nums[j]) {
        return -1;
    }
}

return maxIndex;
```

---

## 📊 Complexity

```text
Time: O(n)
Space: O(1)
```

---

## 🎯 Main Learning

Although I wanted to solve it in one loop, I learned that a two-loop solution can still be optimal when the total complexity remains `O(n)`.

The important thing is not to force everything into one loop just because it looks shorter.

> **Readable and understandable logic is more important than unnecessary cleverness.**

---

# 4. 1534. Count Good Triplets

**Difficulty:** Easy  
**Pattern:** Brute Force + Triplet Search  
**Status:** ✅ Solved

---

## 🧠 Problem Understanding

A good triplet uses three indexes:

```text
i < j < k
```

and must satisfy three conditions:

```text
|arr[i] - arr[j]| <= a
|arr[j] - arr[k]| <= b
|arr[i] - arr[k]| <= c
```

---

## 💭 My Initial Thinking

I immediately recognized this as another **three-loop brute-force** problem.

This connected with:

```text
1925. Count Square Sum Triples
```

which I had solved earlier.

Instead of trying to find a complicated optimization, I could simply try every valid combination of three indexes and check the conditions.

---

## 🔑 Important Improvement

I initially wrote loops like:

```java
i = 1 to n
j = 1 to n
k = 1 to n
```

but I realized that these are **indexes**, not values.

The array size is:

```java
arr.length
```

and the required condition is:

```text
i < j < k
```

So the loops should naturally be:

```java
for (int i = 0; i < arr.length; i++)
for (int j = i + 1; j < arr.length; j++)
for (int k = j + 1; k < arr.length; k++)
```

This automatically guarantees the correct index order.

---

## 💻 Final Approach

```java
int count = 0;

for (int i = 0; i < arr.length; i++) {
    for (int j = i + 1; j < arr.length; j++) {
        for (int k = j + 1; k < arr.length; k++) {

            if (Math.abs(arr[i] - arr[j]) <= a &&
                Math.abs(arr[j] - arr[k]) <= b &&
                Math.abs(arr[i] - arr[k]) <= c) {
                count++;
            }
        }
    }
}

return count;
```

---

## 📊 Complexity

```text
Time: O(n³)
Space: O(1)
```

The brute-force solution is acceptable because the constraints are small.

---

# 📚 Java / DSA Concepts Learned Today

- Total sum
- Running sum
- Pivot index
- Reusing patterns across similar problems
- Difference between index and value
- Finding maximum element with its index
- Validating a maximum against all other elements
- Nested loops
- Triplet search
- `i < j < k` index ordering
- `Math.abs()`
- Brute-force decision based on constraints
- O(1) extra space
- Keeping code simple and readable

---

# 🔥 Important Patterns From Day 30

### Pattern 1 — Total Sum + Left Sum

```text
total
  ↓
leftSum
  ↓
rightSum = total - leftSum - current
```

### Pattern 2 — Reuse Previous Patterns

```text
724 → 1991
```

Same core idea, different problem statement.

### Pattern 3 — Index vs Value

```text
maxIndex       → position
nums[maxIndex] → value
```

### Pattern 4 — Triplet Brute Force

```text
for i
    for j = i + 1
        for k = j + 1
            check conditions
```

### Pattern 5 — Constraints Decide Optimization

If the input is small, a simple brute-force solution can be better than forcing a complicated optimization.

---

# 🔗 Connection With Previous Learning

## Pivot / Prefix Sum Problems

`724` and `1991` showed me that I can reuse a solution pattern instead of treating every problem as completely new.

## Brute Force Triplets

`1534` connected directly with `1925`.

Both problems use:

```text
three loops
   ↓
choose three values/indexes
   ↓
check a condition
   ↓
count valid combinations
```

## Array Indexing

The `747` and `1534` problems reinforced that I need to distinguish:

```text
index → position
value → nums[index]
```

This connects with my earlier recurring mistakes involving arrays and their elements.

---

# 📈 Growth / Improvement

Today I improved most in **pattern recognition**.

I recognized that:

```text
1991 ≈ 724
1534 ≈ 1925
```

Instead of treating them as completely new problems, I reused ideas I had already learned.

I also realized that I sometimes try to make a solution unnecessarily clever.

For example, in `747`, I wanted to force a one-loop solution even though the simple two-loop solution was already `O(n)`.

This taught me:

> **Don't optimize the number of loops; optimize the actual time complexity and keep the logic understandable.**

---

# 📝 Mistakes I Want To Remember

### 1. Index vs Value Confusion

Do not compare an array value with an index.

Remember:

```text
index → position
array[index] → value
```

### 2. Trying To Force One Loop

A solution does not become better just because it uses fewer loops.

Always look at the overall complexity.

### 3. Using the Wrong Range for Indexes

For an array:

```java
0 <= index < arr.length
```

And when the problem says:

```text
i < j < k
```

use:

```java
j = i + 1
k = j + 1
```

---

# 🎯 What I Should Remember

```text
Pivot / Middle Index:
right = total - left - current

Maximum + Index:
maxIndex → position
nums[maxIndex] → value

Triplets:
i < j < k

Absolute Difference:
Math.abs(x - y)

Brute Force:
Use it when constraints are small.

Optimization:
Focus on time complexity, not just number of loops.
```

---

# ✅ Day 30 Status

**Problems Solved:** 4

**Problems:**

- `724. Find Pivot Index` ✅
- `1991. Find the Middle Index in Array` ✅
- `747. Largest Number At Least Twice of Others` ✅
- `1534. Count Good Triplets` ✅

**Main Topics:** Prefix/Total Sum, Maximum Value, Index Handling, Brute Force, Triplet Search

## 🚀 Day 30 — Completed

Today I solved four problems and, more importantly, started recognizing when a new problem is just a variation of a pattern I already know.

The biggest takeaway from today is:

> **Don't solve every problem from scratch. Look for connections with problems you've already solved.**

# 👋 See You on Day 31!

# 📖 LeetCode Learning Log — Day 31

**Date:** 16-08-2026

## Problems Solved

### 1. 1588. Sum of All Odd Length Subarrays

**Difficulty:** Easy  
**Pattern:** Subarray Traversal + Running Sum  
**Status:** ✅ Solved

## 🧠 Problem Understanding

The problem asks for the sum of all **odd-length subarrays**.

An odd-length subarray has length:

```text
1, 3, 5, 7, ...
```

A subarray must be continuous.

## 💭 My Initial Thinking

At first, I checked:

```java
arr.length % 2 == 1
```

but that checks the length of the whole array, not each subarray.

I then understood that I need:

```text
i → starting index
j → ending index
```

and:

```text
length = j - i + 1
```

## ❌ My Mistake

I initially tried:

```java
sum = arr[i] + arr[j];
```

But that only adds the first and last elements.

For:

```text
[1,4,2]
```

the sum must be:

```text
1 + 4 + 2
```

I first thought I would need a third loop to calculate the subarray sum.

## 🔑 Improvement

Instead, I learned to maintain a running sum:

```java
subsum += arr[j];
```

So the process becomes:

```text
Fix i
  ↓
Move j forward
  ↓
Keep updating subsum
  ↓
Check if length is odd
  ↓
Add subsum if odd
```

This removed the unnecessary third loop.

---

# 2. 1351. Count Negative Numbers in a Sorted Matrix

**Difficulty:** Easy  
**Pattern:** 2D Array Traversal  
**Status:** ✅ Solved

## 🧠 Problem Understanding

The task is to count all negative numbers in a 2D matrix.

The straightforward idea is:

```text
Visit every element
    ↓
If element < 0
    ↓
count++
```

## 💭 My Initial Thinking

I understood the overall logic quickly, but I made another 2D-array indexing mistake.

I used the wrong loop boundary and also tried to access:

```java
grid[j]
```

instead of the actual element.

## ❌ My Mistake

I again confused:

```text
grid.length
grid[i].length
grid[i][j]
```

I need to remember:

```text
grid.length       → rows
grid[i].length    → columns in row i
grid[i][j]        → one element
```

## 🔑 Improvement

After correcting the indexes, the solution became straightforward:

```text
Traverse every row
    ↓
Traverse every element
    ↓
Check if negative
    ↓
Count
```

---

# 3. 1281. Subtract the Product and Sum of Digits of an Integer

**Difficulty:** Easy  
**Pattern:** Digit Extraction  
**Status:** ✅ Solved

## 🧠 Problem Understanding

The problem asks for the product of the digits minus the sum of the digits.

## 💭 My Approach

For each digit:

```java
int digit = n % 10;
```

gets the last digit.

Then:

```java
n /= 10;
```

removes the last digit.

I kept a running `sum` and `product`.

## 🔑 Main Pattern

```text
n % 10 → get last digit
n / 10 → remove last digit
```

This is useful for many number problems.

---

# 4. 2236. Root Equals Sum of Children

**Difficulty:** Easy  
**Pattern:** Binary Tree Node Access  
**Status:** ✅ Solved

## 🧠 Problem Understanding

The problem simply checks whether:

```text
root value = left child value + right child value
```

For example:

```text
       10
      /       4    6
```

Then:

```text
10 = 4 + 6
```

so the answer is `true`.

## 💭 My Approach

I used:

```java
root.val
root.left.val
root.right.val
```

and compared them directly.

## 🔑 Main Learning

For a binary tree node:

```text
root.val        → current value
root.left       → left child
root.right      → right child
root.left.val   → left child value
root.right.val  → right child value
```

---

# 5. 2169. Count Operations to Obtain Zero

**Difficulty:** Easy  
**Pattern:** Simulation + While Loop  
**Status:** ✅ Solved

## 🧠 Problem Understanding

The problem repeatedly subtracts the smaller number from the larger until one becomes zero.

Every subtraction counts as one operation.

## 💭 My Approach

I used:

```text
If num1 >= num2
    subtract num2 from num1
Otherwise
    subtract num1 from num2

count++
```

and continued while both numbers were non-zero.

## 🔑 Main Learning

This is a simple simulation pattern:

```text
Check condition
    ↓
Update state
    ↓
Count operation
    ↓
Repeat
```

---

# 6. 657. Robot Return to Origin

**Difficulty:** Easy  
**Pattern:** State Tracking / Simulation  
**Status:** ✅ Solved

## 🧠 Problem Understanding

The robot receives movement commands:

```text
U → Up
D → Down
L → Left
R → Right
```

The goal is to check whether it returns to the starting position.

## 💭 My Approach

I tracked two values:

```text
leftright
updown
```

Then:

```text
U → updown++
D → updown--
L → leftright--
R → leftright++
```

At the end, both must be zero.

## 🔑 Main Learning

This is another state-tracking pattern:

```text
Read command
   ↓
Update state
   ↓
Continue
   ↓
Check final state
```

---

# 🏆 100+ LeetCode Milestone

Today I also crossed an important milestone:

## **101 LeetCode Problems Solved 🎉**

Current progress shown today:

```text
Total Solved: 101
Easy: 93
Medium: 8
Hard: 0
Active Days: 44
Max Streak: 33
Submissions: 139
```

The biggest achievement is not just the number `101`.

I am beginning to recognize connections between problems:

```text
724 + 1991
→ Same total-sum / left-sum idea

1925 + 1534
→ Similar brute-force triplet thinking

2958 + 3090
→ Similar frequency-limited Sliding Window thinking
```

---

# 📚 Java / DSA Concepts Learned Today

- Odd-length subarrays
- Running subarray sum
- 2D array traversal
- Recurring 2D indexing
- Digit extraction
- `% 10` and `/ 10`
- Binary tree node access
- Simulation
- State tracking
- `while` loops
- Counting operations
- Pattern recognition

---

# 🔥 Important Patterns From Day 31

### Pattern 1 — Running Subarray Sum

```java
subsum += arr[j];
```

### Pattern 2 — Odd-Length Check

```java
length % 2 == 1
```

### Pattern 3 — 2D Array Traversal

```text
grid.length       → rows
grid[i].length    → columns
grid[i][j]        → element
```

### Pattern 4 — Digit Extraction

```text
n % 10 → last digit
n / 10 → remove last digit
```

### Pattern 5 — Tree Node Access

```text
root.val
root.left.val
root.right.val
```

### Pattern 6 — Simulation

```text
Read input
   ↓
Update state
   ↓
Repeat
   ↓
Check final state
```

---

# 📝 Mistakes I Want To Remember

### 1. 2D Array Indexing

I am still repeating this mistake:

```text
grid.length
grid[i].length
grid[i][j]
```

I need to slow down and identify what `i` and `j` represent before writing the inner loop.

### 2. Whole Array vs Subarray Length

I initially checked:

```java
arr.length
```

when I actually needed:

```java
j - i + 1
```

The whole array length and the current subarray length are different things.

### 3. Recalculating Instead of Maintaining

For odd-length subarrays, I first thought about a third loop.

I learned that a running `subsum` is enough.

---

# 📈 Growth / Improvement

Today I solved several problems that looked very different:

```text
Subarrays
2D arrays
Numbers
Binary trees
Simulation
Movement tracking
```

But I am starting to see repeated ideas underneath them:

```text
Maintain a value
Track state
Traverse
Check a condition
Update an answer
```

The biggest improvement is that I am becoming more comfortable starting with a **simple direct approach** instead of immediately searching for a complicated trick.

And crossing **100+ solved problems** today shows that the consistency is paying off.

---

# 🎯 What I Should Remember

```text
Odd subarray length:
j - i + 1

Running subarray sum:
subsum += arr[j]

2D array:
grid[i][j]

Digit:
n % 10

Remove digit:
n /= 10

Tree:
root.val
root.left.val
root.right.val

Simulation:
update state → repeat → check result
```

---

# ✅ Day 31 Status

**Problems Solved Today:** 6

**Problems:**

- `1588. Sum of All Odd Length Subarrays` ✅
- `1351. Count Negative Numbers in a Sorted Matrix` ✅
- `1281. Subtract the Product and Sum of Digits of an Integer` ✅
- `2236. Root Equals Sum of Children` ✅
- `2169. Count Operations to Obtain Zero` ✅
- `657. Robot Return to Origin` ✅

**Major Milestone:** **101 LeetCode problems solved 🎉**

**Main Topics:** Subarrays, 2D Arrays, Digit Processing, Binary Trees, Simulation, State Tracking

## 🚀 Day 31 — Completed

Today I crossed **100 solved LeetCode problems** and reached **101 total solves**.

More importantly, I am starting to see the common thinking behind different problems instead of treating every problem as completely new.

> **The goal is not just to solve more problems. The goal is to recognize patterns faster and think more clearly.**

# 👋 See You on Day 32!

# 📖 LeetCode Learning Log — Day 32

**Date:** 17-08-2026

## Problem Solved

### 1. 1854. Maximum Population Year

**Difficulty:** Easy  
**Pattern:** Difference Array + Running Population  
**Status:** ✅ Solved

---

## 🧠 Problem Understanding

The problem gives a list of people's birth and death years.

For each person:

```text
[birth, death]
```

the person is counted in every year from:

```text
birth
```

up to:

```text
death - 1
```

The goal is to find the year with the **maximum population**.

If multiple years have the same maximum population, return the **earliest** year.

---

## 💭 My Initial Thinking

I spent a lot of time trying to understand what the problem was actually asking.

My first thought was:

```text
death - birth
```

because I thought I could use that to determine the number of years a person lived.

That calculation is valid, but it answers a different question.

It tells me:

```text
how many years one person was alive
```

The actual problem asks:

```text
how many people were alive in each year
```

That was the first important distinction I had to understand.

---

## ❌ Initial Confusion

I then started thinking:

> "For a particular year, I need to check whether each person's birth/death range includes that year."

For example:

```text
Person 1 = [1950, 1961]
Person 2 = [1960, 1971]
```

For year `1960`:

```text
Person 1 → alive ✅
Person 2 → alive ✅
```

So:

```text
population(1960) = 2
```

This helped me finally understand that the problem is about **overlapping lifetimes**.

---

## 💡 First Possible Approach I Understood

I realized I could conceptually do:

```text
For every year
    ↓
Check every person
    ↓
If birth <= year < death
    ↓
count++
    ↓
compare population
```

This helped me understand the problem.

But then I noticed that there should be a better way because I do not actually need to repeatedly ask which people are alive.

---

## 🔥 Main Breakthrough

The biggest moment was realizing:

```text
Birth year → population increases by 1
Death year → population decreases by 1
```

For example:

```text
[1950, 1961]
```

can be viewed as:

```text
1950 → +1
1961 → -1
```

Then I can scan through the years and maintain the current population.

This completely changed how I was thinking about the problem.

Instead of:

```text
"Who is alive this year?"
```

I started thinking:

```text
"When does the population change?"
```

That was the key insight.

---

## 🧠 Constraint Insight

The problem gives:

```text
1950 <= birth < death <= 2050
```

So the year range is very small.

There are only:

```text
2050 - 1950 + 1 = 101
```

possible years.

That is why using:

```java
int[] change = new int[101];
```

makes sense.

The array position represents an offset from `1950`.

For example:

```text
1950 → index 0
1951 → index 1
1952 → index 2
...
2050 → index 100
```

---

## 💻 Final Approach

```java
class Solution {
    public int maximumPopulation(int[][] logs) {
        int[] change = new int[101];

        for (int i = 0; i < logs.length; i++) {
            int birth = logs[i][0];
            int death = logs[i][1];

            change[birth - 1950]++;
            change[death - 1950]--;
        }

        int current = 0;
        int maxPopulation = 0;
        int answer = 0;

        for (int j = 0; j < change.length; j++) {
            current += change[j];

            if (current > maxPopulation) {
                maxPopulation = current;
                answer = j + 1950;
            }
        }

        return answer;
    }
}
```

---

## 🔍 How I Understand the Final Code

For each person:

```text
birth → +1
death → -1
```

Then scan the years.

The running value:

```text
current
```

represents the population for that year.

When:

```text
current > maxPopulation
```

I update the answer.

I use `>` instead of `>=` because the problem wants the **earliest** year when the maximum population occurs.

So if:

```text
1960 → population 2
1970 → population 2
```

the answer remains:

```text
1960
```

---

## ❌ Mistakes I Made

### 1. Confusing Lifetime With Population

I kept thinking about:

```text
death - birth
```

but that only tells me how long one person is alive.

I needed to think about **how many people's ranges overlap a particular year**.

### 2. Confusing the Data Structure With the Actual Question

Initially, I focused too much on traversing:

```text
logs[i][j]
```

instead of asking:

> "What is the problem actually asking me to count?"

This reminded me that understanding the problem comes before writing loops.

### 3. Taking Time To Recognize the Optimization

I spent around **1.2 hours** understanding this problem.

At first, that felt too long, but by the end I understood the change-based approach myself.

The important part is that I did not just memorize the solution.

I understood why:

```text
birth = +1
death = -1
```

works.

---

## 📈 Growth / Improvement

This problem took much longer than some of the previous Easy problems.

But it taught me something important:

> **A problem can be Easy by LeetCode's label and still require a completely new way of thinking.**

I also learned that spending a lot of time on one problem is not automatically bad if I actually understand the idea by the end.

Today I went through:

```text
Confusion
   ↓
Wrong interpretation
   ↓
Understand one year
   ↓
Think about checking every person
   ↓
Notice population changes
   ↓
Birth = +1
Death = -1
   ↓
Understand difference array
```

That entire process was valuable.

---

# 🔥 Important Pattern Learned

## Difference Array / Change Tracking

Instead of storing the whole population for every person:

```text
record when something starts
record when something ends
then accumulate the changes
```

For this problem:

```text
birth → +1
death → -1
```

Then:

```text
current += change[year]
```

gives the population.

---

# 🔗 Connection With Previous Learning

This problem was different from most of the brute-force problems I had been solving.

Earlier, I often thought:

```text
Try every possibility
Check the condition
Count
```

Here I learned a different mindset:

```text
Track changes
Accumulate the state
Find the maximum
```

This is a useful step forward because I am starting to see that DSA is not only about loops and conditions.

Sometimes the important part is recognizing **how the data changes over time**.

---

# 🎯 What I Should Remember

```text
death - birth
→ person's lifetime

population(year)
→ number of people alive that year

birth
→ +1

death
→ -1

running population
→ current += change[year]

tie
→ keep the earlier year
```

---

# ✅ Day 32 Status

**Problems Solved:** 1

**Problem:**

- `1854. Maximum Population Year` ✅

**Main Topic:** Difference Array / Change Tracking

**Biggest Lesson:**

> **Don't just ask what each individual value means. Ask how the entire state changes over time.**

## 🚀 Day 32 — In Progress

This problem took me around **1.2 hours to truly understand**, but that time gave me a new way of thinking about timeline-based problems.

I am learning that **understanding is more important than speed**.

# 👋 On day 33

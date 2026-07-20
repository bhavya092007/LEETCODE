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

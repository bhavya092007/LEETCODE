# 🚀 My LeetCode Journey — From Confusion to Confidence

## Introduction

When I started solving LeetCode problems, I thought the biggest challenge would be finding the solution.

But slowly I realized something:

> The hardest part was not finding the answer. The hardest part was training my brain to break problems into smaller logical steps and convert those thoughts into code.

I already knew programming concepts, but implementing those concepts correctly was a completely different skill.

Understanding a concept and writing a working solution are two different things.


---

# 📅 Journey Timeline


| Day | Problems Solved | Main Concepts Learned |
|-----|----------------|----------------------|
| Day 1 | 5 Problems | Arrays, Loops, Prefix Sum, Conditions |
| Day 2 | 6 Problems | Strings, ArrayList, Nested Loops, Mapping |


*(Future days will be added here)*


---

# 📅 Day 1 — Building The Foundation


## Problems Solved

- LeetCode 2235 — Add Two Integers
- LeetCode 1480 — Running Sum of 1D Array
- LeetCode 1929 — Concatenation of Array
- LeetCode 2011 — Final Value of Variable After Performing Operations
- LeetCode 2114 — Maximum Number of Words Found in Sentences


---

# 🧠 Day 1 Learning


## 1. Function Understanding

Learned how LeetCode functions work.

Example:

```java
public int functionName(parameters)
{

}
```

Important things:

- Understanding parameters.
- Understanding return type.
- Returning correct values.


---

## 2. Array Traversal

Learned how to visit every element of an array.


Pattern:

```java
for(int i = 0; i < arr.length; i++)
{

}
```


Learning:

- Accessing values using indexes.
- Understanding positions.
- Processing each element.


---

## 3. Creating New Arrays


Pattern:

```java
int[] ans = new int[size];
```


Learning:

```
Create Array
      ↓
Store Values
      ↓
Return Answer
```


---

## 4. Running Sum Pattern


Problem:

LeetCode 1480 — Running Sum of 1D Array


Important pattern:

```java
arr[i] = arr[i] + arr[i-1];
```


Learning:

Current answer can depend on previous values.


---

## 5. Array Concatenation


Problem:

LeetCode 1929 — Concatenation of Array


Learned:

- Creating larger arrays.
- Copying values using indexes.


Example:

```
Input:

[1,2,3]


Output:

[1,2,3,1,2,3]
```


---

## 6. Conditions & Variables


Problem:

LeetCode 2011


Learned:

- if-else conditions.
- Incrementing variables.
- Decrementing variables.


---

## 7. Maximum Value Pattern


Problem:

LeetCode 2114


Important pattern:


```java
if(current > max)
{
    max = current;
}
```


Used in:

- Maximum value problems.
- Best answer tracking.
- Comparison problems.


---

# 📅 Day 2 — Strings, Lists & Index Mapping


## Problems Solved

- LeetCode 2114 — Maximum Number of Words Found in Sentences
- LeetCode 2942 — Find Words Containing Character
- LeetCode 412 — Fizz Buzz
- LeetCode 2469 — Convert the Temperature
- LeetCode 2652 — Sum Multiples
- LeetCode 1528 — Shuffle String


---

# 🧠 Day 2 Learning


## 1. String Traversal


Learned that a String contains:

- Characters
- Positions
- Indexes


Example:

```java
String s = "hello";

s.charAt(0);
```


Output:

```
h
```


Learned:

- Traversing characters.
- Counting characters.
- Searching inside strings.


---

# 2. Nested Loop Thinking


Many string problems follow:


```
Array of Strings

        ↓

Individual String

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


Used for:

- Searching characters.
- Comparing characters.
- Processing strings.


---

# 3. ArrayList


Learned dynamic storage.


Creating:

```java
List<Integer> ans = new ArrayList<>();
```


Adding:

```java
ans.add(i);
```


Used in:

LeetCode 2942


---

# 4. FizzBuzz Logic


Problem:

LeetCode 412


Important:

Condition order matters.


Correct thinking:


```
Check divisible by 3 and 5

↓

Check divisible by 3

↓

Check divisible by 5

↓

Else return number
```


Learned:

```java
String.valueOf(number);
```


Converts:

```
int → String
```


---

# 5. Returning Multiple Values


Problem:

LeetCode 2469


Learned:

Returning arrays.


Pattern:


```java
double[] ans = new double[2];

ans[0] = value1;
ans[1] = value2;

return ans;
```


---

# 6. Modulus Pattern


Used in:

- FizzBuzz
- Sum Multiples


Pattern:


```java
number % divisor == 0
```


Meaning:

Number is completely divisible.


---

# 7. Index Mapping


Problem:

LeetCode 1528 — Shuffle String


Biggest learning of Day 2.


Example:

```
s = "abc"

indices = [2,1,0]
```


Meaning:


```
a → index 2
b → index 1
c → index 0
```


Final pattern:


```java
answer[indices[i]] = s.charAt(i);
```


Learning:


```
Old Position → New Position
```


---

# 🐛 My Mistake Database


## Java Syntax Mistakes


---

## 1. length vs length()


Array:

```java
arr.length
```


String:

```java
str.length()
```


---

## 2. String Comparison


Wrong:


```java
str == "text"
```


Correct:


```java
str.equals("text")
```


---

## 3. char vs char[]


Single character:


```java
char ch = 'a';
```


Multiple characters:


```java
char[] ch;
```


---

## 4. Array Creation


Wrong:


```java
char arr[size];
```


Correct:


```java
char[] arr = new char[size];
```


---

## 5. Returning Wrong Data Type


If function requires:


```java
String
```


Cannot return:


```java
char[]
```


Convert using:


```java
new String(charArray)
```


---

## 6. Creating String Too Early


Wrong:


```
Create String

↓

Fill Array
```


Correct:


```
Fill Character Array

↓

Convert Into String
```


---

# 🔥 Pattern Library


## Array Traversal

```java
for(int i = 0; i < arr.length; i++)
{

}
```


---

## Character Access

```java
str.charAt(i)
```


---

## String Conversion

```java
String.valueOf(number)
```


---

## Character Array To String

```java
new String(charArray)
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

## Index Mapping

```java
result[newPosition] = value;
```


---

# 📚 My Learning System


For every problem:


```
1. Understand the problem statement.

2. Identify input and output.

3. Think about the brute-force approach.

4. Write logic in simple words.

5. Convert logic into code.

6. Debug mistakes.

7. Write what I learned.

8. Save reusable patterns.
```


---

# 📅 Future Day Template


## Day X — Problem Solving


### Problems Solved

- LeetCode XXXX — Problem Name


---

### My First Thought

What I understood initially.


---

### My Approach

Step-by-step thinking.


---

### Mistakes I Made

- Syntax mistakes.
- Logic mistakes.
- Wrong approach.


---

### What I Learned


Concepts and patterns learned.


---

### Pattern To Remember


```java

Reusable code pattern

```


---

### My Improvement

Before:

"I was confused about..."


After:

"Now I understand..."


---

# 📈 Progress After 2 Days


Problems Solved:

```
10 Problems
```


Concepts Learned:

- Arrays
- Strings
- Loops
- Nested Loops
- ArrayList
- Character Arrays
- Type Conversion
- Index Mapping
- Return Types
- Modulus Operator
- Prefix Sum


---

# Advice For Beginners


## 1. Do Not Rush To Hard Problems

Easy problems build strong foundations.


---

## 2. Maintain A Mistake Log

Your mistakes become your personal roadmap.


---

## 3. Understand Before Coding


Always ask:


```
What is the input?

What is the output?

What data structure should I use?

What pattern does this problem follow?
```


---

## 4. Do Not Compare Speed


Someone solving faster does not mean they are learning better.


Focus on improvement.


---

# Final Message


I started with confusion.

I struggled with syntax.

I struggled with indexes.

I struggled with converting ideas into code.


But every mistake added one small piece of understanding.


The goal is not only solving thousands of problems.

The goal is becoming a better problem solver every day.


One problem at a time. 🚀


---

# 📅 Day 3 — Mapping, Counting & Processing Numbers


## Problems Solved

- LeetCode 1920 — Build Array from Permutation
- LeetCode 1365 — How Many Numbers Are Smaller Than the Current Number
- LeetCode 1295 — Find Numbers with Even Number of Digits


---

# 🧠 Day 3 Learning


## 1. Mapping Can Happen More Than Once


Problem:

LeetCode 1920 — Build Array from Permutation


After learning index mapping in Shuffle String, I encountered another mapping problem.

At first I thought:

```java
ans[i] = nums[i];
```

But the problem required:

```java
ans[i] = nums[nums[i]];
```

This taught me:

```
Index

↓

Value

↓

Another Index

↓

Final Value
```

For the first time I understood that indexes themselves can become data.

This was an important step in improving my problem-solving ability.


---

## 2. Correct Array Creation


One mistake I made:

```java
int ans[] = new ans;
```

Learned:

```java
int[] ans = new int[nums.length];
```

This reinforced a pattern I must remember:

```java
datatype[] arrayName = new datatype[size];
```


---

## 3. Loop Boundary Understanding


Initially I still sometimes wrote:

```java
i <= nums.length
```

But I learned again:

Arrays are 0-indexed.

Correct:

```java
i < nums.length
```

Because:

```
Last Index

=

length - 1
```


---

## 4. Counting Pattern


Problem:

LeetCode 1365 — How Many Numbers Are Smaller Than the Current Number


My thinking process:

For every number:

```
Compare with every other number

↓

If smaller

↓

Increase count
```

Pattern:

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


This problem strengthened my understanding of nested loops.


---

## 5. Storing Answers In Arrays


Important realization:

```java
count[i]
```

stores the answer for:

```java
nums[i]
```

I learned that answer arrays often work like:

```
Input Position

↓

Output Position
```

Every index stores its own answer.


---

## 6. Runtime Is Not Everything


For LeetCode 1365 my solution achieved:

```
7 ms

Beats 82.27%
```

This taught me something important.

Even a simple brute-force solution can perform well.

First priority:

```
Correct Solution
```

Then:

```
Optimization
```


---

## 7. Arrays vs Elements


Problem:

LeetCode 1295 — Find Numbers with Even Number of Digits


One of my biggest mistakes today:

Wrong thinking:

```java
while(nums != 0)
```

I forgot:

```java
nums
```

is an entire array.

What I actually needed:

```java
int num = nums[i];
```

This created a very important lesson:

```
Array

↓

Select Element

↓

Process Element
```


---

## 8. Digit Counting Pattern


Initially I knew:

```
Division by 10

↓

Related to digits
```

But I couldn't convert that idea into code.

Eventually I learned:

```java
while(num != 0)
{
    num /= 10;
    digits++;
}
```

Every division removes one digit.

Example:

```
1234

↓

123

↓

12

↓

1

↓

0
```

Total digits:

```
4
```


---

## 9. Variable Scope Matters


Another mistake:

I created:

```java
int digits = 0;
```

outside the loop.

Because of that:

```
Digit counts from previous numbers

↓

Continued into next numbers
```

Learned:

```java
for(...)
{
    int digits = 0;
}
```

Each number needs its own fresh counter.


---

## 10. Understanding What The Problem Is Asking


One mistake I repeatedly made today:

Checking:

```java
nums[i] % 2 == 0
```

I was checking whether the number was even.

But the problem wanted:

```
Is the number of digits even?
```

This taught me:

Before coding, always ask:

```
What exactly am I counting?
```

Because many mistakes happen when solving the wrong sub-problem.


---

# 🐛 New Mistakes Added To My Mistake Database


## 7. Arrays vs Elements


Wrong Thinking:

```java
nums
```

Correct Thinking:

```java
nums[i]
```

Always ask:

```
Am I working with the entire array

or

one element?
```


---

## 8. Counter Scope


Wrong:

```java
int count = 0;
```

outside the required loop.

Correct:

Reset counters whenever a new element needs independent processing.


---

## 9. Counting The Wrong Thing


Wrong:

```
I know how to code.

↓

I immediately start coding.
```

Correct:

```
Understand exactly what needs to be counted.

↓

Then write code.
```


---

# 🔥 New Patterns Learned


## Nested Mapping


```java
ans[i] = nums[nums[i]];
```


---

## Counting Smaller Elements


```java
if(nums[i] > nums[j])
{
    count[i]++;
}
```


---

## Digit Counting


```java
while(num != 0)
{
    num /= 10;
    digits++;
}
```


---

## Array Element Processing


```java
int num = nums[i];
```


Process the element.

Not the entire array.


---

# 📈 Progress After 3 Days


Problems Solved:

```
13 Problems
```


New Concepts Learned Today:

- Nested Mapping
- Counting Patterns
- Digit Processing
- Variable Scope
- Array vs Element Thinking
- Nested Loop Comparison
- Runtime Awareness


---

# My Biggest Realization Today


Day 1 was about syntax.

Day 2 was about strings and mapping.

Day 3 was about understanding exactly what needs to be counted and processed.

I noticed that most of my mistakes no longer come from not knowing Java.

Most mistakes now come from:

- Understanding the problem incorrectly.
- Processing the wrong thing.
- Applying logic to an entire array instead of one element.
- Forgetting where variables should be reset.

This is a good sign.

It means I am slowly moving from learning syntax to learning problem solving.


---

# My Improvement


Before:

```
I struggled to understand what loops should do.
```

Now:

```
I can identify patterns like:

- Mapping
- Counting
- Comparison
- Digit Processing
```

Before:

```
I focused only on getting an answer.
```

Now:

```
I focus on understanding the pattern behind the answer.
```

That pattern can be reused in future problems.

And that is what turns problem solving into skill building. 🚀


# 📅 Day 4 — The Day I Started Solving Problems on Paper First

## Problems Solved

- LeetCode 1470 — Shuffle the Array
- LeetCode 1431 — Kids With the Greatest Number of Candies
- LeetCode 1732 — Find the Highest Altitude

---

# 🎯 Day 4 Overview

Today was different from the last few days.

For the past 3 days, I usually read the problem and immediately started writing code.

My thinking process looked like:

```text
Read Problem

↓

Get Idea

↓

Start Coding Immediately

↓

Get Stuck

↓

Debug

↓

Fix Mistakes
```

This often resulted in:

- More syntax mistakes
- More logic mistakes
- More confusion
- More debugging time

Today I tried something different.

Before writing code, I manually decoded the problem in my notebook.

I wrote:

```text
What is the input?

↓

What is the output?

↓

What exactly is happening?

↓

Can I create an example manually?

↓

What pattern does this problem follow?

↓

Then write code
```

This single change reduced many mistakes.

It also made the solutions feel much clearer.

---

# 🚀 Biggest Learning Of Day 4

## Manual Decoding Before Coding

Today I realized:

```text
Coding is not the hard part.

Thinking is the hard part.
```

When I manually decoded the problem first:

- Logic became clearer.
- Mistakes reduced.
- Debugging reduced.
- Confidence increased.
- Coding became easier.

New Problem Solving System:

```text
1. Read Problem

↓

2. Create Manual Example

↓

3. Understand Input

↓

4. Understand Output

↓

5. Find Pattern

↓

6. Write Logic In Words

↓

7. Convert Logic Into Code

↓

8. Debug If Needed
```

This is probably the most important thing I learned today.

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

---

# My Initial Thinking

I kept thinking:

```text
Can I store both values in the same position?
```

Example:

```java
array[i] = nums[i];
array[i] = nums[i+n];
```

Then I realized:

```text
Second assignment overwrites the first.
```

One position can only store one value.

---

# Mistakes Made

## Mistake 1

```java
array[i] = nums[i];
array[i] = nums[i+n];
```

Learning:

```text
One position cannot hold two values.
```

---

## Mistake 2

```java
i++;
```

inside the loop.

Learning:

```text
The loop already controls i.

Changing it manually creates confusion.
```

---

## Mistake 3

I thought I could solve it without another variable.

Learning:

```text
Input position and output position
are different things.
```

---

# Biggest Learning

## Separate Pointer Pattern

```java
array[k] = nums[i];
k++;

array[k] = nums[i+n];
k++;
```

Learning:

```text
A separate pointer can control
where values are stored.
```

---

# LeetCode 1431 — Kids With the Greatest Number of Candies

## Problem Understanding

For every child:

```text
Current Candies

↓

Add Extra Candies

↓

Can this child have the maximum candies?
```

---

# My Initial Thinking

I immediately started adding:

```java
candies[i] + extraCandies
```

without knowing:

```text
Who currently has the maximum candies?
```

---

# Mistakes Made

## Mistake 1

Created:

```java
int[] ans = new int[candies.length];
```

Learning:

```text
Not every problem requires an answer array.
```

---

## Mistake 2

Compared:

```java
ans[i] >= extraCandies
```

Learning:

```text
Need to compare with maximum candies,
not extraCandies.
```

---

## Mistake 3

Compared:

```java
if(i >= total)
```

Learning:

```text
i = position

total = value

Positions and values are different things.
```

---

## Mistake 4

Tried solving before finding maximum.

Learning:

```text
Some problems require information gathering first.
```

---

# Biggest Learning

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

---

# LeetCode 1732 — Find the Highest Altitude

## Problem Understanding

Biker starts at:

```java
0
```

Every gain changes altitude.

Need:

```text
Highest altitude reached.
```

---

# My Initial Thinking

I manually created the altitude sequence:

```java
gain = [-5,1,5,0,-7]
```

Altitude:

```java
[0,-5,-4,1,1,-6]
```

This notebook decoding made the problem much easier.

---

# Mistakes Made

## Mistake 1

```java
alt[i] = altitude + gain[i];
alt[i] += gain[i];
```

Learning:

```text
Gain was added twice.
```

---

## Mistake 2

```java
alt += gain[i];
```

Learning:

```text
Arrays cannot use +=.
```

---

## Mistake 3

Forgot to update:

```java
altitude
```

Learning:

```text
Altitude changes after every move.
```

---

## Mistake 4

Used:

```java
for(int j=0;j<altitude;j++)
```

Learning:

```text
Altitude is a value.

Array traversal requires array length.
```

---

# Biggest Learning

This problem combined two previously learned patterns.

## Running Sum

```java
current += value;
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

# 🐛 Day 4 Mistake Database

## Shuffle Array

- Overwriting values.
- Trying to store two values in one position.
- Confusion about needing a separate pointer.
- Modifying loop variable manually.

---

## Kids With Candies

- Created unnecessary array.
- Compared with extraCandies.
- Compared index with value.
- Tried solving before finding maximum.

---

## Highest Altitude

- Added gain twice.
- Tried += on array.
- Forgot to update altitude.
- Used altitude as loop boundary.

---

# 🔥 New Patterns Added Today

## Separate Pointer Pattern

```java
array[k] = value;
k++;
```

---

## Running Sum Pattern

```java
current += value;
```

---

## Maximum Tracking Pattern

```java
if(current > max)
{
    max = current;
}
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

# 📈 Most Important Improvement

Previous Days:

```text
Read Problem

↓

Start Coding Immediately
```

Day 4:

```text
Read Problem

↓

Decode Manually In Notebook

↓

Create Example

↓

Write Logic

↓

Write Code
```

This reduced mistakes significantly.

It also helped me understand the problem more deeply before touching the keyboard.

---

# 🌟 Day 4 Reflection

Today I learned something more valuable than syntax.

I learned that:

```text
Writing code is not the first step.

Thinking is the first step.
```

The notebook became a debugging tool before the code even existed.

Instead of fixing mistakes after writing code,

I started preventing mistakes before writing code.

This may become one of the most important habits in my entire LeetCode journey.

Because good programmers do not just write code.

They understand the problem first.

🚀

### Time Spent

⏱️ Approximate Time: 1 – 1.2 Hours

This problem took significantly longer than most Easy problems I have solved so far.

The reason was not the Bubble Sort itself, but understanding:

- What "third distinct maximum" actually means.
- How to ignore duplicate values.
- How to count distinct maximums correctly.
- The difference between a helper variable (`count`) and the actual answer.
- Handling the special case when a third distinct maximum does not exist.

### My Struggles

During this problem I made several mistakes:

- Tried returning the count instead of the actual value.
- Confused array values with counters.
- Used `count[k]` even though `count` was not an array.
- Made index boundary mistakes with `k-1`.
- Forgot to handle cases with fewer than 3 distinct values.
- Spent time debugging logic rather than syntax.

### Biggest Learning

This was the first problem where I spent a long time manually tracing examples in my notebook before writing code.

Instead of immediately coding, I repeatedly asked:

```text
What exactly is being counted?

What is the actual answer?

When should duplicates be ignored?

What should happen if the third maximum doesn't exist?
```

This manual decoding process helped me eventually understand the problem and reduce random debugging.

### Reflection

Even though this problem took around 1–1.2 hours, it was one of the most valuable problems I have solved so far because it improved my ability to:

- Trace algorithms manually.
- Debug logic step by step.
- Distinguish helper variables from answer variables.
- Handle edge cases.
- Stay patient when a solution is not immediately obvious.

This problem reminded me that time spent understanding logic is often more valuable than quickly reaching an accepted solution.




### LeetCode 26 — Remove Duplicates from Sorted Array

Time Spent: ~30-40 minutes

#### Mistakes Made

- Initially thought I only needed to count unique elements.
- Tried creating a new array unnecessarily.
- Forgot that the problem requires modifying the same array.
- Used return inside the loop, causing early exit.
- Confused unique count with actual array values.
- Tried returning nums instead of an int.

#### Key Learning

This was my first proper Two Pointer problem.

Pointers:
- i = read pointer
- k = write pointer

The read pointer scans the array.
The write pointer stores unique values at the front.

#### Pattern Learned

if(nums[i] != nums[i-1])
{
    nums[k] = nums[i];
    k++;
}

return k;

#### Biggest Takeaway

Not every problem needs a new array.
Sometimes we can overwrite values inside the same array and keep track of the next valid position using a write pointer.


This is date 20-07-2026(Day 4) ,Today felt difficult because I solved my first few problems that required actual pattern recognition rather than simple loops.

LeetCode 414 (Third Maximum Number) and LeetCode 26 (Remove Duplicates from Sorted Array) forced me to manually trace examples, think about edge cases, and understand what each variable represented.

Although these problems took significantly longer than previous Easy problems, they helped me improve my debugging process and taught me not to rush into coding before fully understanding the problem.


# Day 4 of LeetCode Journey
📅 Date: 21/07/2026

## Progress Update

Today I completed my 20th LeetCode problem. 🚀

This feels like a small number compared to people who have solved hundreds or thousands of problems, but for me it's a meaningful milestone because I am building consistency and learning problem-solving step by step.

## Today's Reflection

Some of today's problems felt genuinely difficult, especially:

- LeetCode 414 — Third Maximum Number
- LeetCode 26 — Remove Duplicates from Sorted Array

There were moments where I got stuck and needed help from AI. Overall, I took significant help in around 4–5 problems, but instead of copying answers, I focused on understanding:

- Why my logic was failing
- What each variable should represent
- How to trace examples manually
- How to debug step by step

## Biggest Improvement Today

For the last few days, I often jumped directly into coding.

Today I spent more time manually decoding problems in my notebook before writing code.

This helped me:
- Understand the problem better
- Reduce random mistakes
- Find logic errors earlier
- Improve my confidence while coding

## Important Patterns Learned

### Two Pointer Pattern
Learned through:
- LeetCode 26 — Remove Duplicates from Sorted Array

Concept:
- One pointer reads data
- One pointer writes data

### Distinct Element Handling
Learned through:
- LeetCode 414 — Third Maximum Number

Concept:
- Counting distinct values
- Ignoring duplicates
- Handling edge cases

## Honest Assessment

Today was not easy.

A few problems took much longer than expected.
Some required AI guidance.
Some logic mistakes took a long time to identify.

But I am happy because I did not quit.

I kept tracing examples, asking questions, debugging, and trying again.

## Current Stats

✅ Day 4 Completed  
✅ 20 LeetCode Problems Solved  
✅ Learning Java + Problem Solving Together  
✅ Building Consistency

## Promise to Myself

I will continue this journey.

The goal is not to solve problems quickly.
The goal is to understand patterns, improve my thinking, and become better than I was yesterday.

One problem at a time.
One day at a time.

See you on Day 5. 🚀

# LEETCODE JOURNEY

## Day 5 (21-07-2026)

Problems Solved Today:
1. LeetCode 344 - Reverse String
2. LeetCode 125 - Valid Palindrome
3. LeetCode 58 - Length of Last Word

Total Problems Solved So Far: 20+

---

# LeetCode 344 — Reverse String

## Concept Learned

Two Pointer Technique

Pointers:

- left = beginning
- right = end

Swap values and move inward.

## Pattern

temp = s[left];
s[left] = s[right];
s[right] = temp;

left++;
right--;

## Mistakes I Made

- Used s.length instead of s.length - 1.
- Tried swapping pointer variables instead of characters.
- Moved pointers before completing swap.
- Tried returning an array from a void method.
- Forgot the problem requires modifying the same array.

## Biggest Learning

When reversing arrays or strings:

Use two pointers from opposite ends and swap until they meet.

## Time Complexity

O(n)

## Space Complexity

O(1)

---

# LeetCode 125 — Valid Palindrome

## Concepts Used

- String Traversal
- Character Functions
- Character.toLowerCase()
- Character.isLetterOrDigit()
- Two Pointers
- Palindrome Checking

## Final Approach

1. Traverse original string.
2. Convert every character to lowercase.
3. Keep only letters and digits.
4. Store cleaned characters in a new string.
5. Use two pointers.
6. Compare from both ends.
7. Return false on mismatch.
8. Return true if all comparisons match.

## Mistakes I Made

- Tried checking palindrome while cleaning the string.
- Compared original string instead of cleaned string.
- Used == " " instead of character comparisons.
- Forgot charAt() returns a char.
- Initialized right before building cleaned string.
- Ignored result of Character.isLetterOrDigit().
- Removed only spaces, commas and colons initially.
- Mixed array syntax and string syntax.

## Biggest Learning

Clean data first, then solve the actual problem.

## Time Complexity

O(n)

## Space Complexity

O(n)

---

# LeetCode 58 — Length of Last Word

## Concepts Used

- Reverse Traversal
- Character Comparison
- Counting Pattern
- Early Return

## Approach

- Traverse from the end.
- Skip trailing spaces.
- Count characters of last word.
- Stop when space is found after counting starts.

## Mistakes I Made

- Wrote conut instead of count.
- Used charAt(i) instead of s.charAt(i).
- Used = instead of ==.
- Returned 0 instead of count.
- Mixed skip-space logic with count logic.

## Pattern Learned

Start From End
↓
Skip Unwanted Characters
↓
Count Useful Characters
↓
Stop At Boundary

## Time Complexity

O(n)

## Space Complexity

O(1)

---

## Day 5 Reflection

Today I became more comfortable with:

- Two Pointers
- Reverse Traversal
- String Cleaning
- Character Functions
- Early Return Logic

Biggest Improvement:
I am starting to recognize patterns before solving instead of randomly trying approaches.

Problems that took the most time:
- LeetCode 125 (Valid Palindrome)
- LeetCode 58 (Length of Last Word)

Mood:
Feeling confident and enjoying the process.


# DAY 6 REFLECTION
Date: 22-07-2026

## Problems Solved

1. LeetCode 28 - Find the Index of the First Occurrence in a String
2. LeetCode 796 - Rotate String
3. LeetCode 242 - Valid Anagram

---

## What I Noticed Today

Today I felt that the problems were easier to understand compared to earlier days.

The biggest difference is that I am starting to recognize patterns on my own.

Before, I often struggled with:

- Understanding the problem.
- Deciding where to start.
- Finding the correct approach.
- Identifying the pattern.

Now I can usually recognize things like:

- This looks like String Matching.
- This can be solved using Reverse Traversal.
- This needs a Frequency Array.
- There may be a hidden pattern instead of simulation.
- This problem can be simplified.

---

## My Biggest Improvement

I feel that my logic is improving.

Many times I can already see the correct idea before writing code.

Examples from today:

### LeetCode 28

I eventually understood:

```java
haystack.charAt(i + j)
needle.charAt(j)
```

and the string matching pattern.

### LeetCode 796

I understood that:

```java
(s + s).contains(goal)
```

is a pattern-based solution and much better than manually rotating characters.

### LeetCode 242

I learned how Frequency Arrays work and why counting character frequencies is more important than simply checking whether characters exist.

---

## What Is Still Holding Me Back

Most of my mistakes are no longer logic mistakes.

My main problems now are:

### Syntax Mistakes

Examples:

```java
s[i]
```

instead of

```java
s.charAt(i)
```

Using:

```java
=
```

instead of

```java
==
```

Confusing:

```java
length
```

and

```java
length()
```

---

### Implementation Mistakes

Examples:

- Boundary conditions.
- Wrong loop limits.
- Returning too early.
- Using break vs return incorrectly.
- Index calculations.

---

### Confidence While Coding

Sometimes I actually know the correct logic but get stuck while converting it into Java code.

---

## Biggest Learning Today

I realized that:

```text
Finding the pattern is harder than writing the code.
```

The code can always be fixed.

But if I can recognize the correct pattern, I am already moving in the right direction.

---

## Current Self Assessment

### Pattern Recognition

8/10

I am starting to identify common patterns myself.

### Problem Understanding

8/10

Most problems make sense after reading carefully.

### Logic Building

7.5/10

I can usually find the correct approach.

### Java Syntax

5.5/10

Still making many small syntax mistakes.

### Implementation

6/10

Need more practice converting ideas into code.

---

## Day 6 Takeaway

Today I learned that my biggest weakness is no longer understanding the problem.

My biggest weakness is implementing the solution correctly.

That is good progress because syntax and implementation improve with practice, while logic takes longer to develop.

I feel more confident than I did on Day 1.

---

## Goal For Day 7

- Reduce syntax mistakes.
- Write correct code with fewer retries.
- Improve boundary-condition handling.
- Continue recognizing patterns before coding.
- Solve problems with less AI help.

---

## Final Reflection

Today was one of my most important learning days.

For the first time, I felt that I could recognize patterns and logic on my own.

The challenge now is not finding the idea.

The challenge is expressing the idea correctly in Java.

LeetCode Journey Day: 6 🚀

# Personal Reflection - Day 7

Today was one of my strongest problem-solving days so far.

For all three problems, I was able to identify the correct logic very quickly. I did not struggle much with understanding what the problem was asking. Instead, most of my mistakes came from translating my thoughts into Java code.

## What I Noticed About Myself

I can usually recognize the pattern behind a problem now.

Examples from recent problems:

* Valid Anagram → Frequency Array Pattern
* First Unique Character → Frequency Array + Second Traversal
* Find First Occurrence in String → Nested Loop Search
* Rotate String → Pattern Recognition using Concatenation
* Jewels and Stones → Nested Loop Search + Break
* To Lower Case → Character Processing
* Defanging IP Address → Character Replacement

In most cases, I understand the logic before writing the code.

## Current Weakness

My biggest challenge is no longer finding the approach.

My biggest challenge is expressing the approach correctly in Java syntax.

Common examples:

* Using the correct index inside arrays.
* Remembering when to use `s.charAt(i)`.
* Knowing where to place statements inside or outside an `if` block.
* Accidentally returning too early.
* Forgetting that Strings are immutable.
* Translating a mental step into the exact Java statement required.
* Knowing when to use `break`, `continue`, or `return`.
* Converting a pattern in my head into working Java code.

Many times I know exactly what should happen, but I need a few attempts before I write it correctly.

## Improvement Compared to Earlier Days

Earlier:

```text
Problem
↓
Confusion about logic
↓
Confusion about code
```

Now:

```text
Problem
↓
Understand logic quickly
↓
Minor syntax/debugging mistakes
↓
Accepted solution
```

This is a big improvement because logic is usually harder to learn than syntax.

## Evidence From Recent Problems

### LeetCode 28 - Find the Index of the First Occurrence in a String

I understood that I needed nested loops and character comparison.

Mistakes were:

* Returning `-1` too early.
* Missing boundary conditions.
* Understanding when a complete match was found.
* Using incorrect indexes.

The algorithm was mostly correct. The mistakes were implementation details.

### LeetCode 796 - Rotate String

I quickly understood the rotation concept after seeing the pattern.

Main learning:

```java
(s + s).contains(goal)
```

The challenge was recognizing the hidden pattern, not coding complexity.

### LeetCode 242 - Valid Anagram

I successfully learned frequency arrays.

Biggest breakthrough:

```java
freq[s.charAt(i) - 'a']++;
freq[t.charAt(i) - 'a']--;
```

I now understand how characters can be converted into array indexes.

### LeetCode 387 - First Unique Character in a String

I immediately recognized another frequency-array problem.

The struggle was not the approach.

The struggle was correctly accessing the frequency array and performing the second traversal.

### LeetCode 709 - To Lower Case

I already knew the ASCII difference.

The challenge was:

* Storing converted characters.
* Building the answer string.
* Correct placement of statements.

### LeetCode 771 - Jewels and Stones

I correctly identified the need for nested loops.

The mistake was returning too early on mismatch.

After removing the unnecessary return statement, the solution became correct.

### LeetCode 1108 - Defanging an IP Address

I recognized the entire solution before writing code.

One loop.
One condition.
String building.

This was one of the cleanest solutions I wrote.

## Biggest Lesson From Day 7

I am starting to think like a programmer before writing code.

Instead of asking:

"What is the logic?"

I often ask:

"How do I express this logic in Java?"

That is a major improvement compared to earlier days.

## Pattern Recognition Growth

Patterns I can now recognize:

* Two Pointers
* Frequency Arrays
* Reverse Traversal
* String Matching
* String Building
* Character Processing
* Nested Loop Search
* Rotation Pattern
* Conditional Replacement

Instead of treating every problem as completely new, I am beginning to connect them with previously solved patterns.

## Focus For Day 8

* Improve Java syntax fluency.
* Reduce implementation mistakes.
* Become faster at converting logic into code.
* Practice frequency-array problems.
* Practice nested-loop search patterns.
* Continue building confidence in pattern recognition.

## Confidence Assessment

Logic Understanding: 9/10

Pattern Recognition: 8.5/10

Problem Approach Selection: 8.5/10

Java Syntax Confidence: 6.5/10

Overall Progress: Strong improvement compared to previous days.

## Final Day 7 Reflection

Today showed me that my biggest limitation is no longer problem-solving logic.

Most of the time I can identify the correct approach, pattern, or algorithm.

My current goal is to improve the speed and accuracy with which I convert those ideas into Java code.

That is a much better problem to have than not understanding the logic at all.

I am moving from:

```text
Learning Algorithms
```

to:

```text
Learning How To Express Algorithms In Java
```

and that is real progress.
See Yoou ON day 8
LOg out


Biggest Day 8 Observation

Today I noticed that I am becoming much better at recognizing patterns from previously solved problems.

For Power of Three, I immediately connected it with Power of Two.

Instead of learning a completely new solution, I only had to modify an existing pattern.

This is the first time I strongly felt that solving previous problems is helping me solve new ones faster.

Personal Reflection

Today I learned an important difference:

Knowing the operation
≠
Knowing the stopping condition

In Power of Two, my division logic was correct from the beginning.

The real bug was deciding when to stop.

I also learned that Binary Search is much more powerful than I originally thought.

It is not just for searching elements.

It can also search for answers.

Confidence

Logic Understanding: 9/10

Pattern Recognition: 9/10

Java Syntax Confidence: 7/10

Binary Search Understanding: 7.5/10

Overall Progress: Strong

Final Day 8 Reflection

Earlier I focused mostly on solving one problem at a time.

Today I started recognizing relationships between problems.

I am beginning to build a library of patterns in my mind:

Two Pointers
Frequency Arrays
Reverse Traversal
String Building
Nested Loop Search
Binary Search
Repeated Division

This makes new problems feel less like completely new challenges and more like variations of patterns I already know.

Total Problems Solved Today: 3

LeetCode Journey Day: 8 🚀

SEE YOU ON DAY 9 
LOG OUT..


# DAY 9 DOCUMENTATION

**Date:** 25-07-2026

Today felt different compared to my earlier LeetCode days.

The biggest change I noticed is that I am no longer struggling to understand the core logic of most Easy problems. Instead, I am starting to recognize patterns from previously solved questions and reuse them.

For the first time, I looked at a new problem and immediately connected it to a pattern I had already learned.

Example:

```text
LeetCode 367 - Valid Perfect Square
↓
Looked familiar
↓
Connected it to
LeetCode 69 - Sqrt(x)
↓
Realized both use Binary Search
↓
Solved using the same pattern
```

This was probably the biggest achievement of today.

Earlier in my journey, every new problem felt completely different. Now I am beginning to see that many problems are actually small variations of the same underlying pattern.

---

## Problems Solved

- LeetCode 507 - Perfect Number
- LeetCode 202 - Happy Number
- LeetCode 263 - Ugly Number
- LeetCode 367 - Valid Perfect Square

---

## What I Learned Today

### 1. Pattern Recognition Is Improving

Instead of thinking:

```text
New Problem
↓
Need New Algorithm
```

I am starting to think:

```text
New Problem
↓
Which pattern does this belong to?
```

This mindset helped me solve Valid Perfect Square very quickly because I immediately recognized the Binary Search pattern.

---

### 2. Repeated Division Pattern Is Becoming Natural

After solving:

```text
Power of Two
Power of Three
Ugly Number
```

I noticed all of them share the same idea:

```text
Repeated Division
↓
Reduce Number
↓
Check Final Value
```

I am becoming more comfortable identifying mathematical patterns.

---

### 3. Happy Number Introduced A New Concept

Happy Number was the first problem where I realized:

```text
A process can continue forever.
```

My logic for generating the next number was correct, but I got TLE because I did not know how to detect cycles.

This introduced me to:

```text
HashSet
Cycle Detection
```

Even though I had not learned HashSet before, I was able to understand why it was needed.

This was an important lesson because the problem was no longer about syntax or loops—it required a completely new concept.

---

### 4. My Current Bottleneck

A few days ago my biggest struggle was:

```text
Understanding the problem logic.
```

Now I feel my biggest struggle is:

```text
Expressing the logic correctly in code.
```

Many times I can already see the solution pattern in my head, but I still make mistakes while converting that idea into Java syntax.

Examples of recurring issues:

- Wrong stopping conditions.
- Returning too early.
- Writing conditions in the wrong place.
- Small indexing mistakes.
- Forgetting where a check should happen.

The good part is that these are implementation mistakes, not logic mistakes.

---

## Personal Reflection

Today gave me confidence that my problem-solving ability is improving.

The strongest evidence was:

```text
LeetCode 367
↓
Recognized Binary Search instantly
```

A few weeks ago I would have treated it as a completely new problem.

Now I am starting to see patterns instead of isolated questions.

That feels like real progress.

---

## Biggest Learning Of Day 9

```text
Most Easy LeetCode problems are not about learning
new algorithms.

They are about recognizing an old pattern
inside a new problem.
```

I still have a lot to improve in coding syntax and implementation, but my pattern recognition and logical thinking are becoming much stronger.

This is the first time I genuinely felt that I am starting to think like a problem solver instead of just trying to memorize solutions.


SEE YOU ON DAY 10,
LOG OUT...🚀


# DAY 10 DOCUMENTATION

**Date:** 26-07-2026 (Sunday)

## Problems Solved

- LeetCode 3658 — GCD of Odd and Even Sums

---

## Why I Solved Only One Problem Today

Today I intentionally solved only one LeetCode problem.

The reason was not lack of motivation or consistency.

Instead, I decided to prepare for my next learning topic:

```text
HashMap
```

Over the last few days I encountered my first problem that required a new data structure:

```text
LeetCode 202 — Happy Number
```

While solving it, I realized that my current bottleneck is no longer basic loops or conditions.

The next step in my journey is understanding:

```text
HashSet
HashMap
```

properly.

Because of that, I chose to spend time revising concepts instead of rushing through multiple LeetCode problems.

---

## Problem Solved

### LeetCode 3658 — GCD of Odd and Even Sums

### Biggest Learning

At first, the problem looked like it would require:

```text
Generate odd numbers
↓
Generate even numbers
↓
Calculate sums
↓
Find GCD
```

But after observing the mathematical pattern, the entire problem simplified into:

```java
return n;
```

This was a reminder that:

```text
Not every problem requires loops.
Not every problem requires simulation.
```

Sometimes:

```text
Pattern Recognition
>
Implementation
```

---

## What I Learned Today

### 1. Observation Can Eliminate Code

Earlier in my journey I would immediately start thinking:

```text
Which loop should I use?
```

Today the solution came from:

```text
Understanding the mathematics
```

instead of writing more code.

---

### 2. Preparation Is Also Progress

Today reinforced an important lesson:

```text
Learning is not only solving questions.
```

Sometimes progress comes from:

```text
Revising concepts
Understanding weak areas
Preparing for the next topic
```

and that is exactly what I chose to do today.

---

### 3. Next Focus Area

My next topic is:

```text
HashMap
```

Goals before moving deeper into HashMap:

- Understand HashSet properly.
- Learn storing key-value pairs.
- Learn frequency counting using HashMap.
- Learn lookup operations.
- Learn when arrays stop being enough and HashMap becomes necessary.

---

## Personal Reflection

Compared to the beginning of my journey:

```text
Day 1
↓
Struggled with logic and syntax
```

Now I feel:

```text
Logic Recognition
↑
Pattern Recognition
↑
Confidence
↑
```

Most of my mistakes are no longer about understanding the problem.

Instead, they are usually:

```text
Syntax
Implementation Details
New Data Structures
```

which is a very different type of challenge.

---

## Day 10 Overall Lesson

```text
Solving fewer questions is okay
if the day is spent strengthening fundamentals.
```

Today's focus was not quantity.

Today's focus was:

```text
Understanding
Preparation
Building foundations for HashMap
```

and that is still meaningful progress in my learning journey.


SEE YOU ON 11
LOG OUT...🚀

# DAY 11 DOCUMENTATION

**Date:** 27-07-2026

## Problems Solved

- LeetCode 217 — Contains Duplicate
- LeetCode 20 — Valid Parentheses

---

## Why Today Was Important

Today was not about solving many questions.

Today was about learning two completely new and extremely important data structures:

```text
HashSet
Stack
```

For the first time, I started seeing that many LeetCode problems are not solved by loops alone.

Instead:

```text
Problem
↓
Recognize Pattern
↓
Choose Data Structure
↓
Implement
```

---

# LeetCode 217 — Contains Duplicate

## My Initial Thinking

The first idea was:

```text
Compare every element with every other element
↓
Find duplicate
```

which naturally leads to:

```text
Nested Loops
```

and:

```text
O(n²)
```

time complexity.

---

## What I Learned

I learned that:

```text
HashSet stores only unique values.
```

This means:

```text
Have I seen this number before?
```

can be checked very quickly.

Instead of repeatedly searching the array:

```text
Store
↓
Check
↓
Continue
```

---

## New Concepts Learned

```java
HashSet<Integer> set = new HashSet<>();
```

Operations:

```java
set.add()
set.contains()
```

I also reinforced:

```java
for(int num : nums)
```

and understood its expanded form.

---

## Biggest Learning

```text
HashSet is useful whenever I need to know:

"Have I seen this before?"
```

This is my first solid HashSet problem.

---

# LeetCode 20 — Valid Parentheses

## My Initial Understanding

The problem looked simple:

```text
Opening brackets
Closing brackets
Match them
```

But after analyzing examples, I noticed:

```text
Last Opened
↓
First Closed
```

which follows:

```text
LIFO
```

and therefore:

```text
Stack
```

---

## What I Learned

For the first time I used:

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

## Important Realization

The problem is not about counting brackets.

It is about remembering:

```text
Which bracket was opened most recently.
```

Example:

```text
([{}])

Push (
Push [
Push {

Pop {
Pop [
Pop (
```

Valid.

---

## Biggest Learning

Today I learned a very important interview pattern:

```text
Last Opened
↓
First Closed
↓
STACK
```

Whenever I see:

```text
Parentheses
Nested Structures
Matching Symbols
```

I should think:

```text
Stack
```

---

# Overall Reflection

Today felt different from previous days.

Most of my earlier learning focused on:

```text
Loops
Conditions
Arrays
Math
```

Today introduced:

```text
Data Structures
```

which is a major step forward.

---

## What I Realized About Myself

Earlier my thought process was:

```text
Read Problem
↓
Think About Code
```

Now it is slowly becoming:

```text
Read Problem
↓
Find Pattern
↓
Choose Data Structure
↓
Write Code
```

This is a huge improvement compared to where I started.

---

## Day 11 Overall Lessons

### HashSet Pattern

```text
Seen Before?
↓
Yes → Duplicate
↓
No → Store
```

Used In:

```text
Contains Duplicate
```

---

### Stack Pattern

```text
Last Opened
↓
First Closed
```

Used In:

```text
Valid Parentheses
```

---

## Biggest Learning Of The Day

```text
The correct data structure can make a difficult problem feel easy.
```

Today was not about quantity.

It was about learning two foundational tools:

```text
HashSet
Stack
```

that will appear again and again in future LeetCode problems.
## Additional Day 11 Reflection

Today I also looked at the LeetCode Daily Question.

At first, I was not sure whether I was fully ready for daily problems yet because I am still learning new topics like:

```text
HashSet
Stack
HashMap (next topic)
```

and building my problem-solving skills step by step.

However, when I saw today's Daily Question, it felt approachable and easier than I expected.

That gave me an important realization:

```text
Sometimes I feel I am not ready,
but the only way to know is to try.
```

So instead of skipping it, I decided to attempt it and give my best effort.

Even if I cannot solve every Daily Question right now, attempting them helps me:

```text
Read new problem types
↓
Practice pattern recognition
↓
Test my current level
↓
Learn new approaches
```

This mindset is important because:

```text
Growth does not happen by waiting until I feel ready.

Growth happens by attempting challenges
even when I am unsure.
```

### Personal Observation

A few weeks ago, many LeetCode questions looked impossible.

Now, after learning patterns like:

```text
Binary Search
Repeated Division
HashSet
Stack
Largest & Second Largest Tracking
```

I can at least understand the problem, think of an approach, and attempt a solution.

That itself is progress.

### Commitment

Going forward:

```text
I will continue solving Daily Questions whenever possible.

I may not solve every one of them.

I may get stuck.

I may need hints.

But I will always try first and give my best effort.
```

### Day 11 Final Thought

```text
I do not need to be ready for every challenge.

I only need to be willing to attempt it.

Each attempt teaches me something,
whether I solve the problem or not.
```

SEE YOU ON DAY 12...🚀


# Binary Search Documentation

## Overview

Binary Search is an efficient searching algorithm used to reduce the search space by half in every step.

Instead of checking every element one by one, Binary Search checks the middle element and decides which half of the search space can be ignored.

Time Complexity:

O(log n)

Space Complexity:

O(1)


---

# How Binary Search Works

Binary Search requires a condition where after checking the middle element, we can eliminate half of the possible answers.

Steps:

1. Find the middle element.
2. Compare it with the required condition.
3. Decide whether to search left or right.
4. Repeat until the answer is found.


Formula:

mid = start + (end - start) / 2


---

# Binary Search Patterns Learned


## 1. Normal Binary Search

Used when finding an element in a sorted array.

Example:

Search target in:

[1,3,5,7,9]


If:

target > mid

Search right half


If:

target < mid

Search left half



---

# 2. Binary Search on Answer

Sometimes we are not searching for an element.

We search for the first position where a condition becomes true.

Pattern:

False False False True True True

Goal:

Find the first True.


Example:

## LeetCode 278 - First Bad Version


Concept:

Versions before bad version:

false


Bad version and after:

true


Binary Search helps find the first bad version efficiently.



---

# 3. Binary Search with Conditions


Example:

## LeetCode 374 - Guess Number Higher or Lower


Instead of checking every number:

1 2 3 4 5 6 7 8 9


Check middle value.


If number is higher:

Search left.


If number is lower:

Search right.


If correct:

Return answer.



---

# 4. Mountain Array Binary Search


Example:

## LeetCode 852 - Peak Index in a Mountain Array


Mountain array structure:

Increasing → Peak → Decreasing


Example:

[0,2,5,10,6,3,1]


Peak:

10


Instead of finding maximum using O(n),

we use Binary Search.



## Logic


Compare:

arr[mid]

and

arr[mid+1]



### Case 1:

arr[mid] < arr[mid+1]


Meaning:

We are on increasing side.


Peak exists on the right.


Move:

start = mid + 1



---

### Case 2:

arr[mid] > arr[mid+1]


Meaning:

We are on decreasing side.


Peak is at mid or left.


Move:

end = mid



---

# How to Recognize Binary Search Problems


Look for:

- O(log n) requirement
- Sorted array
- Increasing/decreasing pattern
- Finding minimum/maximum
- Finding first or last occurrence
- Finding peak element
- Search space reduction


Main Question:

"After checking the middle, can I remove half of the possibilities?"

If yes:

Think Binary Search.


---

# Common Mistakes


## 1. Confusing Maximum Value and Index

Example:

arr = [0,10,5,2]


Maximum value:

10


Peak index:

1


Problem may ask for index, not value.



## 2. Wrong Direction

In mountain array:


arr[mid] < arr[mid+1]

means:

Move right


arr[mid] > arr[mid+1]

means:

Move left



## 3. Wrong Mid Calculation


Wrong:

mid = start + (end=start)/2


Correct:

mid = start + (end-start)/2



Reason:

Using '=' assigns a value.

Using '-' calculates the distance.



---

# Key Learning

Binary Search is not only for finding numbers.

It is a technique to reduce a problem's search space by half.

The main skill is recognizing:

"Can one decision eliminate half of the choices?"

SEE YOU ON DAY 13...🚀


## Why Only One Problem Today?

Today was a travel day, and I was physically tired after travelling.

Because of that, I did not have the same energy or focus level that I normally have for solving multiple LeetCode problems.

Instead of forcing myself to solve many questions with low concentration, I decided to solve one problem properly and understand its logic completely.

Problem Solved:

- LeetCode 1539 — Kth Missing Positive Number

Although the number of questions solved was lower than usual, I still maintained consistency and continued my learning streak.

### Personal Reflection

```text
Some days are high-output days.
Some days are low-output days.

What matters most is staying consistent.
```

Today was not about quantity.

It was about:

```text
Showing up
↓
Learning something new
↓
Maintaining momentum
```

Even solving one problem is better than breaking the habit completely.

### Day 13 Final Thought

```text
I was tired because of travelling,
but I still solved a problem and learned a new pattern.

Progress may be slow on some days,
but consistency keeps the journey moving forward.
```

SEE YOU ON DAY 14...🚀


# DAY 14 LEARNING LOG

**Date:** 30-07-2026

## Activities Completed

### 1. Learned LinkedIn Basics
Today I spent some time understanding the fundamentals of LinkedIn.

Topics explored:

- Purpose of LinkedIn
- Professional networking
- Building an online presence
- Importance of maintaining a professional profile
- How LinkedIn can help with internships, jobs, and career growth

This was not coding-related but is an important step toward future professional development.

---

## LeetCode 206 — Reverse Linked List

### Initial Challenge

This was my first serious Linked List problem.

At first, I was trying to solve it like an array problem.

My initial thinking included:

```java
head.length
head[i]
```

which made me realize that Linked Lists are fundamentally different from arrays.

---

### Concepts Learned

#### Linked List Structure

A node contains:

```java
value
next
```

Example:

```text
1 -> 2 -> 3 -> null
```

Each node stores a value and a reference to the next node.

---

#### Linked List vs Array

Array:

```java
arr[i]
arr.length
```

Linked List:

```java
node.next
```

No direct indexing is possible.

---

### Main Pattern Learned

Three Pointer Technique:

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

### Reverse Process

Pattern:

```java
next = curr.next;
curr.next = prev;
prev = curr;
curr = next;
```

Logic:

```text
Save next node
↓
Reverse current link
↓
Move pointers
↓
Repeat
```

---

### Biggest Breakthrough

Understanding:

```java
curr.next = prev;
```

Initially this looked confusing.

After visualizing each step, I understood that this line actually reverses the direction of the link.

Example:

Before:

```text
1 -> 2 -> 3
```

After first reversal:

```text
1 -> null
```

This is the core operation behind linked list reversal.

---

### Important Realization

When the loop ends:

```java
curr == null
```

The fully reversed list is pointed to by:

```java
prev
```

Therefore:

```java
return prev;
```

---

### Key Learning

Today I learned that Linked Lists require a completely different mindset from arrays.

This problem introduced me to pointer manipulation and helped me understand how references move inside a linked list.

---

## LeetCode 315 — Count of Smaller Numbers After Self

### My Approach

I successfully derived a brute-force solution using nested loops.

Logic:

```text
For every element
↓
Check all elements on its right
↓
Count smaller values
↓
Store count
```

Example:

```text
nums = [5,2,6,1]

5 → 2
2 → 1
6 → 1
1 → 0

Output = [2,1,1,0]
```

---

### What Went Well

I was able to understand the problem independently and build a logically correct solution.

This confirmed that my problem understanding was correct.

---

### Issue Faced

Although the solution produced correct output, it received:

```text
TLE (Time Limit Exceeded)
```

Reason:

```text
Time Complexity = O(n²)
```

The nested loops become too slow for large inputs.

---

### Biggest Lesson

Today I learned:

```text
A solution can be correct
but still fail due to efficiency constraints.
```

Correctness and optimization are two separate skills.

---

### New Awareness

This problem introduced me to advanced techniques that I have not studied yet:

```text
Merge Sort Counting
Fenwick Tree (Binary Indexed Tree)
Segment Tree
```

I now understand why advanced algorithms are necessary for some Hard problems.

---

## Overall Reflection

Today was less about solving many problems and more about understanding deeper concepts.

Major takeaways:

```text
Learned LinkedIn basics
↓
Learned Linked List fundamentals
↓
Understood pointer manipulation
↓
Experienced the difference between correctness and efficiency
```

Even though I solved only a few problems, today's learning was highly valuable because it introduced completely new concepts.

---

## Day 14 Final Thought

```text
Today taught me that growth is not measured only by the number of questions solved.

Sometimes understanding a new data structure,
learning a new pattern,
or realizing why a solution fails
is more valuable than solving many easy questions.

I learned my first major Linked List pattern today
and understood that optimization is a skill that develops over time.
```


SEE YOU ON DAY 15...🚀

# DAY 15 LEARNING LOG

**Date:** 31-07-2026

## Today's Progress

Today I solved:

- LeetCode 21 — Merge Two Sorted Lists
- LeetCode 33 — Search in Rotated Sorted Array

---

## LeetCode 21 — Merge Two Sorted Lists

### My Initial Thought

When I saw the problem, I was not worried about comparing values because I already understood the basic logic.

The confusing part was:

```text
How do I create a completely new linked list
while moving through two existing linked lists?
```

Since I recently started learning Linked Lists, I still think like an array programmer.

Whenever I see a Linked List problem, my brain still tries to find:

```java
arr[i]
length
indexes
```

which obviously do not exist.

---

### What Frustrated Me

The Dummy Node concept felt strange at first.

I kept thinking:

```text
Why create a fake node?
Why not directly create the answer list?
```

After visualizing it multiple times, I finally understood that the dummy node only makes handling the first element easier.

---

### What I Learned

Today I learned another important Linked List pattern:

```text
Dummy Node
+
Tail Pointer
```

I am slowly becoming comfortable with pointers and references.

---

## LeetCode 33 — Search in Rotated Sorted Array

### My Initial Thought

The moment I saw:

```text
O(log n)
```

I immediately knew:

```text
Binary Search
```

should be involved.

That was a good sign because a few days ago I probably would not have recognized that immediately.

---

### Where I Got Stuck

I kept trying to think about the problem using normal Binary Search.

My thinking was:

```java
nums[mid] < target
```

But the array was rotated, so the usual binary search logic did not work.

I was confused because:

```text
The array looked unsorted,
yet the problem still expected O(log n).
```

---

### Breakthrough Moment

The biggest realization was:

```text
Even if the entire array is not sorted,
one half is always sorted.
```

Once I understood that idea, everything started making sense.

After that, the problem became:

```text
Find sorted half
↓
Check if target is inside it
↓
Search there
```

instead of normal binary search.

---

## Personal Thoughts

Today felt less frustrating than some previous days.

I noticed something encouraging:

```text
I am starting to recognize patterns faster.
```

For example:

```text
O(log n)
→ Binary Search

Linked List
→ Pointer manipulation
```

A few weeks ago, I would immediately think:

```text
How do I code this?
```

Now I am starting to ask:

```text
What pattern does this problem belong to?
```

which feels like real progress.

---

## Challenges Faced

- Still not fully comfortable with Linked Lists.
- Still need visual explanations to understand pointer movement.
- Sometimes I jump into coding before fully understanding the logic.
- Rotated Binary Search took time because I was stuck in normal Binary Search thinking.

---

## What Made Me Happy Today

I recognized Binary Search on my own when I saw:

```text
O(log n)
```

That felt good because it shows I am slowly building intuition.

---

## Day 15 Reflection

Today was not about learning new syntax.

It was about learning how to think differently.

I learned that:

```text
Not every Binary Search problem looks sorted.

Not every Linked List problem is about values.

Sometimes the real challenge is identifying
the underlying pattern.
```

I still have a long way to go, but today I felt that my problem-solving mindset improved a little.

SEE YOU ON DAY 16...🚀

# DAY 16 LEARNING LOG

**Date:** 01-08-2026

## Today's Activity

Today was a busy day because I was outside for work and had very limited time for coding.

Because of this, I could not dedicate a long study session to LeetCode or learn a new topic in depth.

However, I did not want to break my consistency streak, so I made sure to solve at least one problem.

---

## Problem Solved

### LeetCode 1688 — Count of Matches in Tournament

### Difficulty

Easy

---

## Thought Process

Since I was short on time and energy, I decided not to force myself into solving a difficult problem.

Instead, I chose a problem that I could complete quickly while still keeping my coding habit alive.

My goal today was:

```text
Stay consistent.
Do not break the streak.
Keep showing up.
```

---

## Concepts Reinforced

### Simulation

The problem was mainly based on simulating tournament rounds and counting matches.

### Problem Reading

I practiced understanding the problem statement carefully before writing code.

### Consistency Mindset

Today's biggest lesson was not technical.

It was:

```text
Even one solved problem is better than solving none.
```

---

## Challenges Faced

- Limited time due to work.
- Physical tiredness.
- Very little energy left for long coding sessions.
- Temptation to skip coding for the day.

---

## What I Learned Today

### Small Progress Still Counts

Today reminded me that:

```text
Consistency is more important than intensity.
```

Some days will be:

```text
3-4 LeetCode problems
Learning new concepts
Deep problem solving
```

And some days will be:

```text
One simple problem
Protect the streak
Keep moving forward
```

Both types of days are important.

---

## Personal Reflection

Initially, I thought about skipping coding because I was tired and busy.

But then I realized:

```text
The purpose of building a habit
is to continue even when conditions are not perfect.
```

So I completed one problem and maintained the streak.

That itself feels like a small victory.

---

## Day 16 Final Thought

```text
Today was not about learning a difficult algorithm.

Today was about discipline.

I learned that consistency is built on ordinary days,
not only on productive days.

One problem completed.
One more day added to the journey.
Streak continues.
```

SEE YOU ON DAY 17...🚀

# DAY 17 — 02 AUGUST 2026

Today was honestly another difficult day.

I spent almost the entire day outside and by the time I got home, I was tired both physically and mentally.

For most of the day, I wasn't even thinking about coding. I was thinking about whether I would have enough time to keep my streak alive.

At one point I genuinely considered skipping coding for the day.

Not because I didn't want to learn, but because I simply felt exhausted.

Still, I kept thinking about the streak I have built over the last few weeks.

I knew that if I solved even one problem, I could go to sleep knowing that I showed up.

So instead of aiming for a big achievement, I changed the goal.

The goal became:

"Just solve one question."

That decision immediately removed pressure from my mind.

---

I picked LeetCode 349 (Intersection of Two Arrays).

At first the problem looked simple, but I quickly realized that I did not know much about HashSet.

While solving it, I made several small mistakes.

I accidentally stored indexes instead of values.

I forgot that a HashSet is not the same thing as an array.

I also got stuck thinking about how to return the final answer.

Normally these small mistakes would have frustrated me.

But today I was actually happy to make them because every mistake taught me something new about Java.

For the first time, HashSet stopped feeling like a theory topic and started feeling like a useful tool.

By the end of the problem I felt like I had unlocked a new weapon that I could use in future questions.

---

The funniest moment of today was LeetCode 877.

I expected a complicated solution.

When I saw the problem, I thought:

"This definitely looks like DP."

Then I discovered that the accepted solution is literally:

return true;

I laughed when I saw that.

It reminded me that sometimes understanding the problem is more important than writing complex code.

---

Today was not a productive day in terms of quantity.

I solved very little.

But I am still proud of today.

Because on days when motivation is high, coding is easy.

The real challenge is coding when you're tired, busy, and tempted to skip.

Today I won that battle.

Not against LeetCode.

Against myself.

And honestly, that feels like the bigger victory.

- Bhavya

OUT.....DAY 18


# DAY 18 — 03 AUGUST 2026

Today felt much more like a learning day than a grinding day.

I wasn't chasing the number of questions solved. Instead, I spent more time understanding how certain concepts actually work.

The biggest realization today was that I am slowly starting to see patterns instead of just solving problems.

---

The first problem I worked on was LeetCode 744.

At first glance, it looked like another Binary Search question.

Normally when I see Binary Search, my brain immediately thinks:

"Find the target."

But today I learned that Binary Search is much bigger than that.

The target itself wasn't important.

The real goal was:

```text
Find the smallest element greater than the target.
```

That completely changed my thinking.

For the first time, I felt like I was using Binary Search as a tool to find a position rather than a specific value.

The wrap-around logic was also interesting.

When I finally understood why:

```java
st % letters.length
```

works, it felt satisfying because the solution suddenly became very elegant.

The best part was that I didn't directly jump to the answer.

I slowly understood:

- Why we move left
- Why we move right
- Why we don't actually need an answer variable
- Why `st` itself becomes the answer position

That felt like genuine growth.

---

The second problem was Fibonacci.

This problem looked simple, but it introduced me to something important:

```text
Recursion
```

For a long time recursion felt mysterious whenever I saw it.

Today I finally understood the basic idea:

```text
Solve a smaller version
of the same problem.
```

Instead of trying to understand the entire recursion tree at once, I focused on one thing:

```text
What is the smallest problem?
```

That question made everything easier.

Once I understood the base case:

```java
if(n <= 1)
{
    return n;
}
```

the rest of the solution started making sense.

For the first time, recursion felt understandable rather than scary.

---

One thing I noticed today is that my thinking is slowly changing.

A few weeks ago, I was mostly focused on syntax.

I would get stuck on:

```text
length vs length()
char vs String
Array vs ArrayList
```

Now I still make mistakes, but more of my attention is going toward:

```text
Why does this algorithm work?
Why are we moving left?
Why are we moving right?
Why does recursion stop?
```

That feels like progress.

---

Today wasn't a huge achievement day.

I didn't solve difficult problems.

I didn't learn an advanced algorithm.

But I strengthened two very important foundations:

```text
Binary Search
Recursion
```

And those foundations will be useful for hundreds of future problems.

---

## Important Concepts Added Today

```text
Binary Search can find positions,
not only exact targets.

Smallest Greater Element pattern.

Wrap-around indexing using:

st % length

Recursion Basics.

Base Case.

Recursive Calls.

Breaking large problems into
smaller versions of themselves.
```

---

## Personal Reflection

Today felt like one of those days where growth is not obvious from the number of questions solved.

But I can feel my understanding getting deeper.

I am slowly moving from:

"I know the syntax."

to

"I understand the idea."

And that is probably the most important shift in my DSA journey so far.

🚀 Day 18 Completed.

OUT...DAY 19...🚀


# Day 19 — August 4, 2026

## Today's Reality

Today wasn't one of those days where I solved a bunch of problems and felt unstoppable.

I spent most of my time trying to truly understand recursion instead of just copying solutions. At multiple points, I felt confused, especially while working on **Pow(x, n)**. What looked like a simple problem turned into a deep lesson about how recursion actually works.

There were moments where I thought I understood the solution, but the moment I tried implementing it myself, I got stuck. Negative powers, recursive calls, overflow issues, and even Java syntax started mixing together in my head.

Instead of rushing to finish the problem, I slowed down and focused on understanding *why* each step existed.

## Problems Worked On

* 50. Pow(x, n)
* 342. Power of Four

## What Made Today Different

The biggest win wasn't solving a problem.

The biggest win was realizing that recursion is not magic.

For the first time, I started seeing recursion as:

1. Define a base case.
2. Reduce the problem.
3. Trust the smaller answer.
4. Build the final answer from it.

This mindset helped me understand both problems much better.

## Frustrations

* Got confused between mathematical expressions and Java syntax.
* Mixed negative exponent logic with recursive logic.
* Struggled to understand why accepted solutions use `long` instead of `int`.
* Kept trying to fix code before fully understanding the underlying idea.

There were moments where everything felt mixed up and I genuinely felt stuck.

## Small Wins

* Understood Fast Power / Binary Exponentiation.
* Understood why solving half the problem is enough.
* Understood the difference between even and odd exponent handling.
* Successfully built a recursive solution for Power of Four on my own.
* Learned an important overflow edge case involving `Integer.MIN_VALUE`.

## Mindset Check

Today reminded me that learning DSA isn't about collecting solved questions.

It's about reaching the point where the logic starts making sense.

Some days the progress is visible through accepted submissions.

Other days the progress is invisible and happens through confusion, mistakes, and persistence.

Today was definitely the second type of day.

## Streak Status

Day 19 completed.

Not the cleanest day.
Not the fastest day.

But definitely a valuable one.

OUT...DAY 20..🚀

# 📖 Day 20 Documentation (08-05-2026)

Today felt different.

Instead of rushing to code, I spent more time trying to understand the pattern behind each problem. I noticed that whenever I slowed down and asked myself *"What is this problem actually asking?"*, the solution became much clearer.

The **Ransom Note** problem taught me not to think about whether a character simply exists, but whether enough copies of that character exist. That small shift in thinking helped me understand why frequency arrays are so useful.

The **Number of Segments in a String** problem was another interesting lesson. My first instinct was to count spaces, but I quickly realized that spaces don't determine the answer—**the beginning of each word does**. That completely changed the way I approached the problem.

The **Detect Capital** problem challenged my logic more than my coding. I initially wanted to check every character without a clear plan, but after thinking about the valid capitalization patterns, I realized that breaking the problem into different cases made everything much simpler.

One thing I noticed today is that I am becoming more patient. A few days ago, I would have immediately asked for the solution whenever I got stuck. Today, I kept thinking, asking questions, and correcting my own logic until I finally reached the solution myself.

I also made mistakes today:

* I forgot Java operator precedence and learned why parentheses are important.
* I tried to return too early inside loops.
* I focused on checking individual characters before deciding the overall pattern.

Instead of getting frustrated, I treated each mistake as a clue that helped me understand the problem better.

The biggest improvement I noticed is in my mindset.

Earlier, I mostly thought:

> "How do I write this code?"

Today, I found myself thinking:

> "What pattern is this problem following?"

That feels like real progress.

I know I'm still making mistakes, but they are becoming more logical mistakes than syntax mistakes, and that tells me I'm moving in the right direction.

Every problem I solve now feels a little less about memorizing solutions and a little more about learning how to think.

**Day 20 complete. 

Documentation (06-08-2026)

Today was one of those days where I realized that understanding a concept is much more valuable than simply getting the correct answer.

The first problem, **Move Zeroes**, completely changed the way I think about the Two Pointer technique.

At first, I was convinced that "two pointers" meant using two nested loops. I kept trying to build my solution around that idea because it felt natural. But after thinking through the problem step by step, I realized that two pointers are simply two variables with different responsibilities.

One pointer scans the array, while the other remembers where the next valid element should go.

That small realization completely changed my perspective.

I also learned that there can be multiple correct approaches to the same problem. Initially, I wanted to solve the problem using only swapping because that was the first idea that came to my mind. Later, I understood that copying values forward is also a valid solution, and that both approaches solve the same problem in different ways.

The second problem, **Smallest Divisible Digit Product I**, reminded me that not every problem requires a clever trick. Sometimes, the simplest brute-force solution is exactly what the problem expects.

Instead of trying to overcomplicate the logic, I simply checked every number one by one until I found the answer.

While solving it, I revised one of the most important number manipulation patterns:

* Extract the last digit using `% 10`.
* Remove the last digit using `/ 10`.

I also learned why creating a copy of a number is important before modifying it.

Another interesting lesson today came from Java itself.

For the first time, I encountered the **"Unreachable statement"** compiler error. At first, I was confused because I thought every method should end with a `return` statement.

After understanding the program flow, I realized that my infinite loop already guaranteed a return statement inside it, making the final return impossible to execute.

That was a nice reminder that the compiler doesn't just check syntax—it also understands logic.

The biggest improvement I noticed today was in my thinking process.

Earlier, I often focused on writing code as quickly as possible.

Today, I spent much more time asking myself:

* What is the role of each variable?
* What is each pointer responsible for?
* What pattern is hidden inside this problem?

That small change made the coding part much smoother.

Looking back, I can clearly see that my confidence is improving. I still make mistakes, but they are becoming smaller and easier to identify.

Every day, I'm relying a little less on memorizing solutions and a little more on understanding patterns.

That's exactly the kind of progress I wanted when I started this journey.

**Day 21 Complete.**
# 📖 Day 22 Documentation (07-08-2026)

Today was different from my previous practice sessions because I started learning an entirely new topic: **Bit Manipulation**.

The first problem, **Find the Difference**, looked like a new type of string problem. My first instinct was to think about different approaches, but after analyzing it carefully, I realized something important.

It was actually the same frequency-array pattern that I had already used while solving **Ransom Note**.

Instead of learning a completely new algorithm, I simply reused an existing one.

That made me realize that many LeetCode problems are just different stories built around the same core idea.

While solving it, I also learned that once I know the answer, I don't always need to finish traversing the entire data structure.

As soon as a character's frequency became negative, I already knew it was the extra character, so returning immediately made the solution simpler and more efficient.

The second part of today's learning was much more interesting.

I started studying **Bit Manipulation** for the first time.

Initially, binary numbers looked confusing because I always thought in decimal.

After understanding that computers only work with **0s and 1s**, things slowly started making sense.

I learned the basic bitwise operators:

* AND (`&`)
* OR (`|`)
* XOR (`^`)
* NOT (`~`)

Among them, XOR immediately stood out because of its unique property:

* Same bits become `0`
* Different bits become `1`

I also learned some useful identities like:

* `a ^ a = 0`
* `a ^ 0 = a`

These identities are used in many DSA and interview problems.

While studying **Number Complement**, I initially believed that simply using the NOT operator (`~`) would solve the problem.

Later, I discovered that Java stores integers using **32 bits**, which means applying `~` flips every single bit, including the leading zeros that are not part of the number's actual binary representation.

That introduced me to a completely new concept called a **mask**.

Although I haven't fully mastered masks yet, I now understand why they are needed.

A mask allows us to flip only the meaningful bits instead of all 32 bits.

Another thing I learned today was that Java already provides utility methods like:

```java
Integer.numberOfLeadingZeros(num)
```

Although I don't want to depend on built-in methods before understanding the concept manually, it's good to know these utilities exist.

The biggest lesson from today wasn't about coding.

It was about recognizing patterns.

Earlier, every new problem felt like a completely new challenge.

Now I'm slowly starting to ask myself:

* Have I solved something similar before?
* Can I reuse an existing pattern?
* Is this really a new algorithm, or just a new application of an old one?

That mindset is helping me think more like a problem solver instead of someone who memorizes solutions.

Today's learning also marked the beginning of Bit Manipulation, a topic I had always avoided because it looked complicated.

After today's session, it doesn't feel scary anymore—it just feels like another pattern that I'll understand with enough practice.

**Day 22 Complete.**

# 📖 Day 23 — DSA Journey Documentation

**Date:** 08-08-2026

Today I solved two Easy LeetCode problems: **121. Best Time to Buy and Sell Stock** and **392. Is Subsequence**.

The first problem taught me an important lesson about arrays: sometimes simply finding the minimum and maximum value is not enough. The **order of elements matters**.

Initially, I was thinking about keeping a `max` and `min` value and calculating their difference. But I realized that this could break the condition of the problem because the minimum price must come **before** the selling price.

For example, in `[7,6,4,3,1]`, the maximum value is `7` and the minimum value is `1`, but using them together would mean selling before buying.

I changed my thinking to:

> "While moving from left to right, what is the cheapest price I could have bought at until today?"

I maintained two variables:

```java
int minPrice = prices[0];
int maxProfit = 0;
```

For every new price, I checked whether it was a new minimum. If it was, I updated `minPrice`. Otherwise, I calculated the profit I could make by selling on that day and compared it with the best profit found so far.

This introduced me to a useful pattern:

**Minimum so far + maximum result so far.**

The second problem, **392. Is Subsequence**, reinforced the **two-pointer pattern**.

At first, I wasn't completely sure how to handle the two strings. I eventually understood that I only need to scan through `t` while keeping a pointer `j` for the next character I need from `s`.

Whenever:

```java
s.charAt(j) == t.charAt(i)
```

I increase `j`.

One important thing I learned here was that `j` represents the **number of characters from `s` that have already been matched**.

Therefore, when:

```java
j == s.length()
```

it means the complete string `s` has been found as a subsequence of `t`.

I also learned why boundary checking matters. Before accessing:

```java
s.charAt(j)
```

I need to make sure:

```java
j < s.length()
```

Otherwise, after matching the final character, `j` could become equal to `s.length()`, and accessing that index would cause an error.

The biggest thing I noticed today is that my problem-solving is slowly changing.

Earlier, I often looked at a problem and immediately tried to write code. Now I'm starting to spend more time asking:

* What does each variable represent?
* Does the order of elements matter?
* Can I solve this with one traversal?
* Is this a pattern I've already seen?
* Can I maintain the answer while scanning?

Today's two problems looked completely different, but both were solved using simple and reusable ideas rather than complicated algorithms.

For **Best Time to Buy and Sell Stock**, I learned to maintain the **minimum value so far and the best result so far**.

For **Is Subsequence**, I reinforced **two pointers and ordered traversal**.

This is exactly the kind of pattern recognition I want to develop during my LeetCode journey.

## 📌 Day 23 Summary

**Problems Solved:** 2

**Main Patterns:**

* Minimum So Far
* Maximum Result So Far
* Two Pointers
* Ordered Traversal
* Character Matching
* Boundary Checking

**Main Lesson:**

> Don't just look at the values. Understand what each variable represents and how the order of operations affects the answer.

**Day 23 — Complete ✅**
SEEYA ON DAY 24...🚀

# 📖 Day 24 — DSA Journey Documentation

**Date:** 09-08-2026

Today I solved two Easy LeetCode problems: **599. Minimum Index Sum of Two Lists** and **1047. Remove All Adjacent Duplicates In String**.

The first problem, **Minimum Index Sum of Two Lists**, was a good exercise in using nested loops and maintaining a minimum value.

My initial thought was to compare every element of `list1` with every element of `list2`. Whenever both strings matched, I calculated their index sum using:

```java id="3f8w6h"
int indexSum = i + j;
```

Then I maintained the smallest index sum.

One important thing I learned was that the answer can contain **multiple strings with the same minimum index sum**. Because of this, I needed a separate `List<String>` to store the answers.

The logic became:

```text id="lks1y0"
New smaller index sum → update minimum + clear old answers + add current string
Same minimum        → add current string
Larger minimum      → ignore
```

I initially made the mistake of setting:

```java id="e8w2xk"
int min = 0;
```

but realized that this would not work because index sums are non-negative. I learned to initialize the minimum with:

```java id="1i1z7v"
Integer.MAX_VALUE
```

I also reinforced Java concepts such as using `.equals()` for String comparison, using `List<String>` with generics, `ArrayList`, `clear()`, `add()`, and converting a list back into a `String[]`.

The second problem, **Remove All Adjacent Duplicates In String**, was more interesting because I initially found the given example confusing.

For:

```text id="q7i9g4"
"abbaca"
```

the process is:

```text id="7k1x6r"
abbaca
  ↓ remove bb
aaca
  ↓ remove aa
ca
```

The important observation was that after removing `bb`, the two `a`s become adjacent. This made me realize that the problem is naturally suited to a **stack**.

The stack keeps the characters that have survived so far.

For every character:

```text id="xg7k93"
If current character == stack top
        → pop

Otherwise
        → push
```

For example:

```text id="h0kj3d"
a → [a]
b → [a,b]
b → [a]       // bb removed
a → []        // aa removed
c → [c]
a → [c,a]
```

The final stack contains `c` and `a`, giving:

```text id="9xj8cs"
"ca"
```

While coding, I made several syntax and Java API mistakes. I initially tried to use methods such as `top()` directly on the String, but learned that these are stack operations.

For a Java `Stack<Character>`:

```text id="4g0a5b"
isEmpty() → checks whether the stack is empty
peek()    → looks at the top element
pop()     → removes the top element
push()    → adds an element
```

I also initially tried to push the index:

```java id="v7d4u1"
stack.push(i);
```

but the stack contains `Character`, so the correct value to push is:

```java id="g9m2sa"
stack.push(s.charAt(i));
```

Another small but useful lesson was using `StringBuilder` to construct the final answer. I initially used assignment when I needed to append characters. I learned the difference between:

```java id="h3k8s2"
ans = something;
```

and:

```java id="x4m7q1"
ans.append(something);
```

The first replaces the value, while the second adds to the existing `StringBuilder`.

Overall, Day 24 helped me understand two useful patterns:

**Minimum + collect all ties** for the first problem, and **Stack + adjacent cancellation** for the second.

More importantly, I am getting better at identifying the data structure or pattern before immediately trying to code the solution.

## 📌 Day 24 Summary

**Problems Solved:** 2

**Main Patterns Learned:**

* Nested Loop Comparison
* Minimum Value Tracking
* Collecting Multiple Minimum Answers
* Stack
* Adjacent Cancellation
* Push / Pop / Peek
* StringBuilder
* Java Generics
* String `.equals()`

### 🔥 Main Lesson

> **First understand what needs to be remembered during the traversal, then choose the data structure that naturally stores that information.**

For today's stack problem, the key realization was:

> **If the current character needs to interact with the most recently kept character, think about a stack.**

**Day 24 — Complete ✅**

SEEYA ON DAY 25...🚀

# 📖 DSA Journey Documentation — Day 25

**Date:** 10-08-2026

## Problem Solved

### 49. Group Anagrams

**Difficulty:** Medium
**Pattern:** HashMap + Sorting

---

## 🧠 Problem Understanding

The problem gives an array of strings and asks us to group strings that are anagrams of each other.

For example:

```text
["eat", "tea", "tan", "ate", "nat", "bat"]
```

The anagram groups are:

```text
["eat", "tea", "ate"]
["tan", "nat"]
["bat"]
```

The important thing I understood is that two strings don't need to be in the same order to be anagrams. They only need to contain the same characters with the same frequencies.

---

## 💭 My Initial Thinking

I immediately connected this problem with **Valid Anagram**, which I had already learned.

In Valid Anagram, I used a frequency array to check whether two strings contained the same characters.

For Group Anagrams, however, there are many strings, so I needed a way to identify which strings belong to the same group.

I decided to use a **HashMap**.

The key idea was:

```text
Original String
      ↓
Sort its characters
      ↓
Use sorted string as key
      ↓
Store original string in that key's list
```

---

## 🔑 Core Idea

For every string, I sort its characters.

For example:

```text
eat → aet
tea → aet
ate → aet
```

Since all three produce `"aet"`, they can use the same HashMap key.

The HashMap concept becomes:

```text
"aet" → ["eat", "tea", "ate"]
"ant" → ["tan", "nat"]
"abt" → ["bat"]
```

This allows all anagrams to automatically fall into the same group.

---

## 💻 Approach

### Step 1 — Create the HashMap

```java
HashMap<String, List<String>> map = new HashMap<>();
```

The structure is:

```text
Key   → Value
String → List<String>
```

The key is the sorted representation, and the value is the group of original strings.

### Step 2 — Traverse Every String

```java
for (String str : strs)
```

Process one string at a time.

### Step 3 — Convert String to Character Array

```java
char[] chars = str.toCharArray();
```

This allows the characters to be sorted.

### Step 4 — Sort the Characters

```java
Arrays.sort(chars);
```

Example:

```text
"tea"
 ↓
['t','e','a']
 ↓
['a','e','t']
```

### Step 5 — Create the Key

```java
String key = new String(chars);
```

Now:

```text
"tea" → "aet"
```

### Step 6 — Create a Group if Necessary

```java
map.putIfAbsent(key, new ArrayList<>());
```

If the key doesn't exist, create an empty list.

### Step 7 — Add the Original String

```java
map.get(key).add(str);
```

Important: I add the **original string**, not the sorted string.

### Step 8 — Return All Groups

```java
return new ArrayList<>(map.values());
```

The keys are only used for grouping, so I return the values.

---

# 🧩 Example Walkthrough

Input:

```text
["eat","tea","tan","ate","nat","bat"]
```

Processing:

```text
eat → aet → aet: [eat]

tea → aet → aet: [eat, tea]

tan → ant → ant: [tan]

ate → aet → aet: [eat, tea, ate]

nat → ant → ant: [tan, nat]

bat → abt → abt: [bat]
```

Final:

```text
[
    ["eat","tea","ate"],
    ["tan","nat"],
    ["bat"]
]
```

The order doesn't matter.

---

# 📚 Java Concepts Learned

Today I reinforced several Java concepts:

* `HashMap`
* `List<String>`
* `ArrayList`
* `toCharArray()`
* `Arrays.sort()`
* `new String(char[])`
* `putIfAbsent()`
* `map.get(key)`
* `map.values()`
* Generics
* Nested collection structure: `List<List<String>>`

---

# 🔥 Important DSA Pattern

The biggest pattern I learned today is:

## Common Key → HashMap Grouping

When multiple elements need to be grouped according to some property:

```text
Element
   ↓
Find common representation
   ↓
Use it as HashMap key
   ↓
Store elements with same key together
```

For this problem:

```text
Property → Anagram
Key      → Sorted characters
Structure → HashMap
```

---

# 🔗 Connection With Previous Problems

This problem connected directly with **Valid Anagram**.

### Before:

```text
Two strings
    ↓
Check character frequencies
    ↓
Are they anagrams?
```

### Today:

```text
Many strings
    ↓
Create common anagram key
    ↓
HashMap
    ↓
Group them
```

This was a good example of taking an already-learned concept and applying it to a more advanced problem.

---

# 📈 Growth / Improvement

Today I learned that I don't always need to compare every string with every other string.

Instead of doing:

```text
eat ↔ tea
eat ↔ tan
eat ↔ ate
...
```

I can transform every string into a common representation.

```text
eat → aet
tea → aet
ate → aet
```

Then the HashMap handles the grouping.

This is an important improvement in how I think about DSA problems:

> **Look for a property that can become a key instead of repeatedly comparing elements.**

---

# 🎯 What I Should Remember

### Main Pattern

**HashMap + Common Key**

### Anagram Key

**Sort characters → use sorted string as key**

### Useful Java Pattern

```java
map.putIfAbsent(key, new ArrayList<>());
map.get(key).add(str);
```

### Mental Model

```text
Transform
    ↓
Create Key
    ↓
HashMap
    ↓
Group
```

---

# ✅ Day 25 Status

**Problem Solved:** 1
**Problem:** 49. Group Anagrams
**Difficulty:** Medium
**Main Pattern:** HashMap + Sorting
**Previous Concept Reused:** Valid Anagram
**New Major Concept:** Common-key HashMap grouping

## 🚀 Day 25 — Problem 1 Complete

SEEYA ON DAY 26...🚀

# Day 26 — LeetCode Documentation

**Date:** 11-08-2026

## Problems Solved

### 1. 2996 — Smallest Missing Integer Greater Than Sequential Prefix Sum

**Approach:** HashSet + Sequential Prefix

**What I learned:**

* A sequential prefix continues when `nums[i] == nums[i - 1] + 1`.
* Calculate the sum only until the sequential prefix breaks.
* Use a `HashSet` to store all array elements.
* Use `set.contains(sum)` to check whether the current number exists.
* Keep increasing `sum` until a missing number is found.

**Pattern:**

```text
Find sequential prefix
        ↓
Calculate prefix sum
        ↓
HashSet membership check
        ↓
Increase until missing
```

---

### 2. 1475 — Final Prices With a Special Discount in a Shop

**Approach:** Nested Loops / Brute Force

**What I learned:**

* For every element, search only to its right.
* Start `j` from `i + 1`.
* Find the **first** price satisfying `prices[j] <= prices[i]`.
* Apply the discount and immediately `break`.
* Initialize `ans[i] = prices[i]` because there may be no discount.

**Pattern:**

```text
Current element
      ↓
Search to the right
      ↓
First valid element
      ↓
Update answer
      ↓
break
```

**Complexity:**

* Time: `O(n²)`
* Space: `O(n)`

---

### 3. 1512 — Number of Good Pairs

**Approach:** Nested Loops

**What I learned:**

* A good pair requires `nums[i] == nums[j]` and `i < j`.
* Starting `j` from `i + 1` automatically guarantees `i < j`.
* Count every matching pair.

**Pattern:**

```java
for (int i = 0; i < nums.length; i++) {
    for (int j = i + 1; j < nums.length; j++) {
        if (nums[i] == nums[j]) {
            count++;
        }
    }
}
```

**Complexity:**

* Time: `O(n²)`
* Space: `O(1)`

---

# 🧠 Important Concepts — Day 26

1. **Sequential Prefix**
2. **HashSet for Membership Checking**
3. **Nested Loops**
4. **Look to the Right using `j = i + 1`**
5. **First Valid Element + `break`**
6. **Default Answer Initialization**
7. **Frequency Counting**
8. **Good Pair Condition**
9. **Separating Different Parts of a Problem**

## 🔥 Biggest Learning

One important pattern from today was:

```text
Previous Frequency → Number of New Pairs
```

If a number has already appeared `k` times, seeing it again creates exactly `k` new good pairs.

This is the foundation of the more optimized **HashMap frequency-counting solution** for problems like Number of Good Pairs.

**Day 26 — Completed Successfully ✅**

SEEYA ON DAY 27...🚀

# 📖 DSA Journey Documentation — Day 27

**Date:** 12-08-2026

## Problems Worked On

### 2958. Length of Longest Subarray With at Most K Frequency

**Difficulty:** Medium
**Pattern:** HashMap + Sliding Window
**Status:** ⏸️ Paused

---

## 🧠 Problem Understanding

The problem gives an integer array `nums` and an integer `k`.

We need to find the **longest contiguous subarray** where every element appears at most `k` times.

For example:

```text
nums = [1,2,3,1,2,3,1,2]
k = 2
```

The longest valid subarray is:

```text
[1,2,3,1,2,3]
```

because every number appears exactly two times.

---

## 💭 My Initial Thinking

I first thought this was mainly a **HashMap / HashSet** problem because the problem talks about frequency.

I tried a brute-force approach:

```text
Choose starting index i
        ↓
Traverse using j
        ↓
Count frequency
        ↓
If frequency > k → break
        ↓
Calculate subarray length
        ↓
Update maximum
```

The approach was logically correct, but it resulted in **TLE**.

---

## ❌ Why My Approach Got TLE

The nested loops repeatedly check many of the same elements.

The approximate complexity is:

```text
O(n²)
```

For a large input, this becomes too slow.

---

## 🔑 New Concept Introduced — Sliding Window

The optimized pattern for this problem is:

```text
HashMap + Sliding Window
```

The basic idea is:

```text
right → expand the window
left  → shrink the window when invalid
```

The HashMap stores:

```text
element → frequency
```

When an element's frequency becomes greater than `k`, the current window becomes invalid. Instead of restarting the search from the beginning, we move `left` forward and decrease the frequency of the elements we remove.

I decided to **pause this problem** because I want to understand Sliding Window properly instead of memorizing the solution.

---

# 1672. Richest Customer Wealth

**Difficulty:** Easy
**Pattern:** 2D Array Traversal + Maximum Value
**Status:** ✅ Solved

---

## 🧠 Problem Understanding

The problem gives a 2D array where:

```java
accounts[i][j]
```

represents the amount of money customer `i` has in bank `j`.

We need to calculate the total wealth of every customer and return the maximum wealth.

Example:

```text
accounts = [
    [1,2,3],
    [3,2,1]
]
```

First customer:

```text
1 + 2 + 3 = 6
```

Second customer:

```text
3 + 2 + 1 = 6
```

Answer:

```text
6
```

---

## 💭 My Initial Thinking

I understood that this was a **2D array traversal** problem, so I needed nested loops.

However, I initially confused:

```java
accounts.length
```

with:

```java
accounts[i].length
```

This was the same type of mistake I had made before with 2D arrays.

---

## 🔑 Important 2D Array Concept

```java
accounts.length
```

means:

```text
Number of rows
```

while:

```java
accounts[i].length
```

means:

```text
Number of elements in row i
```

Therefore:

```java
for (int i = 0; i < accounts.length; i++) {
    for (int j = 0; j < accounts[i].length; j++) {
        sum += accounts[i][j];
    }
}
```

---

## ⚠️ Recurring Mistake — Row vs Element

I noticed that I repeatedly confuse:

```java
accounts[i]
```

and:

```java
accounts[i][j]
```

Remember:

```text
accounts[i]       → entire row
accounts[i][j]    → one element
```

And:

```text
i → row
j → column
```

This is now a **recurring DSA mistake** that I should actively check whenever I solve a 2D array problem.

---

## 🔥 Maximum Value Pattern

After calculating each customer's wealth:

```java
if (sum > max) {
    max = sum;
}
```

General pattern:

```text
Calculate current value
        ↓
Compare with max
        ↓
Update max if current value is larger
```

This is the **Maximum Value Pattern**.

---

# 1572. Matrix Diagonal Sum

**Difficulty:** Easy
**Pattern:** 2D Array + Diagonal Indexing
**Status:** ✅ Solved

---

## 🧠 Problem Understanding

The problem gives a square matrix and asks for the sum of both diagonals.

Example:

```text
[1 2 3]
[4 5 6]
[7 8 9]
```

Main diagonal:

```text
1 + 5 + 9 = 15
```

Secondary diagonal:

```text
3 + 5 + 7 = 15
```

The center `5` is counted twice, so it must be subtracted once.

Final answer:

```text
25
```

---

## 🔑 Main Diagonal

The main diagonal follows:

```java
mat[i][i]
```

Example:

```text
mat[0][0] → 1
mat[1][1] → 5
mat[2][2] → 9
```

Pattern:

```text
[i][i]
```

---

## 🔑 Secondary Diagonal

The secondary diagonal follows:

```java
mat[i][n - 1 - i]
```

Example:

```text
mat[0][2] → 3
mat[1][1] → 5
mat[2][0] → 7
```

Pattern:

```text
[i][n - 1 - i]
```

---

## ⚠️ Center Element

If the matrix size is odd, the center element belongs to both diagonals.

Therefore:

```java
if (n % 2 == 1) {
    sum -= mat[n / 2][n / 2];
}
```

This prevents counting the center twice.

---

# 📚 Java / DSA Concepts Learned Today

* 2D array traversal
* Nested loops
* Rows and columns
* `array[i]` vs `array[i][j]`
* `accounts.length`
* `accounts[i].length`
* Row sum
* Maximum value pattern
* Main diagonal indexing
* Secondary diagonal indexing
* Handling duplicate center elements
* HashMap frequency
* Subarray concept
* Sliding Window introduction
* Recognizing TLE
* Understanding `O(n²)` brute force

---

# 🔥 Important Concepts — Day 27

### 1. 2D Array Traversal

```java
array[i][j]
```

```text
i → row
j → column
```

### 2. Row vs Element

```java
array[i]       // entire row
array[i][j]    // individual element
```

### 3. Correct Inner Loop

```java
for (int j = 0; j < array[i].length; j++)
```

The inner loop should use the current row's length when traversing its columns.

### 4. Row Sum

```java
sum += accounts[i][j];
```

### 5. Maximum Value Pattern

```java
if (sum > max) {
    max = sum;
}
```

### 6. Main Diagonal

```java
mat[i][i]
```

### 7. Secondary Diagonal

```java
mat[i][n - 1 - i]
```

### 8. Frequency Pattern

```text
element → frequency
```

### 9. Sliding Window

```text
right → expand
left  → shrink
```

### 10. TLE Recognition

A brute-force nested-loop solution can become:

```text
O(n²)
```

and may cause TLE when the input size is large.

---

# 🔗 Connection With Previous Problems

### HashMap

I previously used HashMap in problems such as:

```text
49. Group Anagrams
```

Today I recognized that frequency-based problems can also use HashMap:

```text
element → frequency
```

This is useful for problems where we need to know how many times an element appears.

### Maximum Value Pattern

The same pattern appears again:

```java
if (value > max) {
    max = value;
}
```

Used in:

```text
1672. Richest Customer Wealth
```

### 2D Arrays

Today I practiced two different types of 2D array problems:

```text
1672 → row traversal + row sum
1572 → diagonal indexing
```

This helped me understand that correct indexing is one of the most important parts of working with matrices.

---

# 📝 Recurring Mistake To Remember

## 2D Array Row vs Element Confusion

I repeatedly confuse:

```java
array[i]
```

with:

```java
array[i][j]
```

Remember:

```text
array[i]
    ↓
entire row

array[i][j]
    ↓
one element
```

And:

```text
i → row
j → column
```

Before writing a 2D array loop, I should first identify:

```text
How many rows?
How many columns in the current row?
What does i represent?
What does j represent?
```

---

# 📈 Growth / Improvement

Today I strengthened my understanding of **2D arrays, nested loops, matrix indexing, row sums, and maximum-value patterns**.

I also started recognizing when a brute-force solution is too slow.

The 2958 problem was difficult because it introduced **Sliding Window**. I understood the reason my nested-loop approach got TLE, but I decided to pause the problem and learn the pattern properly before solving it.

Most importantly, I identified a recurring mistake:

> I sometimes confuse `array[i]` (the complete row) with `array[i][j]` (a single element).

I need to keep checking this whenever I work with 2D arrays.

---

# 🎯 What I Should Remember

```text
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

---

# ✅ Day 27 Status

**Problems Solved:** 2
**Problem Paused:** 1
**Problems Worked On:** 2958, 1672, 1572
**Main Topics:** 2D Arrays, HashMap, Frequency, Maximum Value, Matrix Diagonals, Sliding Window

## 🚀 Day 27 — Completed

Today I solved two Easy problems and strengthened my understanding of **2D array traversal, row sums, maximum-value patterns, and matrix diagonal indexing**.

I also attempted a Medium Sliding Window problem and understood why my brute-force approach resulted in TLE.

I identified a recurring mistake in my DSA journey:

> **`array[i]` is a row, while `array[i][j]` is an individual element.**

This is something I need to remember in every future 2D array problem.

# 👋 See You on Day 28!

# 📖 DSA Journey Documentation — Day 28

**Date:** 13-08-2026

Today was a really interesting DSA session because I worked with different types of problems instead of staying with one pattern.

I started with **1486. XOR Operation in an Array**. The problem looked simple, and I was able to understand the formula behind the array quickly. Instead of creating the array first, I realized that I could generate each value directly while traversing it and keep combining the values. This was a good reminder that I don't always need to explicitly create the data mentioned in the problem. Sometimes I can work with it directly.

After that, I solved **136. Single Number**. This felt easier because I was able to connect it with the XOR concept from the previous problem. The biggest improvement here was recognizing that the idea I had just learned could immediately be reused in another problem. I didn't have to treat the problem as something completely new.

Then I worked on **1859. Sorting the Sentence**. This was different because I decided to try solving it in **Python**, even though most of my recent LeetCode work has been in Java. I already understood the logic of the problem, so instead of worrying about the algorithm, I focused on learning how Python expresses the same idea. This helped me realize that once the problem-solving logic is clear, changing the language mainly becomes a syntax challenge rather than a DSA challenge.

The final problem was **1925. Count Square Sum Triples**. At first, I was confused about how to decide which values should be used for `a`, `b`, and `c`. I was looking for some special way to choose them, but then I realized that I didn't need to guess anything. I could simply try every possible value within the given range and check whether the condition was satisfied. That helped reinforce an important mindset: when the constraints are small, a straightforward brute-force solution can be completely reasonable.

### 💭 How My Thinking Was Today

One thing I noticed today is that I am becoming better at breaking problems into smaller questions.

Instead of immediately asking:

> "What is the code?"

I am starting to ask:

> "What exactly is the problem asking me to find?"

and then:

> "What values are possible?"

and finally:

> "Can I simply check all possibilities?"

That change in thinking is important.

### ❌ Mistakes I Made Today

My biggest mistake today was not really a coding mistake. It was **overthinking the choice of values** in the square-triples problem.

I initially thought I somehow needed to know in advance which numbers should become `a`, `b`, and `c`.

I eventually realized that I don't always need to predict the answer. Sometimes I can let the algorithm **try the possibilities and verify them**.

Another thing I noticed is that I still sometimes focus too much on the programming language syntax before fully settling the algorithm. Working on the Python problem showed me that the better order is:

**Understand the logic first → then worry about syntax.**

### 📈 Improvements Today

I feel that my problem-solving is becoming more flexible.

Earlier, I often tried to find a specific trick immediately. Today I was more comfortable with:

* Reusing a pattern I had just learned.
* Switching from Java to Python without changing the underlying logic.
* Using brute force when the constraints allow it.
* Generating values directly instead of unnecessarily creating extra structures.
* Breaking a problem into "generate → check → count" instead of overcomplicating it.

### 🧠 What I Want to Improve

I still want to get faster at recognizing **what kind of problem I am looking at**.

I also want to become better at deciding when brute force is enough and when I should look for an optimized approach.

Most importantly, I want to stop feeling that every Medium-looking problem needs some complicated trick. Sometimes the simplest correct idea is enough.

### 🎯 Biggest Lesson of Day 28

> **Don't try to be clever before understanding the problem.**

Today showed me that many problems become much easier when I first understand:
what I have, what I need, and what possibilities I am allowed to check.

My goal is not just to solve more problems. It is to become better at **thinking through problems before touching the code**.

## ✅ Day 28 — Completed

Today I solved four problems and, more importantly, practiced different ways of thinking instead of relying on one single pattern.

**Day 28 complete. 🚀**

# 👋 See You on Day 29!

# 📖 DSA Journey Documentation — Day 29

**Date:** 14-08-2026

Today was an important day in my DSA journey because I finally started understanding a pattern that I had struggled with before.

I began with **3090. Maximum Length Substring With Two Occurrences**. At first, I did not understand the problem statement clearly. The phrase "at most two occurrences" confused me, and I was not sure what the problem actually wanted.

After breaking the statement down into a simple sentence, I understood it as:

> Find the longest continuous part of the string where no character appears more than two times.

At first, I thought about whether the problem might be related to Binary Search, but after understanding the structure of the problem, I realized that it was a **Sliding Window** problem.

This was important because I had already struggled with **2958** earlier and had paused it because I could not understand Sliding Window properly.

While solving 3090, I made several small mistakes. I initially used the wrong Java string method, confused the frequency array with the frequency of the current character, and tried to move the `left` pointer without actually removing the character that was leaving the current substring.

The biggest breakthrough came when I understood what `left` really means.

> `left` is not just a variable that moves. It represents the beginning of the current substring.

So when `left` moves forward, the character at the old position is no longer part of the current substring and its frequency must be reduced.

Once that clicked, the whole pattern became much easier to understand:

```text
Expand the substring
        ↓
Check the condition
        ↓
If invalid, shrink from the left
        ↓
Continue
```

This problem gave me confidence because something that previously felt confusing in 2958 finally started making sense.

---

## 💭 My Thinking Improvement

One of the biggest improvements today was that I stopped trying to memorize the Sliding Window code.

Instead, I started understanding **why the window moves**.

Earlier, I was thinking:

> "What code do I need for Sliding Window?"

Today, I started thinking:

> "What is inside my current window, why is it invalid, and what needs to leave?"

That is a much better way of learning.

---

# 2185. Counting Words With a Given Prefix

The second problem was much easier.

The main thing I had to understand was the word **prefix**.

I understood that a prefix must start from the beginning of the word.

For example:

```text
attention
```

contains prefixes such as:

```text
a
at
att
atte
```

but something in the middle is not a prefix.

The problem itself was straightforward once I understood the definition.

I did make a small mistake while coding. I tried using the string method on the entire array instead of the individual word.

That reminded me of a mistake I have made before:

> I sometimes confuse the collection itself with the individual element inside it.

I corrected it by focusing on what `words[i]` actually represents.

This was another useful reminder that before using a method, I should check **what type of object I am calling it on**.

---

# 1967. Number of Strings That Appear as Substrings in Word

This problem was connected directly to the previous one, which made it easier.

The important thing I had to understand was the difference between a **prefix** and a **substring**.

A prefix must be at the beginning.

A substring can appear anywhere, but it must remain continuous.

Once I understood this difference, the problem became very simple.

The nice part was that I could connect it directly with the previous question:

```text
2185 → starts with the pattern
1967 → contains the pattern anywhere
```

This helped me understand that sometimes two problems look almost identical, but one small change in the wording changes exactly what I need to check.

---

# ❌ Mistakes I Made Today

The main mistakes today were:

- Not understanding the problem statement clearly at the beginning.
- Confusing the whole array with an individual string.
- Using the wrong Java string method initially.
- Moving the sliding-window `left` pointer without removing the character from the current window.
- Thinking about the algorithm before fully understanding the definition in the problem.

These are not just coding mistakes. They show me that I need to slow down during the **problem-understanding stage**.

---

# 📈 What Improved Today

Today I improved in a few important ways.

First, I finally made real progress with **Sliding Window**, which had been a weak point for me.

Second, I became more comfortable reading problem statements and translating them into simple language.

Third, I started noticing the importance of small wording differences:

```text
prefix     → beginning
substring  → anywhere, but continuous
```

Fourth, I became more comfortable reusing ideas from one problem in another.

The biggest improvement was not the code itself.

It was my **thinking process**.

---

# 🧠 What I Want To Remember

Before coding, I should ask myself:

```text
What exactly is the problem asking?
What does each important word mean?
What is the current window / current element?
What makes the current situation invalid?
What needs to change to make it valid again?
```

I also want to remember:

> **Don't rush into code when the problem statement itself is still unclear.**

Understanding the problem first makes the coding much easier.

---

# 🎯 Biggest Lesson of Day 29

> **A pattern becomes easier when I understand why it works instead of memorizing its code.**

Today, Sliding Window finally started making sense because I understood the role of `left` and `right`, not because I memorized a template.

That is the kind of progress I want to keep making in my DSA journey.

# ✅ Day 29 — Completed

Today I solved three Easy problems, improved my understanding of Sliding Window, strengthened my string-problem thinking, and learned to pay more attention to the exact wording of a problem.

This was a good step forward.

# 👋 See You on Day 30!


# 📖 DSA Journey Documentation — Day 30

**Date:** 15-08-2026

Today was a good day for understanding how much my problem-solving is changing compared to when I started this journey.

I worked on four problems today: **724. Find Pivot Index**, **1991. Find the Middle Index in Array**, **747. Largest Number At Least Twice of Others**, and **1534. Count Good Triplets**.

The biggest thing I noticed today was **pattern recognition**.

When I started `724`, my first thought was to create separate arrays for the left sums and right sums. That was a natural way for me to think about the problem, but while working through it, I realized that I didn't actually need to store everything. I could use the total sum and keep track of the left side while calculating the right side from what I already knew.

That was an important improvement in my thinking. Instead of storing more information than necessary, I started asking:

> “What information do I really need at this moment?”

Then I came across **1991**, which was almost the same idea as `724`. Instead of treating it as a completely new problem, I recognized the connection immediately and reused the same way of thinking.

This was probably my biggest win today.

I am slowly starting to understand that DSA is not about memorizing hundreds of separate solutions. A lot of problems are different versions of ideas I have already seen.

---

## 💭 How My Thinking Changed

In `747`, I initially wanted to solve everything in one loop.

I was trying to make the solution shorter and more clever, but I realized that this was not actually helping me understand the problem better.

I ended up using two simple passes:

1. Find the largest element and its index.
2. Check it against every other element.

The important realization was that **using two loops does not automatically mean the solution is slow**.

I was focusing too much on the number of loops instead of thinking about the overall efficiency.

That is something I want to remember going forward:

> **Don't try to reduce the number of loops just for the sake of writing fewer loops.**

A clear solution with good overall complexity is better than a confusing "one-loop" solution.

---

## ❌ Mistakes I Made Today

One mistake that stood out was confusing an **index** with a **value**.

I was using a variable to represent the position of the largest element, but then I accidentally treated that position as if it were the actual number.

That reminded me of the array-related mistakes I have made before.

I need to keep asking myself:

> “Am I storing the position, or am I storing the actual value?”

Another mistake was trying to force an unnecessarily clever solution when the straightforward solution was already good enough.

---

## 💡 1534 and Connection With Previous Problems

When I reached `1534`, I immediately recognized it as another problem where I could simply try combinations and check the conditions.

This connected directly with **1925. Count Square Sum Triples**, which I solved earlier.

That made `1534` much easier.

Instead of thinking:

> “I have never solved this exact problem before.”

I started thinking:

> “This looks like something I have already done, just with a different condition.”

That is exactly the kind of thinking I want to develop through this journey.

---

## 📈 Improvements Today

Today I feel I improved in three major ways.

### 1. Pattern Recognition

I recognized:

```text
724 → 1991
1534 → 1925
```

The problems were not exactly identical, but the underlying way of thinking was very similar.

### 2. Simpler Thinking

I am becoming more comfortable with simple solutions when the constraints allow them.

I don't want to force an advanced algorithm just because it looks more impressive.

### 3. Understanding Before Optimizing

I am starting to separate these two questions:

```text
Does my logic work?
        ↓
Is my solution efficient enough?
```

First I want to understand the problem correctly. Then I can think about optimization.

---

## 🧠 What I Want To Remember

Today reminded me that a very important DSA skill is:

> **Recognizing something familiar inside something that looks new.**

I also want to remember:

```text
Don't confuse index with value.
Don't force fewer loops unnecessarily.
Reuse patterns from previous problems.
Understand first, optimize second.
```

---

## 🎯 Biggest Lesson of Day 30

> **The real progress in DSA is not just the number of problems solved. It is how quickly I can recognize the thinking behind a new problem.**

Today I saw multiple examples of that.

`1991` reminded me of `724`.

`1534` reminded me of `1925`.

And `747` taught me that a simple two-pass solution can be better for me than forcing everything into one loop.

That makes me feel like I am slowly moving from:

**“How do I solve this?”**

to:

**“Which pattern does this remind me of?”**

That is a change I want to keep building.

# ✅ Day 30 — Completed

Today I solved four problems and focused more on **thinking patterns, connections, and mistakes** than just the final code.

The goal is becoming clearer:

> **I don't want to memorize solutions. I want to become someone who can figure out the solution.**

# 👋 See You on Day 31!

# 📖 DSA Journey Documentation — Day 31

**Date:** 16-08-2026

Today was a special day in my DSA journey because I crossed a milestone that I had been working toward for a long time:

# 🏆 101 LeetCode Problems Solved

Seeing the number go from two digits to **101 solved problems** felt different.

It is not just a number.

It represents all the times I was confused by a problem, made a wrong assumption, wrote incorrect code, got stuck, tried again, and eventually understood it.

Today I solved six problems, but the bigger achievement was realizing how much my way of thinking has changed.

---

## 💭 How I Approached Today's Problems

The first problem I worked on was about **odd-length subarrays**.

At first, I made a simple mistake: I was checking the length of the entire array instead of thinking about the length of the current subarray.

That made me stop and rethink what the problem was actually asking.

I then started thinking in terms of:

```text
Where does the subarray start?
Where does it end?
How long is it?
```

This was a useful reminder that I need to understand the exact object the problem is talking about before writing code.

I also initially thought I might need an extra loop to calculate the sum of every subarray. While working through it, I found a better way to keep track of the sum as the subarray grew.

That felt like a genuine improvement in my thinking because I was able to simplify my own approach instead of depending on a completely different solution.

---

The second problem was another **2D array** problem.

Interestingly, I made the same kind of indexing mistake that I have made several times before.

I again confused the whole row with an individual element.

This is now clearly a recurring mistake in my DSA journey.

The positive part is that I noticed it quickly and corrected it.

I think this is something important about learning:

> Repeated mistakes are not a problem if I am actually becoming faster at recognizing them.

I don't expect myself to stop making every mistake immediately.

I want to become better at catching them.

---

The number-digit problem was much more straightforward.

I was comfortable breaking the number down digit by digit and maintaining the values I needed.

This kind of problem now feels much more natural compared to when I first started DSA.

---

The binary-tree problem was also very simple.

What I liked about it was that I did not overthink it.

I saw exactly what the problem was asking and directly checked the relationship between the root and its children.

That is something I want to become better at:

> Not every problem needs a complicated thought process.

Sometimes understanding the statement clearly is enough.

---

The operations problem was another good exercise in thinking step by step.

I treated it like a simulation:

```text
Do the operation
↓
Update the values
↓
Count the operation
↓
Repeat
```

This felt natural.

I didn't try to search for a clever trick immediately.

I just followed the rules of the problem.

That is a small but meaningful improvement in my problem-solving style.

---

The final problem was the robot movement problem.

I tracked what was happening to the robot as each move came in.

Again, I focused on the state of the problem rather than trying to overcomplicate it.

At this point, I am starting to feel more comfortable with problems where the answer comes from simply tracking what changes over time.

---

# 🧠 What I Realized Today

The biggest lesson from today wasn't from any single problem.

It was about **consistency**.

When I look back at the problems I was struggling with earlier in this journey, many things that seemed confusing are now becoming more familiar.

I'm starting to recognize things like:

```text
"This looks similar to something I already solved."
```

That is probably one of the biggest signs of progress.

---

# ❌ Mistakes I Still Make

I still make repeated mistakes.

The biggest one today was again related to 2D arrays.

I also sometimes misunderstand what exactly the problem is asking before I start coding.

And sometimes I make things harder than they need to be because I try to find a "better" solution before making sure my simple solution is fully understood.

These are things I want to keep improving.

---

# 📈 How I Am Improving

I think my biggest improvement is that I am becoming more comfortable with being stuck.

Earlier, getting stuck felt like:

> "I don't know this."

Now it feels more like:

> "I haven't figured this out yet."

That difference matters.

I'm also getting better at:

- breaking problems into smaller parts
- connecting new problems with old ones
- recognizing when I am repeating a mistake
- staying with a problem longer
- keeping the solution simple when simplicity is enough

---

# 🏆 101 Problems — What It Means To Me

Reaching 101 solved problems today feels like proof that consistency works.

I didn't solve 100 problems in one day.

I didn't suddenly become good at DSA.

It happened because I kept showing up.

Some days I solved a lot.

Some days I got stuck.

Some problems I paused and came back to later.

Some mistakes appeared again and again.

But I continued.

That's what got me here.

---

# 🎯 Biggest Lesson of Day 31

> **Progress is not about never getting stuck. Progress is about getting unstuck faster than before.**

I want to continue learning this way.

Not just collecting solved problems, but improving the way I think through them.

Today I reached:

# 🚀 101 Problems Solved

And this feels less like an ending and more like the beginning of the next stage.

# ✅ Day 31 — Completed

**6 problems solved today.**

**101 total LeetCode problems solved.**

**44 active days.**

**33-day maximum streak.**

The journey continues.

# 👋 See You on Day 32!

# 📖 DSA Journey Documentation — Day 32

**Date:** 17-08-2026

Today I worked on **1854. Maximum Population Year**, and honestly, this problem taught me more about understanding problem statements than about coding.

## 😂 The “Easy” Problem That Took 1.2 Hours

I thought LeetCode Easy would be… easy. 😭

Then I opened **1854. Maximum Population Year**.

The coding part? Pretty straightforward.

The description? **This pretty shit** 💀

I just invested **1.2 hours** trying to understand what the problem was actually asking. 😂

Once I translated the LeetCode language into normal human language, I realized the problem was simply:

👉 Given people's birth and death years, find the year in which the **most people were alive**.

For example:

`[1993, 1999]` means the person is alive from 1993 to 1998.

So the idea becomes:

- Birth year → population `+1`
- Death year → population `-1`
- Keep a running population for each year
- Track the earliest year with the maximum population

I ended up using a **difference array**, which made the solution much cleaner.

One thing I'm realizing while learning DSA:

**Sometimes the hardest part of an Easy problem isn't the algorithm — it's understanding what the problem is actually asking.**

**1.2 hours understanding the problem. A few minutes writing the solution.** 😭

Still learning. Still getting humbled by “Easy” problems. 😂

---

## 🧠 What I Took Away

The biggest lesson from today was that **problem understanding comes before implementation**.

I spent most of the time figuring out what the question actually meant. Once I understood the timeline and the population changes, the code became much easier.

That experience reminded me that being slow on one problem does not mean I'm bad at DSA. Sometimes the difficult part is learning a new way to look at the problem.

## ✅ Day 32 — Completed

**Problem Solved:**
- `1854. Maximum Population Year` ✅

**Biggest Lesson:**
> Understand the problem in normal language first. The code becomes much easier after that.

**1.2 hours understanding. A few minutes coding. Still progress.** 🚀

#DSA #LeetCode #Java #LearningInPublic #CodingJourney

# 👋 See You on Day 33!

# Problem Solving & Metacognition Documentation — Day 36
**Date:** August 20, 2026  
**Day Number:** Day 36

---

## 1. Mental Models & Problem Decomposition

### LeetCode 1299: Overcoming Forward-Scanning Bias
* **Initial Intuition:** The direct mental model of the problem statement reads left-to-right ("look at everything to your right"). This naturally leads to writing an outer loop for the current element and an inner loop scanning the rest of the array.
* **Cognitive Shift:** Recognizing redundant computation. Scanning index `2` to `n-1` repeats the work just done when scanning index `1` to `n-1`. By flipping the direction of time/traversal (moving right-to-left), the "future" maximum is already known and can be carried backwards in a single accumulator variable.

---

### LeetCode 3069: Pointer Management & State Tracking
* **Initial Intuition & Data Structure Selection:**
  * First instinct leaned toward `HashMap`, reflecting a quick association with collection problems.
  * Pausing to analyze requirements showed that no key-value association was needed—only ordered appending and peek operations on the tail element.
  * Transitioned to primitive arrays for lower overhead and direct memory access.

* **Mistakes & Debugging Process:**
  1. **Zero-Capacity Allocation:** Initially declared `new int[0]`, which leads to immediate boundary exceptions upon writing. Corrected by allocating worst-case capacity `new int[n]`.
  2. **Coupled Indexing vs. Independent Pointers (`i - 2` Trap):**
     * Mistake: Attempted to use the loop counter expression `i - 2` to access the last element in both arrays.
     * Realization: `arr1` and `arr2` grow asynchronously. Using a shared index assumes equal distribution, which breaks when one array receives consecutive elements.
     * Resolution: Introduced independent state pointers `idx1` and `idx2`.
  3. **Off-by-One in Tail Access (`idx - 2` vs. `idx - 1`):**
     * Mistake: Subtracted 2 instead of 1 when reading the last element, causing negative index crashes.
     * Realization: Since `idx` represents the *next insertion point*, the item inserted immediately prior resides at `idx - 1`.
  4. **Array Concatenation Nuances:**
     * Mistake: Attempted to copy full buffer length `n` instead of the active slice length `idx1` / `idx2`, which would introduce unwanted default zero values.
     * Resolution: Iterated strictly through valid elements using dedicated output pointers.

---

## 2. Summary of Questions Solved

* **Total Questions Solved:** 2
  1. LeetCode 1299 — *Replace Elements with Greatest Element on Right Side*
  2. LeetCode 3069 — *Distribute Elements Into Two Arrays I*

---

*See you on Day 37*

# Problem Solving & Metacognition Documentation — Day 37
**Date:** August 21, 2026  
**Day Number:** Day 37

---

## 1. Mental Models & Problem Decomposition

### LeetCode 13: Lookahead vs. State Machine
* **Mental Model:** Roman numeral parsing requires disambiguating single-character additions from subtractive combinations (`IV`, `IX`, etc.).
* **Logical Structuring:** Instead of grouping characters into composite multi-character tokens (`"IV"`), evaluated the string strictly element-by-element with a **1-step lookahead**.
* **Invariant:** If the current value is strictly smaller than the immediately succeeding value, it acts as a negative offset to the total; otherwise, it is additive.
* **Boundary Safeguard:** Guarded lookahead comparisons with an explicit `i + 1 < s.length()` check to prevent index out-of-bounds exceptions on the tail character.

---

### LeetCode 67: Leveraging Standard Libraries vs. Fundamental Simulation
* **Mental Model:** Recognize the trade-off between practical production tools and core algorithmic expectations:
  * Using language-level arbitrary-precision utilities (`BigInteger`) solves integer overflow cleanly and handles variable length automatically.
  * In problem-solving practice, this bypasses the core structural simulation of ripple-carry adders.
* **Algorithmic Takeaway:** Standardizing the column-by-column addition mental model (iterating backwards from least-significant bits, carrying `sum / base`, appending `sum % base`) generalizes across binary addition, decimal string addition (LeetCode 415), and arbitrary base conversions.

---

## 2. Summary of Questions Solved

* **Total Questions Solved:** 2
  1. LeetCode 13 — *Roman to Integer*
  2. LeetCode 67 — *Add Binary*

---

*See you on Day 38*

# Problem Solving & Metacognition Documentation — Day 38
**Date:** August 22, 2026  
**Day Number:** Day 38

---

## 1. Mental Models & Problem Decomposition

### LeetCode 459: Moving Beyond Substring Generation
* **Initial Intuition & Misconception:**
  * Initial thought leaned toward using a `Stack`, confusing periodic pattern checking with nested structure / bracket validation.
* **Cognitive Shift & Structural Insight:**
  * Re-evaluated periodicity from a mathematical perspective:
    * If $s = P^k$ (where $k \ge 2$), then concatenating $s + s$ produces $2k$ copies of unit $P$.
    * Removing the first and last characters destroys the original copy at the start and the original copy at the end, leaving $2k - 2$ copies intact.
    * If $k \ge 2$, at least $k$ intact copies of $P$ remain contiguous in the middle, allowing $s$ to be detected via a substring match.
* **Implementation Reflections:**
  * Recognized that loops are unnecessary when checking whole-string periodicity.
  * Accounted for Java string immutability (ensuring substring operations are chained or stored rather than assuming in-place alteration).

---

## 2. Summary of Questions Solved

* **Total Questions Solved:** 1
  1. LeetCode 459 — *Repeated Substring Pattern*

---

*See you on Day 39*

# Problem Solving & Metacognition Documentation — Day 39
**Date:** August 23, 2026  
**Day Number:** Day 39

---

## 1. Mental Models & Problem Decomposition

### LeetCode 1071: Commutativity as an Equivalence Test
* **Mental Model:** String periodicity behaves algebraically. If $S = P^a$ and $T = P^b$, concatenation must commute ($S + T = T + S$).
* **Reduction:** Checking string commutativity completely isolates the structural check from the numerical GCD computation, reducing string problem complexity to arithmetic.

---

### LeetCode 1309: Multi-Character Token Disambiguation
* **Mental Model:** Resolving token ambiguity (single vs. double digit) by identifying the delimiter token (`'#'`).
* **Lookahead vs. Lookbehind:**
  * **Forward Traversal (Lookahead):** Checking index `i + 2` for `'#'` allows greedy token resolution from the front.
  * **Pointer Increment Discipline:** When using a `for` loop with `i++`, advancing by 2 (`i += 2`) inside the conditional block results in a net advancement of 3 steps. Using `StringBuilder` avoids the quadratic $O(n^2)$ overhead of repeated immutable string concatenation.

---

## 2. Summary of Questions Solved

* **Total Questions Solved:** 2
  1. LeetCode 1071 — *Greatest Common Divisor of Strings*
  2. LeetCode 1309 — *Decrypt String from Alphabet to Integer Mapping*

---

*See you on Day 40*

# Problem Solving & Metacognition Documentation — Day 40
**Date:** August 24, 2026  
**Day Number:** Day 40

---

## 1. Mental Models & Problem Decomposition

### LeetCode 1614: Replacing Explicit Stacks with Invariant Counters
* **Mental Model:** 
  * Parentheses nesting problems often trigger the instinct to use an explicit `Stack<Character>` data structure.
  * Because the problem guarantees a valid parentheses string (VPS) and only asks for the *maximum depth* (not validation or index matching), the actual content of the stack is homogeneous (only `'('`).
* **Cognitive Shift & Optimization:**
  * Storing identical `'('` characters in dynamic heap memory via `Stack` is redundant.
  * A single integer counter tracking the current size of the conceptual stack (`openedbr`) completely simulates the stack's depth in $O(1)$ auxiliary space.
* **Brute Force vs Optimal Clarification:**
  * Even though simple counting feels basic, this single-pass counter approach is strictly optimal ($O(n)$ time, $O(1)$ space).

---

## 2. Summary of Questions Solved

* **Total Questions Solved:** 1
  1. LeetCode 1614 — *Maximum Nesting Depth of the Parentheses*

---

*See you on Day 41*

# Problem Solving & Metacognition Documentation — Day 41
**Date:** August 25, 2026  
**Day Number:** Day 41

---

## Thought Process & Problem Solving Journey

### LeetCode 3718: Smallest Missing Multiple of K

* **Initial Understanding & Approach:**
  * The goal is to find the lowest positive multiple of $k$ that does not exist in `nums`.
  * My initial idea was straightforward: start generating multiples of $k$ one by one ($k 	imes 1, k 	imes 2, k 	imes 3, \dots$) and compare each against the numbers in the array.

* **Tracking the Logic & Finding Bugs:**
  * I set up an open loop to calculate `mul = k * i` and nested a second loop to search through `nums`.
  * During the process, I ran into a state bug where the boolean flag `found` was placed outside the loop. This meant once a multiple was found in the array, `found` stayed `true` permanently, preventing future missing numbers from ever being returned.
  * Moving `boolean found = false;` inside the loop ensured each multiple started with a clean slate.
  * I also realized that once a match is found in the array, adding a `break` immediately saves unnecessary comparisons.

---

### LeetCode 2129: Capitalize the Title

* **Breaking Down the Problem Requirements:**
  * The input is a full sentence, but the rules apply to individual words independently:
    * Length $\le 2$: complete lowercase.
    * Length $\ge 3$: first letter uppercase, rest lowercase.
  * To process each word, the first step is to split the sentence by spaces into an array of words (`title.split(" ")`).

* **Stepping Through Word by Word:**
  * Using a standard loop over the words array, I separated the logic into two clear branches based on `words[i].length()`:
    * For 1 or 2 letters: apply `.toLowerCase()` to the entire word.
    * For 3 or more letters: split the word conceptually into two parts—take the first letter (`charAt(0)`), uppercase it, then take everything from index 1 onwards (`substring(1)`) and lowercase it.

* **Formatting the Spacing:**
  * Joining the words back together requires spaces between words, but no trailing space at the very end.
  * By checking `if (i < words.length - 1)`, I ensured spaces were only appended after words that were not the final word.

* **Interview Reflection & Thought Structure:**
  * The ideal way to tackle string manipulation in an interview is:
    1. Clarify what needs to be isolated (words vs. characters).
    2. Split into clean chunks.
    3. Loop through and apply branch conditions based on length or constraints.
    4. Recombine cleanly while maintaining correct delimiters.
    5. Be mindful of string immutability in Java and transition from `ans += ...` to `StringBuilder` for $O(N)$ efficiency.

---

## Summary of Questions Solved

* **Total Questions Solved:** 2
  1. LeetCode 3718 — *Smallest Missing Multiple of K*
  2. LeetCode 2129 — *Capitalize the Title*

---

*See you on Day 42*

# Problem Solving & Metacognition Documentation — Day 42
**Date:** August 26, 2026  
**Day Number:** Day 42

---

## Thought Process & Problem Solving Journey

### LeetCode 705: Design HashSet

* **Initial Understanding & Unpacking the Problem:**
  * When I first looked at the problem, designing a "HashSet" from scratch sounded like it would require complex hash functions, bucketing, and collision handling.
  * But after reading the constraints carefully, I noticed that the keys are strictly between $0$ and $1,000,000$.
  * This was the key breakthrough: because the universe of keys is bounded and non-negative, I don't need a complex hash table—I can directly use a boolean array where the array index itself represents the key.

* **Working Through Confusions & Fixing Early Mistakes:**
  * **Mistake 1 (Self-Instantiating Class):** Early on, I wrote `MyHashSet myHashSet = new MyHashSet();` inside the class itself. I quickly realized this creates infinite recursion because the class *is* the data structure, not a wrapper holding another instance of itself.
  * **Mistake 2 (Hardcoded Values):** I initially thought about writing specific values like `myHashSet.add(1)`, but remembered that the method parameter `int key` gives us dynamic input that must be mapped directly: `set[key] = true`.
  * **Clarifying Store vs. Return:** I had a major conceptual hurdle around `set[key] = true`. I was confusing assigning state with returning a value. I realized that `add` and `remove` have a `void` return type—their only job is to update/store state in memory (`set[key] = true` or `false`). Only `contains()` needs to read and `return set[key]`.

* **Mental Model Summary:**
  * The index is the key itself.
  * `set[5] = true` means "number 5 exists in the set".
  * `set[5] = false` means "number 5 has been removed".
  * `return set[5]` tells the caller whether 5 is present or not.
  * Looking at constraints first simplifies what looks like a complicated design problem into direct array indexing.

---

## Summary of Questions Solved

* **Total Questions Solved:** 1
  1. LeetCode 705 — *Design HashSet*

---

*See you on Day 43*

# Learning Log — Day 43
**Date:** August 27, 2026  
**Day Number:** Day 43


* **didnt do anyhting today bcz to much tiredness

*See you on Day 44*

# Problem Solving & Metacognition Documentation — Day 44
**Date:** August 28, 2026  
**Day Number:** Day 44

---

## Daily Reflection & Rest Day Note

* **Daily Reflection:**
  * Today was fully dedicated to celebrating Raksha Bandhan with family, resulting in a very busy schedule throughout the day.
  * Taking planned or festival-related breaks is a normal part of maintaining long-term consistency and avoiding burnout across a daily streak.
  * The goal is to reset, recharge, and return to standard algorithmic problem solving with full focus tomorrow.

---

## Summary of Questions Solved

* **Total Questions Solved:** 0

---

*See you on Day 45*

# Problem Solving & Metacognition Documentation — Day 46
**Date:** August 30, 2026  
**Day Number:** Day 46

---

## Thought Process & Problem Solving Journey

### LeetCode 682: Baseball Game

* **Initial Understanding & Approach:**
  * When reading the rules, the operations naturally rely on recent history:
    * We frequently need the most recent score (`"D"` and `"+"`).
    * We occasionally need the second most recent score (`"+"`).
    * We need to remove the most recent score entirely (`"C"`).
  * Because every special rule refers strictly to the last entered elements, a **Stack** is the most natural and clean mental model.

* **Handling Stack Operations & The `"+"` Case:**
  * For `"C"`, a simple `pop()` removes the last score.
  * For `"D"`, `peek()` allows us to read the top without removing it, calculate double, and push it back.
  * The interesting case was `"+"`: we need both the top score and the one right below it. To get the second element without destroying history, I popped the top element, peeked at the second, pushed the top back, and then pushed their sum.
  * Any normal number string is parsed into an integer using `Integer.parseInt()` and pushed directly.

* **Final Summation Reflection:**
  * Once all operations are processed, whatever numbers remain on the stack represent the valid scores of the game.
  * Looping through the stack elements and summing them up gives the final answer cleanly.

---

## Summary of Questions Solved

* **Total Questions Solved:** 1
  1. LeetCode 682 — *Baseball Game*

---

*See you on Day 47*

# Problem Solving & Metacognition Documentation — Day 47
**Date:** August 31, 2026  
**Day Number:** Day 47

---

## Thought Process & Problem Solving Journey

### LeetCode 2351: First Letter to Appear Twice

* **Initial Intuition & The Stack Misconception:**
  * When I first saw the problem, my intuition went toward using a Stack or checking `current == previous`.
  * I thought: push characters and check if the incoming character equals the top.
  * However, dry-running an example like `"nwcn"` immediately exposed the flaw in that mental model:
    * A stack/adjacent check only detects **consecutive duplicates** (`"abcc"` where `'c'` is next to `'c'`).
    * It completely misses **non-consecutive repeats** (`"nwcn"` where `'n'` reappears after several other characters).

* **Mental Model Shift (Consecutive vs. Global History):**
  * I realized the fundamental question: *Do I only care about the adjacent previous element, or do I care about ANY prior occurrence across the entire prefix history?*
  * The problem requires finding if a character exists anywhere in the preceding sequence.

* **Developing the Prefix-Scan Approach:**
  * To check the entire preceding prefix, I designed a two-loop structure:
    * Outer loop: advances the current character $i$ from left to right.
    * Inner loop: scans all previously visited characters $j$ where $0 \le j < i$.
  * The exact moment $s[i] == s[j]$, we are guaranteed that $s[i]$ is the first character to reach a frequency count of 2 because the outer loop moves sequentially from left to right.
  * We can immediately return $s[i]$ without further checks.

* **Looking Ahead to Optimal Lookups:**
  * While the nested loop approach solves the problem cleanly in $O(1)$ extra memory, searching the past prefix costs $O(n^2)$ time.
  * In future problems involving prefix history checks, using a `boolean[26]` array or `HashSet` will allow us to check historical presence in $O(1)$ time per step.

---

## Summary of Questions Solved

* **Total Questions Solved:** 1
  1. LeetCode 2351 — *First Letter to Appear Twice*

---

*See you on Day 48*

# Problem Solving & Metacognition Documentation — Day 48
**Date:** September 1, 2026  
**Day Number:** Day 48

---

## Thought Process & Problem Solving Journey

### LeetCode 1748: Sum of Unique Elements

* **Initial Intuition & Early Obstacles:**
  * My first instinct was to compare the current element with preceding elements and add to the sum if no match was found.
  * I encountered several logic errors in that early attempt:
    * `j = 1` accidentally skipped the first element at index 0.
    * An early `return 0` terminated the whole algorithm as soon as any duplicate was detected anywhere.
    * Summing `nums[j]` directly risked repeated additions.

* **The Shift to Counting & The Prefix Trap:**
  * I adjusted the logic to use a `count` variable, incrementing it when duplicates were detected before index `i` (`0 <= j < i`).
  * However, dry running `[1, 2, 3, 2]` exposed the prefix trap:
    * At `i = 1` (the first `2`), looking only backwards showed `count = 0` (no preceding `2`), making it appear unique at that moment even though another `2` existed later in the array.
    * I realized: *Prefix history only tells if an element is repeated up to now; it cannot confirm global uniqueness.*

* **Global Frequency Realization:**
  * To determine if an element is truly unique, we must count its total occurrences across the entire array (`0 <= j < nums.length`).
  * If an element's total frequency across the entire array is exactly `1`, it is added to the running sum.
  * This cemented the core distinction: *Checking for historical duplication is not the same as verifying global uniqueness.*

---

## Summary of Questions Solved

* **Total Questions Solved:** 1
  1. LeetCode 1748 — *Sum of Unique Elements*

---

*See you on Day 49*

eq i$) to ensure the final array is either entirely even or entirely odd.
  * I wondered: *Can we always satisfy this condition, or is there an edge case that fails?*

* **Unpacking Parity Arithmetic:**
  * If the array is already all even or all odd, we do nothing and keep `nums2[i] = nums1[i]`. Condition satisfied.
  * If the array has mixed elements (both evens and odds):
    * Suppose we aim to make everything **odd**:
      * The odd numbers can stay untouched.
      * For any even number, we can subtract any available odd number: $	ext{even} - 	ext{odd} = 	ext{odd}$.
      * This flips every even number into an odd number!
    * Because we have at least one odd number in a mixed array, we can always transform every even number into an odd number.
  * Hence, regardless of the input array, it is always possible to construct a uniform parity array. Simply returning `true` satisfies the problem completely.

---

## Summary of Questions Solved

* **Total Questions Solved:** 2
  1. LeetCode 844 — *Backspace String Compare*
  2. LeetCode 3875 — *Construct Uniform Parity Array I*

---

*See you on Day 50*

# Problem Solving & Metacognition Documentation — Day 50
**Date:** September 3, 2026  
**Day Number:** Day 50

---

## Thought Process & Problem Solving Journey

### LeetCode 1544: Make The String Great

* **Understanding In-Place Mutation Challenges:**
  * Since `String` is immutable, handling continuous character removals requires a mutable buffer like `StringBuilder`.
  * To delete an adjacent pair, I used `sb.delete(i, i + 2)` because the end index is exclusive.
  * However, deleting elements shrinks the string dynamically and shifts subsequent characters left, which introduces boundary hazards.

* **Tracking the Index Shift and Edge Cases:**
  * **Lookahead Out-of-Bounds:** When accessing `i + 1`, loop termination must be `i < sb.length() - 1` rather than `<=`.
  * **The Cascade Reaction:** Removing a middle pair like `"bB"` in `"abBA"` merges previously non-adjacent characters (`"aA"`). To re-evaluate newly created pairs, I had to move the index backward (`i -= 2`).
  * **Negative Index Trap:** If the deletion occurs at index 0, moving backwards (`i - 2`) pushes `i` to `-2`. When the loop increments it to `-1`, accessing `sb.charAt(-1)` throws a `StringIndexOutOfBoundsException`.
  * Fixing this with `i = Math.max(-1, i - 2)` ensures the index stays safe while allowing proper re-evaluation.

---

### LeetCode 1598: Crawler Log Folder

* **Initial Intuition vs. Minimal State Realization:**
  * My immediate thought was to use a `Stack<String>` to simulate folder navigation:
    * `"d1/"` $\to$ push
    * `"../"` $\to$ pop
    * `"./"` $\to$ ignore
  * But before implementing, I stopped and asked myself: *Do I actually care about the folder names?*
  * The problem only asks for the number of steps required to return to the root folder, which is simply the current directory depth.

* **Simplifying from Stack to Counter:**
  * Storing names in a stack wastes memory when only depth is needed.
  * Replaced the stack with a single integer: `int depth = 0`.
  * Rule boundaries:
    * `"../"` $\to$ `if (depth > 0) depth--` (preventing negative depth below root).
    * `"./"` $\to$ no change.
    * `"x/"` $\to$ `depth++`.
  * This reduced space complexity from $O(N)$ down to $O(1)$.

---

## Summary of Questions Solved

* **Total Questions Solved:** 2
  1. LeetCode 1544 — *Make The String Great*
  2. LeetCode 1598 — *Crawler Log Folder*

---

*See you on Day 51*

# Problem Solving & Metacognition Documentation — Day 51
**Date:** September 4, 2026  
**Day Number:** Day 51

---

## Thought Process & Problem Solving Journey

### First Stable Index: Prefix Max & Suffix Min Stability

* **Problem Understanding & Strategy Selection:**
  * For each index $i$, the goal is to evaluate the instability score: $\max(\text{nums}[0 \dots i]) - \min(\text{nums}[i \dots n-1])$.
  * If this difference is $\le k$, index $i$ is stable.
  * Because the constraint is small ($n \le 100$), an $O(n^2)$ brute-force simulation checking each index independently is fully viable and easy to reason through.

* **Identifying and Correcting Implementation Pitfalls:**
  * **Variable Indexing Bug:** In my first attempt inside the inner loops, I accidentally used `nums[i]` instead of the iteration index `nums[j]` / `nums[l]`. I corrected this so that each loop accurately checks the current candidate element.
  * **Minimum Initialization Trap:** Setting `int min = 0;` caused a silent logic error because all values in `nums` are non-negative ($\ge 0$). A default of `0` would prevent `min` from ever capturing a higher actual minimum. Initializing `min = nums[i]` guarantees a valid baseline from the suffix range.
  * **Scope & Resetting:** Both `min` and `max` must be declared and reset inside the outer loop so that each candidate index $i$ starts with a fresh baseline.
  * **Sequential vs. Nested Scans:** I initially nested the suffix loop inside the prefix loop. I realized this was structurally incorrect: the prefix maximum and suffix minimum are independent calculations over separate ranges. They must run sequentially, and only after both finish should `ans = max - min` be computed.
  * **Return Value Clarification:** I initially wrote `return k;` out of habit, but caught myself—the problem asks for the *first stable index*, so returning `i` upon the first match (and `-1` if no index qualifies) is required.

* **Metacognitive Takeaway:**
  * When problem statements define metrics combining multiple ranges (e.g., prefix $0 \dots i$ vs. suffix $i \dots n-1$), break the process into distinct, sequential sub-steps:
    1. Scan left range.
    2. Scan right range.
    3. Evaluate boundary condition.
  * Always initialize extremum variables with elements from the actual domain rather than arbitrary zeroes when values can be positive.

---

## Summary of Questions Solved

* **Total Questions Solved:** 1
  1. *First Stable Index (Prefix Max & Suffix Min Stability)*

---

*See you on Day 52*

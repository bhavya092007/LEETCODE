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

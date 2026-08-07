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


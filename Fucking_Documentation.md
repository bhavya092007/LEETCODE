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

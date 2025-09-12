---
layout: essay
type: essay
title: "The Gen Z Stare"
# All dates must be YYYY-MM-DD format!
date: 2025-09-08
published: true
labels:
  - Questions
  - Answers
  - StackOverflow
  - Gen Z
---

<img width="300px" class="rounded float-start pe-4" src="../img/smart-questions/emoji.jpg">
Write a technical essay that discusses why smart questions are important for smart software engineers, how the chosen questions fulfill (or not) the precepts for smart questions, how the responses reflect the smartness (or lack thereof), and the insights you gained as a result of this experience. 


## The Gen Z Stare

So for those of you who are chronically online, like moi, you may have heard this new slang referered as... Tada, The Gen Z Stare! It's the type of look that beautifully encaptures that culminates dismay, stink eye, and apathy alto into a nicely wrapped gift of blank stares and fixed eyes. It's *the* stare that someone gives you when you ask a not so smart question. You know we've all been there like why is my printer not printing when you're not connected or will unplugging my ethernet improve my ping? 

The Gen Z stare is one of many ways that the world tries to remind you that, maybe just maybee... 
We should think before we ask so, onwards to the path

## What’s a smart question?

Low and behold to the holy grail of smart questions.. Stackoverflow! 
Now you many be asking what Stackoverflow is; it's essentially reddit for programmers, math enthusiasts, and anyone interested in coding! It's the place to be to ask questions about issues on coding or anything technical that you'd like more familiarity with. Now using this excellent website, I gathered some  examples of smart questions and well the opposite.. 

In the following example, we examine the components of a decent question. In this case, the asker is trying to figure out a way to get the date of the previous month in Python.

```
Q: What is the '-->' operator in C/C++?



After reading Hidden Features and Dark Corners of C++/STL on comp.lang.c++.moderated, I was completely surprised that the following snippet compiled and worked in both Visual Studio 2008 and G++ 4.4. I would assume this is also valid C since it works in GCC as well.

Here's the code:

#include <stdio.h>
int main()
{
    int x = 10;
    while (x --> 0) // x goes to 0
    {
        printf("%d ", x);
    }
}

Output:

9 8 7 6 5 4 3 2 1 0

Where is this defined in the standard, and where has it come from?

```

While the heading of his question could be better, it does convey what he’s trying to figure out. Usually something as brief as “python date of previous month” is what other users would enter in as search terms on Google, making it easily found. Another good thing about the question is that it’s not just a question. The asker shows what he or she has done and that he or she has put in some effort to answer the question. And while it may not be as important as the question itself, the asker shows courtesy, which does increase the chance of getting an answer.

```
A: datetime and the datetime.timedelta classes are your friend.

1. find today
2. use that to find the first day of this month.
3. use timedelta to backup a single day, to the last day of the previous month.
4. print the YYYYMM string you're looking for.

Like this:

 >>> import datetime
 >>> today = datetime.date.today()
 >>> first = datetime.date(day=1, month=today.month, year=today.year)
 >>> lastMonth = first - datetime.timedelta(days=1)
 >>> print lastMonth.strftime("%Y%m")
 201202
 >>>

```
 
The asker received six possible answers, and he or she was successful in inciting discussion from multiple users. The answers themselves were clear and were devoid of the rumored sarcasm and hostility of “hackers.” Since I myself have referenced this page and found it useful, I can confidently say that it is a good question.

## The foolproof way to get ignored.

While there are decent questions that benefit everyone, there are those one can ask to create an entirely different effect. In the following example, a user asks how he would, in short, create a desktop application with Facebook.

```
Q: Facebook Desktop Notifier

I am a beginner programmer that have never used anything other than what's included in a language.

I am trying to create a desktop application that notifies me anytime I get an update onfacebook. 
How should go about doing this? Thanks in advance.

edit Sorry I was not clear. Is there any way to make a DESKTOP application with facebook?
```

A simple “yes” would have answered the question, but we know that’s not the sort of answer he or she is looking for. Fortunately, someone kindly responded with a link to Facebook’s developer website. The asker should have done more research on his or her potential project. Then further down the road, he or she could have asked more specific and detailed questions that wouldn’t require a thousand-paged response for a sufficient answer.

## Conclusion

When we rely on others’ generosity and expertise to provide answers to our questions, it should hold that the question we ask should be one that leads to efficient and effective help that not only benefits us, but also the people we ask and others who might ask the same question in the future. Thus, if you have a question… make it a smart one! Asking questions may not always get you the best answer, but asking them in a way that will make others want to answer them will increase the success of finding a good solution and make it a positive experience on all sides.

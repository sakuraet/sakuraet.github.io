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

For those of you who are chronically online, like myself, you may have heard this new slang term referred to as... Tada, The Gen Z Stare! It's the type of look that beautifully encapsulates dismay, stink eye, and apathy all wrapped into a nicely packaged gift of blank stares and fixed eyes. It's the stare that someone gives you when you ask a not-so-smart question. We've all been there—asking things like "Why is my printer not printing?" when you're not connected, or "Will unplugging my ethernet improve my ping?"

*The Gen Z stare is one of many ways that the world tries to remind you that maybe, just maybe... we should think before we ask.*
So onwards to the path of enlightenment!

## What’s A Smart Question?

Lo and behold, the holy grail of smart questions: Stack Overflow!

Now you may be asking what Stack Overflow is—it's essentially Reddit for programmers, math enthusiasts, and anyone interested in coding! It's the place to be to ask questions about coding issues or anything technical that you'd like more familiarity with. Using this excellent website, I gathered some examples of smart questions and, well... the opposite.

For example, this question I found on stackoverflow is an example of a smart question: [click here!](https://stackoverflow.com/questions/1642028/what-is-the-operator-in-c-c)
```
Q: What is the '-->' operator in C/C++?

After reading [Hidden Features and Dark Corners of C++/STL](http://groups.google.com/group/comp.lang.c++.moderated/msg/33f173780d58dd20) on comp.lang.c++.moderated, I was completely surprised that the following snippet compiled and worked in both Visual Studio 2008 and G++ 4.4. I would assume this is also valid C since it works in GCC as well.

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

The header of this question allows users to clearly understand what the asker is trying to ask—it's clear and concise, practically the golden rule when asking questions. Moreover, they provide links to an article where they found the 'operator' --> and explain what they're referencing. This is great as it allows users to gain context about the question. They also provide both the output and input to demonstrate their confusion, and end with a brief recap question. I think this question is a great example of a smart question, as there's no ambiguity without over-explaining.

```
A:
--> is not an operator. It is in fact two separate operators, -- and >.

The code in the condition decrements x, while returning x's original (not decremented) value, and then compares the original value with 0 using the > operator.

To better understand, the statement could be written as follows:

while( (x--) > 0 )

```

The asker received 26 replies and this is one of the most visited threads in all of Stack Overflow with over 1 million views total. So yeah, I think they deserve the golden star for asking a smart question. Not only that, but this asker was able to help out their community as well, as multiple sub-threads have spread from this question asking about syntax in C.

## How The Digital Salem Witch Trials Starts

While Stack Overflow may be considered one of the last hubs for civil discourse and an 'intelligent fanbase/userbase,' sometimes users get the wrong memo on how to conduct their questioning on this website. Here's a good example: a question asked the day I wrote this essay that somehow managed to already get 3 downvotes and not a single upvote. [Click here](https://stackoverflow.com/questions/79762561/c-capitalize-each-word) if you think I'm lying to you!

```
Q: C capitalize each word


I try to run , but there no output after I put any input, can check for me pleasee, im beginner btw

Task: (Create a function that capitalizes the first letter of each word and converts all other letters to lowercase. A word is a sequence of alphanumeric characters

My code:

 13 #include <unistd.h>
 14 
 15 int     alphanum(char c)
 16 {
 17         if (c >= 'a' && c <= 'z')
 18                 return (1);
 19         else if (c >= 'A' && c <= 'Z')
 20                 return (1);
 21         else if (c >= '0' && c <= '9')
 22                 return (0);
 23         else
 24                 return (0);
 25 }
 26 
 27 char    *ft_strcapitalize(char *str)
 28 {
 29         int     i;
 30 
 31         i = 0;
 32         while (str[i])
 33         {
 34                 if (i == 0 || !alphanum(str[i - 1]))
 35                 {
 36                         if (str[i] >= 'a' && str[i] <= 'z')
 37                                 str[i] = str[i] - 32;
 38                 }
 39                 else
 40                 {
 41                         if (str[i] >= 'A' && str[i] <= 'Z')
 42                                 str[i] = str[i] + 32;
 43                 }
 44                 i++;
 45         }
 46         return (str);
 47 }

I try put one word, it can be run , but after i put more than 1 word, no output, guide me please

```
Not only is it clear that this question was never revised (as shown from its numerous spelling and grammatical errors), it also just doesn't make sense. As the reader, I spent over three times reading this and I'm still confused about what they would like help with. In cases like these, better judgment is needed to not only proofread your question but also to provide clear context about what exactly isn't working and what you've already tried to debug the issue.

## My Hot Take

Asking smart questions is more than just a way to get faster and better answers—it is a habit that shows professionalism and reflects that you're a highly functioning developer. By asking smart questions, you ensure others know that you have already invested thought and effort before seeking someone else's advice. This makes you more appealing to work with, as people will believe you actively collaborate and aren't just putting off your work onto others.

Even online communities like Stack Overflow share this responsibility and maintain high standards when it comes to asking questions. Asking good questions will not only make your answers more accurate and quick, but will also provide the community of future engineers with quick solutions to an array of problems. On the other hand, if you structure your questions poorly, it will waste everyone's time and even lead to confusion and additional back-and-forth. This can be extremely frustrating for both parties, and in a professional setting, will cause problems in communication and lead people to believe you are an incompetent worker.
The bottom line? Think before you ask, and save yourself from receiving the dreaded Gen Z stare.

*Oh and of course ChatGPT helped with checking for grammatical and spelling errors!*

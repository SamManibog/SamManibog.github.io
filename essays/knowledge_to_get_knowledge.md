---
layout: essay
type: essay
title: "You Need Knowledge to Get Knowledge"
# All dates must be YYYY-MM-DD format!
date: 2025-09-07
published: true
labels:
  - Questions
  - Communication
  - StackOverflow
---

<img class="img-fluid" src="../img/knowledge-to-get-knowledge/question_discussion.png">

## The Necessity of Inquery

The human brain loves to learn. It’s deeply attracted to novelty, and that’s the reason why we ask questions about our world. As software engineers in an ever-changing landscape, we *need* to learn. It’s not enough to stick to a single version of library, language, or compiler; to stay afloat, we must be constantly adapting. The first part of this process is inquiry: “What must I learn?”, “Why does this work?”, and “How do I fix this incessant bug in my code?”.

## How to ask the Wrong Questions

It is often said that there are no stupid questions. However, this is a half-truth. There are no stupid questions to ask, but there *are* stupid questions to ask someone else. One of the most popular places to ask programming questions is Stack Overflow, so let’s explore some examples of what not to do.

### Case Study: A Bad Question to Ask Somebody

Here’s the [question](https://stackoverflow.com/questions/44674997/or-c-struct-accessor):

Title: *'.' or '->' C struct accessor [duplicate]*

*What is the difference between `.` and `->` when accessing data in a C structure? I couldn't find any difference in my several attempts. Both provide me access to the desired data.*

<hr>

While this question is certainly relevant to C programming and its answer is necessary to understand C’s syntax, it is not deserving of anyone’s time or response. The first problem with this question is that it doesn’t require a person to answer it. A quick Google search will tell you the answer. Even worse, this question has been flagged as a duplicate. A search within the same forum would have led to the answer they sought.

The second problem with this question is the lack of detail. The user states they “couldn’t find any difference in my several attempts”, but does not describe the attempts being referenced. Did they attempt to compile and/or run code? Did they attempt to search for the answer online and not find anything? (Doubtful.) Did they review examples and not understand the difference? Whatever the case, including this information would certainly help those responding to the question.

These points are further proved by the responses to the thread: “What does your data look like? What does your struct look like? Could you give a minimal example?” or “What does the textbook tell about these operators?” In general, questions like these are often the source of frustration and wasted time. Before deciding to delegate the problem to someone else, you should first do your homework and attempt to solve or understand the problem yourself. Not only will this anger fewer people, but I find that a question that you solve is more thoroughly understood than one with the answer handed to you.

### Case Study: A Poorly Posed Question

Not only is it important to know what questions to ask, but we must also understand how to ask them effectively. Take [this](https://stackoverflow.com/questions/59851613/why-does-my-code-does-not-work-even-though-it-is-correct) thread from Stack Overflow as an example on how not to ask a question:

Title: *Why does my code does not work even though it is correct?*

*This is the part of my code. It has 0 errors and 0 warnings but it does not work. It is completely correct. But it does not work.*

[The user provides a snippet of their C code including a struct and a main function].

<hr>

Problem number one is obvious from the title: a lack of humility. The attitude with which you pose the question is just as important as the content of the question itself. By including the words “even though it is correct,” this user has invited a host of understandably sassy comments that contribute nothing to his search for an answer. This problem is only worsened by the fact that multiple responders found that “0 errors and 0 warnings” was not accurate. Even if you are frustrated by a problem, do not let emotions mar your question.

The next problem is that this question is vague. How can we know if our code “does not work” if we don’t know what it’s supposed to do? When asking a question about code, you must explicitly communicate what you are trying to accomplish and where or how the code is failing. This may include providing code, its intended output, and the actual output. Since the user provided neither, the answers to this thread all required the responding developers to guess the intended behavior, which can lead to unproductive “answers:”.

## How to Seek and Find

So what does a good question look like? If bad questions will withhold me from answers, how can I ask questions so that I will learn as much as possible? Let’s go through one more example, but this time we will examine a good question.
[This](https://stackoverflow.com/questions/11227809/why-is-processing-a-sorted-array-faster-than-processing-an-unsorted-array) is the highest scored question on Stack Overflow:

Title: *Why is processing a sorted array faster than processing an unsorted array?*

*In this C++ code, sorting the data (before the timed region) makes the primary loop ~6x faster. Without `std::sort(data, data + arraySize);`, the code runs in 11.54 seconds. With the sorted data, the code runs in 1.93 seconds.*

[The user provides a code snippet in C++]

*Initially, I thought this might be just a language or compiler anomaly, so I tried Java, with a similar but less extreme result.*

[The user provides the previous code snippet, rewritten in Java]

*My first thought was that sorting brings the data into the cache, but that's silly because the array was just generated. What is going on? Why is processing a sorted array faster than processing an unsorted array? The code is summing up some independent terms, so the order should not matter.*

<hr>

The first comparison to make with this question and the others is its length. You may think that a short question is faster to read and therefore easier to answer, but that is not the case. Good questions are concise, not short. They include all necessary details while excluding unnecessary ones. Be sure to state the facts, and don’t cloud the question with filler.

Another thing that sets this question apart is that the user has clearly done their homework. They reference and provide the results from multiple tests that they performed within the question to provide context. This means that the question is contributing to the discussion rather than simply initiating it.

Furthermore, this question can’t be solved by a Google search. Rather than ask about information found in language references or documentation, this question inquires about deeper, conceptual knowledge. That isn’t to say that non-conceptual questions are bad, but to highlight that it's more considerate and efficient to find existing information than to interrogate another person for it.

This question is written very well, and it shows. Besides the high rating (which is meaningless in the grand scheme of things), it succeeds in creating a discussion where understanding can be reached. When you read through the answers and comments you are met with in-depth essays, details, and clarifications, not only because the question is clear, but because its author presented it as a question worthy of answering.


<hr>


Whenever you ask questions, simply posing them is not enough. You must do your due diligence to attempt to find an answer yourself, and only then should you begin to draft a question. When you write a question, your goal should not be limited to arriving at a cut-and-dried solution, but to create a meaningful discussion about an issue and its possible solutions.

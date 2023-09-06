---
layout: essay
type: essay
title: Asking Smart Questions
date: 2023-9-5
published: true
labels:
  - Software Development
  - StackOverflow
---

Developers will get stuck working on a problem eventually. They spend long nights debugging something that just looks right. As a last resort, developers turn to the web or AI for help. Most developers likely are able to filter out a well crafted StackOverflow post at a glance. The shape of the title, description, and answers give off enough information such that they know whether to click off or keep reading. Well made StackOverflow posts feel amazing to encounter, and literally nobody wants to waste their time reading and or answering a low effort post. Here we will go through 2 posts to demonstrate both how to ask smart questions and how to waste people's time. We will also go over the importance of asking smart questions for software engineers.

1. Well crafted question: <a href="https://stackoverflow.com/questions/5240789/scanf-leaves-the-newline-character-in-the-buffer">scanf-leaves-the-newline-character-in-the-buffer</a>
2. Poorly crafted question: <a href="https://stackoverflow.com/questions/77049525/anyone-help-me-how-to-solve-this-problem">anyone-help-me-how-to-solve-this-problem</a>

The first thing everyone sees is the title. Can you even tell what the second question is asking for? Why would you make me work harder to understand your problem. The difference between this and the well crafted question is that at least there is enough context to get an idea of the problem. Anyone who has worked with C for a bit can recognize the problem that the person is encountering at a glance and is able to dive a bit further to answer them. Of course, not every title can capture the entire context, but enough to be meaningfully identifiable. This is important especially for when people search for answers because if by some miracle someone answers a poorly worded post, they might not even find the thread due to the title. 

The description is important to get right because too much content will leave the reader overwhelmed, whereas too little content might leave the reader unable to diagnose your problem and solve it. The most important part of the description to get right is to:
1. Lean towards precision over volume
	1. Copy pasting things that obviously are unrelated to the question will only bloat your post. Make sure to double check whether what you are pasting is relevant to the problem
	2. You don't want to distract from your question by including comments such as "I'm stupid for not knowing how to solve this, hopefully someone can help."
2. Describe your goal and the symptoms/errors
	1. If the reader doesn't know what you are trying to achieve, it's extremely difficult for them to help. They cannot read your mind. Communicate what your end goal is and share the symptoms or errors you are running into
3. Ask explicit questions
	1. Questions like: "help pls?" are not as helpful. Try your best to ask as precise a question as you can such as the one shown in the well crafted question.

Note that in the poorly crafted question, it violates the explicit questions rule. It is also clear that this person copy pasted a problem they were trying to solve without giving their attempt at it. They basically assigned the internet their homework. I don't know who would want to spend their time answering this question.

Now lets take a look at the well crafted question. They explicitly cite a resource they used and is asking an explicit question about the correctness of the resource. They described the exact symptoms of using scanf in the code they shared. Also they are precise and address the problem directly in their description. This example is great for demonstrating how to ask smart questions.

Asking smart questions for developers is extremely important, both for the asker and the answerer. Developers must work with complex systems that need precise language to both describe the problem and prescribe a solution. A quick scroll through StackOverflow's New Questions section shows that it's actually quite rare to encounter a smart question. The next time you post a question or ask someone in person, think about these rules above to ensure you get the best answers. Ask smart questions, get smart answers.
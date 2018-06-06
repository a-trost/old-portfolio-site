---
title: Two Ways to Make Teaching Better With Code
category: "EdTech"
cover: cover.jpg
author: Alex Trost
---
I've been a teacher for 4 years and have tried dozens of software solutions aimed at teachers and classrooms. It’s painfully clear that teachers are in need of better computer support. We need to move past code that just does flash card review or attendance taking, but software that actually makes the job of the teacher better.

The act of teaching is incredibly hard work on its own. Figuring out what each individual student needs to learn next to help them catch up, keep going, or stay ahead takes a great deal of work and understanding of how students learn. 

## 1. Fix the Information Overload
I've never heard a teacher complain of not having enough data.
>"We don't give enough tests!"

...said no teacher in the past 10 years.

Teachers get an overflow of data from standardized tests, unit tests, book tests, quizzes, worksheets, small group work, homework, etc. Teachers need to be efficient and effective at actually using all that data. Often times, it can be a herculean task. 

### Keeping up with Test Data
Many computer tests like the [NWEA Map](https://www.nwea.org/) go in-depth and return specifics on precisely where a student stands. Information on what the student knows and what they need to know next is returned to the teacher.

"Great!" you might be thinking. "Now you know exactly what you need to teach next."

The problem lies in the fact that teachers receive over a hundred "next things" per student. 

Over 100 Items **x** Every Student = Data Paralysis

[Across business, researchers estimate that up to 73% of collected data is never successfully used.](https://www.forbes.com/sites/tomaslaurinavicius/2017/11/01/risk-too-much-data/#57175cda44b3) Education probably isn't much different. 


Also, tests like the NWEA Map provide a *snapshot*, as it's only given 2-3 times a year. Students are learning daily, so with each passing day the data grows stale until, like last year's shoes, it doesn't fit the 2nd grader. 

**This is something that can be remedied through better code.**

Software that quickly maps every bit of student data to the Common Core State Standards would likely be the best solution to the problem. 

The teacher enters Timmy's results from today's math test. The app knows that question #3 is assessing for the following standard:
> CCSS.MATH.CONTENT.2.NBT.A.1.A
>100 can be thought of as a bundle of ten tens — called a "hundred."

It updates Timmy's profile with this new data point. Because Timmy has been tested on this in the past, it combines this data with Timmy's homework and classwork data to get the full profile. The app checks for growth or mastery. It recommends next steps to the teacher.

This kind of deep dive is tough and time consuming to be done by hand for each standard and each child. Computers can simply do it better.
## 2. Make Practice Apps Smarter

Computer practice adds a great layer of immediate feedback over the pencil and paper work that has been the standard for decades. However, we've had immediate feedback since the days of Number Munchers, and modern math apps should be doing so much more.
![Number Munchers Screenshot](/content/images/2018/03/number_munchers.gif) 
### Misconception Correction
If a student is adding incorrectly, it is the teacher’s job to determine not just that the problem is wrong, but why it is wrong. 

What's the misconception that the student has about solving this kind of problem? Do they not understand place value? Are they subtracting instead of adding? 

Teachers use this information to correct the misconception, targeting that specific error and clearing it away. 

Most math applications I’ve seen only give a boolean response. If the student gets it right, great, let’s move on (without much care for whether or not the student used an efficient strategy or counted to 72 on her fingers). 

If the student gets it wrong, a good app will give a detailed breakdown of how to solve the problem, but still give the same explanation no matter what the student’s given answer was. 

Smarter programs would be able to break these mistakes into categories and remediate the student accordingly. It’s a bit of extra leg work, but not too much. Most math programs give the student randomly generated numbers within a certain range, depending on the skill. 

A second grader working on 2 digit plus 2 digit numbers might get the problem `35+58`. The program will calculate the answer and compare the student’s answer against it. 
<pre><code class="language-python">if student_answer == answer:
	return True
else:
		return False
</code></pre>

If the student types `93`, great! She’s got it. But there are so many reasons a student might input a different number, and a few extra if statements would catch and quickly remediate those errors.

<pre><code class="language-python">if student_answer == answer:
	return “Correct!”
elif student__answer == addend2 - addend1:
	return “Careful! You subtracted when you should be adding.”
elif student_answer == (answer+1) or student__answer == (answer-1):
	return “Careful! You were just one off. Double check your work.”
</code></pre>

Much of the learning process in math comes when a student compares their incorrect answer to the correct one, has an 💡 “OHHH!” realization, and solidifies some new learning. Unfortunately, left to their own devices, many students would rather get a problem wrong time after time than stop and reflect on why they were wrong and fix it themselves. 

Trust me on this one.

These students that need a bit more guidance would benefit greatly from an app that can target their misconceptions that specifically. 

### Second Chances
Another aspect I don’t see enough is the opportunity to correct an answer and try again. This involves the program not giving them the answer, but instead just giving a “Not quite! Try again or click here for a hint.” sort of message. 

Khan Academy does this beautifully, but unfortunately it seems to be the exception rather than the rule. 

Second chances give the student a chance to make their work correct, perhaps for a half point or whatever metric the app is tracking. Almost as important: it teaches them that going back and fixing mistakes is an incredibly valuable skill and habit to get into.

## The Future
With machine learning exploding right now, I don't think we're far off from detailed 'learner profiles' for each student. Software that can continually probe and adapt to student progress and learning styles is a teacher's dream.

I realize (and hope) that I haven't seen it all. If you know of any great apps that are solving the problems I've outlined, let me know about them! I'm always on the lookout for a better way to teach. 
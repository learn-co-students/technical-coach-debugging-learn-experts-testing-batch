# Debugging
When you're working with student questions related to test errors, it's important that you first are able to look at the problem, deconstruct, and debug it. Once you do that, then you can transfer the same process (**process and not answer**) to students.

## Error Messages and the Lab

Always ask students to show you the error message first. Read through it and understand what the error is. If the student doesn’t already understand, tell them that error messages are great because they show you the exact reason(s) and location of why your program isn't working the way that you want it to. Error messages get you one step closer to solving the problem in front of you and most of the time, they're specific.

Make sure the student understands how to read the stack trace below an error message to see the path through their code that led to the error.

Now ask students to show you the code block that is relevant to the error message. Use the following debugging strategies to see if you can figure out what's happening. If you can't from the given code block, then ask them to show you the whole code.

From reading the error message, can you tell what the correct expected behavior is and what the error is? If so, great.

If you’re not clear on the error AND the solution to the error from the limited snippet, ask the student to push their code with `learn save` and you can click on the fork icon in Expert Chat to go their repo

![Student Repo Link](https://s3.amazonaws.com/learn-experts/student-repo-link.png)

If you're on dispatch and it isn't immediately clear from the code and error messages where the problem is, this is a good time to ask the student: "Would you like to pair program with a Technical Coach for 20 minutes?" If they say yes, feel free to continue working with the student while they wait.

Make sure that you understand all the steps necessary to solve this. What are the inputs and the outputs of the code? This might mean that in addition to the student's code, you will also need to read the Readme of the lab first and make sure that you know holistically what's expected.

Now break the problem of the lab into the smaller components necessary to solve it.

## Breaking Down Student Code

When looking at each method, you should know what the method does, what the inputs are, what the expected outputs are, and any edge cases. This makes it easier to discover what went amiss and what the bug is.

For example, you can start debugging by tracking the value of your variables. You may find that variables in the student's code don't hold the values that they expect, or that they don't hold any value at all. There are several ways to examine the values your variables hold (IRB, pry, console, debugger, etc.).

If you have the time, always run the student's code to make sure that your assumptions are correct. Test the solution too to make sure that it works. In some cases, there may be a totally different bug that you weren't aware of.

If you get stuck and you’re not sure _what_ the bug is, you can compare the student’s code to the solution branch. (An easy way to do this is with `git diff master solution`).

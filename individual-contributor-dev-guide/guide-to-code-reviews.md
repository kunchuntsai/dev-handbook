# Guide to Code Reviews

> [!TIP]
> **TL;DR**
> - Reviewing test results and running tests
> - Reviewing code style
> - Communicating changes

### Content

Understand the [concept](https://google.github.io/eng-practices/review/reviewer/standard.html) and [full picture of a code review](https://google.github.io/eng-practices/review/reviewer/looking-for.html)

1. Understand how to [write good CL descriptions](https://google.github.io/eng-practices/review/developer/cl-descriptions.html)
2. Understand how to [navigate a CL in review](https://google.github.io/eng-practices/review/reviewer/navigate.html)
3. Understand how to [write code review comments](https://google.github.io/eng-practices/review/reviewer/comments.html)
4. Understand how to [handle pushback in code reviews](https://google.github.io/eng-practices/review/reviewer/pushback.html)

For a deeper review, please check out [Clean Code](../learning-resource/clean-code.md)

### Introduction

[Code Review Developer Guide](https://google.github.io/eng-practices/review/)

- [How To Do A Code Review](https://google.github.io/eng-practices/review/reviewer/): A detailed guide for code reviewers
- [The CL Author's Guide](https://google.github.io/eng-practices/review/developer/): A detailed guide for developers whose CLs are going through review.

### The Standard of Code Review

[The Standard of Code Review](https://google.github.io/eng-practices/review/reviewer/standard.html)

In general, reviewers should favor approving a CL once it is in a state where it definitely improves the overall code health of the system being worked on, even if the CL isn't perfect.

- Mentoring
- Principles
- Resolving Conflicts

### What Do Code Reviewers Look For?

[Introduction](https://google.github.io/eng-practices/review/#look_for)

[What to look for in a code review](https://google.github.io/eng-practices/review/reviewer/looking-for.html)

Code reviews should look at:

- Design: Is the code well-designed and appropriate for your system?
- Functionality: Does the code behave as the author likely intended? Is the way the code behaves good for its users?
- Complexity: Could the code be made simpler? Would another developer be able to easily understand and use this code when they come across it in the future?
- <ins>**Tests: Does the code have correct and well-designed automated or manual tests?**</ins>
- Naming: Did the developer choose clear names for variables, classes, methods, etc.?
- Comments: Are the comments clear and useful?
- Style: Does the code follow our style guides?
- Consistency: What if the existing code is inconsistent with the style guide?
- Documentation: Did the developer also update relevant documentation?
- Every Line: Did the reviewer review every line of code you've been asked to review?
- Context: Did the reviewer think about the CL in the context of the system as a whole?
- Good Things: Did the reviewer offer encouragement and appreciation for good practices?

### Navigating a CL in review

[Navigating a CL in review](https://google.github.io/eng-practices/review/reviewer/navigate.html)

1. Does the change make sense? Does it have a [good description](https://google.github.io/eng-practices/review/developer/cl-descriptions.html)?
2. Look at the most important part of the change first. Is it well-designed overall?
3. Look at the rest of the CL in an appropriate sequence.

Step One: Take a broad view of the change

Step Two: Examine the main parts of the CL

Step Three: Look through the rest of the CL in an appropriate sequence

### How to write code review comments

[How to write code review comments](https://google.github.io/eng-practices/review/reviewer/comments.html)

- Be kind.
- Explain your reasoning.
- Balance giving explicit directions with just pointing out problems and letting the developer decide.
- Encourage developers to simplify code or add code comments instead of just explaining the complexity to you.

### Handling pushback in code reviews

[Handling pushback in code reviews](https://google.github.io/eng-practices/review/reviewer/pushback.html)

Sometimes a developer will push back on a code review. Either they will disagree with your suggestion or they will complain that you are being too strict in general.

- Who is right?
- Upsetting Developers
- Cleaning It Up Later
- General Complaints About Strictness
- Resolving Conflicts

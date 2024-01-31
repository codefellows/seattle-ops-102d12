<!-- .element class="main-title" -->
# Ops 102: Intro to Computer Operations

Class 01

NOTE:
DO:
- Introduce yourself
- Take attendance
- Start Zoom cloud recording

SAY:
- Welcome to Ops 102! In this course, we will prepare you and your cyber range to be successful in the upcoming Ops 201 course and beyond.
- By the end of this course, you will:
  - understand the core building blocks of computing
  - have your own home lab capable of virtualization
  - develop proficiency in installing software in Linux
  - gain valuable hands-on experience with computer hardware internals and peripherals
  - be fully prepared for the challenges ahead in Ops 201
  - be a part of a learning community, and begin to prepare your resume and professional skills for an in-demand technical career
- But first, let's make sure we are ready for our first day!

---

<!-- .element class="title-and-subtitle" -->
<div>

# Ops 102 Checklist

- Get connected in the class Slack channel <!-- .element: class="fragment" data-fragment-index="1" -->
- Join Ops 102 on Canvas <!-- .element: class="fragment" data-fragment-index="2" -->
  - Look for your invite in your email inbox. <!-- .element: class="fragment" data-fragment-index="3" -->
  - Bookmark this site! <!-- .element: class="fragment" data-fragment-index="4" -->
  - Have you turned in your prework yet? <!-- .element: class="fragment" data-fragment-index="5" -->
- Your personal computer meets the <!-- .element: class="fragment" data-fragment-index="6" -->[requirements](https://www.codefellows.org/faq/#computer-requirements).
- Your lab kit meets the <!-- .element: class="fragment" data-fragment-index="7" -->[requirements](https://codefellows.github.io/common_curriculum/prework/computer-setup-ops).

</div>

NOTE:
DO: Make a list of everyone who needs to be followed up on and return to this list after lecture.

---

<!-- .element class="split-screen-with-title" -->

# Lab vs Personal Machines Slide

<div>

<div>

**Personal Computer**
  - Your personal computer is the machine you will be doing all your work on after 102.<!-- .element: class="fragment" data-fragment-index="1" -->
  - You will use this machine to remotely log into your lab computer in order to create virtual machines and complete lab and challenge assignments.<!-- .element: class="fragment" data-fragment-index="2" -->
  - Your personal computer is how you will attend lecture, collaborate with others and communicate with your instructors.<!-- .element: class="fragment" data-fragment-index="3" -->
  - You will also complete your reading and career coaching assignments on your personal computers.<!-- .element: class="fragment" data-fragment-index="4" -->

</div><!-- .element class="medium-text" -->

<div>

**Lab Kit**
  - The lab kit is made up of a computer, a monitor, a keyboard, a mouse, a router, plus a few other handy tools. <!-- .element: class="fragment" data-fragment-index="5" -->
  - The tower, monitor, keyboard and mouse make up your "lab computer". <!-- .element: class="fragment" data-fragment-index="6" -->
    - This lab computer is a safe place for you to experiment and learn without the concern of accidentally creating any lasting damage. <!-- .element: class="fragment" data-fragment-index="7" -->
    - You will perform tasks on your lab computer that are only allowed with the owner's permission. <!-- .element: class="fragment" data-fragment-index="8" -->
- HINT: "machine", "PC" and "computer" can be used interchangeably. <!-- .element: class="fragment" data-fragment-index="9" -->

</div><!-- .element class="medium-text" -->

</div>

NOTE:
SAY:
  - The lab kit is made up of a computer, a monitor, a keyboard, a mouse, a router, plus a few other handy tools.
  - The tower, monitor, keyboard and mouse make up your "lab computer".
    - This lab computer is a safe place for you to experiment and learn without the concern of accidentally creating any lasting damage.
      - Virtual computers will be utilized on the lab computer in order to protect the host operating system.
      - If something goes wrong, the student can simply delete the broken virtual computer, create a new one and try again.
    - You will perform tasks on your lab computer that are only allowed with the owner's permission.
- HINT: "machine", "PC" and "computer" can be used interchangeably.

---

<!-- .element class="main-title" -->
# Ops 102 Overview

NOTE:
SAY:
- What is the objective of Ops 102?
  - Get to know your lab kit PC and deploy a basic homelab.
- Let’s take a look at what to expect in this course.

---

<!-- .element class="split-screen-with-title" -->

# Ops 102 Overview

<div>

<div>

  - Class 01: What is a computer? <!-- .element: class="fragment" data-fragment-index="1" -->
  - Class 02: Build a computer <!-- .element: class="fragment" data-fragment-index="2" -->
  - Class 03: Startup sequence and BIOS <!-- .element: class="fragment" data-fragment-index="3" -->
  - Class 04: Operating Systems <!-- .element: class="fragment" data-fragment-index="4" -->
  - Class 05: Install Virtualbox <!-- .element: class="fragment" data-fragment-index="5" -->

</div>

<div>

  - Class 06: SOHO Networking <!-- .element: class="fragment" data-fragment-index="6" -->
  - Class 07: Network Connectivity <!-- .element: class="fragment" data-fragment-index="7" -->
  - Class 08: Windows OS Virtualization <!-- .element: class="fragment" data-fragment-index="8" -->
  - Class 09: Basic Windows Operations <!-- .element: class="fragment" data-fragment-index="9" -->
  - Class 10: 201 Entrance Exam <!-- .element: class="fragment" data-fragment-index="10" -->

</div>

</div>

![Image](/ops-102-guide/curriculum/class-01/slides/assets/3_1.png)<!-- .element class="small" -->

NOTE:
SAY:
- Today we'll be exploring what a computer is, how it works, and some of the fundamental processes a computer performs at the most basic level.
- Throughout this course we'll examine computers at their lowest level of operations.
- We'll work with computer hardware the first two classes, then start working with the bootup sequence before installing a new Ubuntu OS onto our lab computers.
- Then we'll pivot over to networking where we'll set up a SoHo router and remote connection.
- And finally, we introduce virtualization and finish up Windows operations and security settings before we take the 201 Entrance Exam.

---

<!-- .element class="split-screen-with-title" -->
# Agenda

<div>

<div>

- Welcome to Ops 102 <!-- .element: class="fragment" data-fragment-index="1" -->
  - Introduce Yourself! <!-- .element: class="fragment" data-fragment-index="2" -->
  - How You Will Learn <!-- .element: class="fragment" data-fragment-index="3" -->
  - Intro to Resources <!-- .element: class="fragment" data-fragment-index="4" -->
    - Canvas <!-- .element: class="fragment" data-fragment-index="5" -->
    - Zoom <!-- .element: class="fragment" data-fragment-index="6" -->
    - Slack <!-- .element: class="fragment" data-fragment-index="7" -->
  - The Learning Pit <!-- .element: class="fragment" data-fragment-index="8" -->
  - Growth Mindset <!-- .element: class="fragment" data-fragment-index="9" -->
  - Professional Ethics and Integrity <!-- .element: class="fragment" data-fragment-index="10" -->
  - GitHub and Wikis <!-- .element: class="fragment" data-fragment-index="11" -->

</div>

<div>

- VS Code and Markdown <!-- .element: class="fragment" data-fragment-index="12" -->
- What is a Computer? <!-- .element: class="fragment" data-fragment-index="13" -->
  - Computer Components <!-- .element: class="fragment" data-fragment-index="14" -->
  - Stages of Computing <!-- .element: class="fragment" data-fragment-index="15" -->
  - Levels of Abstraction <!-- .element: class="fragment" data-fragment-index="16" -->
  - Circuits & Logic <!-- .element: class="fragment" data-fragment-index="17" -->
  - Binary & Data <!-- .element: class="fragment" data-fragment-index="18" -->
- Inside a Computer <!-- .element: class="fragment" data-fragment-index="19" -->
  - Disassembly <!-- .element: class="fragment" data-fragment-index="20" -->
- Lab assignment <!-- .element: class="fragment" data-fragment-index="21" -->
- Open Lab Time <!-- .element: class="fragment" data-fragment-index="22" -->

</div>

</div>

NOTE:
SAY: Here's our plan for class today.

---

<!-- .element class="title-and-subtitle" -->

# Introductions

<div>

- How shall we refer to you? Name/pronoun/nickname... <!-- .element: class="fragment" data-fragment-index="1" -->
- What's your background and where are you from? <!-- .element: class="fragment" data-fragment-index="2" -->
- What would you like to gain from this workshop? <!-- .element: class="fragment" data-fragment-index="3" -->

</div>

![Image](/ops-102-guide/curriculum/class-01/slides/assets/6_0.png)<!-- .element class="small" -->

NOTE:
DO:
- Introduce yourself with your professional pitch.
- To avoid this taking too much time, try to set expectations so that each students will spend no more than 15-20 seconds answering the above questions.
- Facilitator calls on each person to answer the questions on the slide, and at the same time identifies who will be up next
  - “Courtney, you are up. And then we will hear from David.”


---

<!-- .element class="title-and-text" -->

<div>

# How You Will Learn

- Path learning is a style of education that is closely guided, making students consumers of information and creating dependency. <!-- .element: class="fragment" data-fragment-index="1" -->
  - The goal: An exchange of information <!-- .element: class="fragment" data-fragment-index="2" -->
- Sandbox learning instead fosters exploration, making students co-creators of their own learning experience. <!-- .element: class="fragment" data-fragment-index="3" -->
  - The goal: Learning and discovery <!-- .element: class="fragment" data-fragment-index="4" -->

</div>

![Image](/ops-102-guide/curriculum/class-01/slides/assets/7_0.png)<!-- .element class="small" -->

NOTE:
SAY:
- Today you’ll have different learning experiences. Some portions of the class will be what we call “path” learning:
  - We’ll show you how to do something, and you can follow along and replicate what we do.
- Other portions of the class are what we call “sandbox” learning:
  - We’ll give you a task with a few guidelines (think of these as the sides of the sandbox), and then what you do and learn within those guidelines is up to you.
  - In sandbox learning, students are provided with a safe and supportive environment where they can explore and experiment with concepts, ideas, and skills through direct experience.
- You may recall that the experience of a sandbox environment can feel overwhelming and uncomfortable at first. That’s okay!
- Sandbox learning promotes critical thinking, problem-solving skills, collaboration, and creativity.
  - It encourages students to take risks, learn from their mistakes, and iterate on their ideas.
  - By providing a hands-on and interactive learning experience, sandbox learning enhances retention and transfer of knowledge and skills to real-world situations.
- Like any skills, they take time and practice to acquire. Here at school, we intentionally use a mix of both path and sandbox learning to help you learn concepts, and also learn how to learn - an important skill for tech professionals of all kinds.
- We want this course to meet your needs, as much as we can. For us to be able to do that, we need - and very much want! - your feedback.
  - During the class, we want to know if we’re going too fast/slow, if you can’t hear, if you have questions, etc.
  - After the workshop, you’ll receive a survey, and we take your responses very seriously as we work to make the next class even better.
- Now, let’s get to know those tools a bit!

---

<!-- .element class="split-screen-with-title" -->

# Resources

<div>

<div>

- Your new friends!!! <!-- .element: class="fragment" data-fragment-index="1" -->
- Your instructor / TAs for questions <!-- .element: class="fragment" data-fragment-index="2" -->
- The internet for researching <!-- .element: class="fragment" data-fragment-index="3" -->
- AI tooling (Chatbot) for guidance <!-- .element: class="fragment" data-fragment-index="4" -->
- Slack for peer messaging <!-- .element: class="fragment" data-fragment-index="5" -->
- Zoom for collaborative screenshares <!-- .element: class="fragment" data-fragment-index="6" -->
- Canvas for tracking tasks <!-- .element: class="fragment" data-fragment-index="7" -->
- Your curiosity <!-- .element: class="fragment" data-fragment-index="8" -->

</div>

<div>

![Image](/ops-102-guide/curriculum/class-01/slides/assets/8_0.png)<!-- .element class="small" -->
![Image](/ops-102-guide/curriculum/class-01/slides/assets/8_1.png)<!-- .element class="small" -->

</div>

</div>

NOTE:
SAY:
- Sorting through technical challenges can feel like jumping hurdles sometimes. Don't feel alone if you feel the struggle, we're all in this together and we'll help you through it.
- You have a number of tools at your disposal today.
- One of the most important ones is your fellow students!
- We have TAs ready to answer you questions through the day and you can enter in questions on our Slack channel.
- Slack is where we chat and share files.
- We want this course to meet your needs, as much as we can.
- For us to be able to do that, we need - and very much want! - your feedback.
- During the class, we want to know if we're going too fast/slow, if you can't hear, if you have questions, etc.
- After the workshop, you'll receive a survey, and we take your responses very seriously as we work to make the next class even better.
- Now, let's get to know those tools a bit!

---

<!-- .element class="image-and-title" -->

# Online Classroom: Canvas

![Image](/ops-102-guide/curriculum/class-01/slides/assets/9_0.png)

NOTE:
SAY:
- Canvas is where you will find your future assignments, and submit your work in discussion with your classmates.
- You have been sent an invite to Canvas in your email inbox. Click the blue "Get Started" button.

DO:
- Navigate to the course in Canvas
- Go into Student View.
- Review the Syllabus tab and the course info.
  - The link to Zoom if they lose or forget it.
  - Explain how and where to watch the daily recordings.
- Review the Home page.
  - Explain how Modules work.
  - Explain due dates vs open/closed dates.
  - Explain due times.
    - How to set the Time Zone in Canvas:
      - Account > Settings > Edit Settings > In the Time Zone drop-down menu select a new time zone > Update Settings
  - Explain last day to resubmit assignments.
- How to look at grades tab.
  - Explain Due Column, Status Column and Score.
  - Explain how assignments are weighted by group.
  - Show grade percentages of groups at bottom of page.
- Review the Quizzes tab.
- Review the Calendar view.

---

<!-- .element class="main-title" -->
# Zoom

Use the tools to interact with the screen!

![Image](/ops-102-guide/curriculum/class-01/slides/assets/10_0.png)

NOTE:
SAY:
- We will meet in this same Zoom link for lecture every day in 102. You will get new Zoom links for 201, 301 and 401.
- These lectures are recorded for later review.
  - Due to the nature of our accelerated program, lecture moves very fast and a great way to take notes is to record the timestamps of important concepts during lecture  then go back and review the recordings at that particular timestamp in order to slow down or pause while you take your notes.
- We do expect you to have your cameras on during class.
  - You may turn your camera off if you have something going on that day but please message your instructor and let them know ahead of time.
- Please keep your mics off if you are not speaking.
- Feel free to use the Zoom chat to contribute to the dicussion or ask questions. This is a good way to keep side conversations from derailing the lecture.
  - Keep in mind that this chat goes away after lecture ends.
- This is meant to be interactive classroom experience, so at any time:
  - Speak up!
  - Use the “Raise-Hand” feature.
  - Use the Reactions feature.
  - Annotate
    - You can draw on my screen!
    - Bonus points for pointing out my errors!
- If you have any questions about Zoom etiquette, please see the guide linked in the Syllabus on Canvas.

DO:
- If you want to warm students up to drawing on the screen...
  - Let’s draw a robot together on the whiteboard!
  - Draw a robot body in the middle of the screen
  - Ask someone to draw a head on top of the screen.
  - Ask 3 more people to add arms.
  - Ask 4 more people to add legs or ways of getting around.
  - Ask everyone else to add any details they like.

---

<!-- .element class="main-title" -->
# Slack


NOTE:
SAY:
- This is the main means of communication, both during class, and in between courses.
- It’s a useful way of sharing links to learning resources, example websites to be used in class, sharing files, and code snippets.
- Slack has many tech-friendly features which is quickly making it an industry standard.
- It’ll be your main way of keeping in touch with me and each others.
- Did you know that you can DM yourself important info you don't want to ever lose?
- Please share important infomation in Slack as much as possible because the chat in Zoom goes away when class ends.


DO:
- Explain the class Slack channel and the on-campus channel.
  - Show pinned comments in the class Slack channel.
    - You can find the links to Zoom and Canvas here!
  - If you haven't already, type a short message introducing yourself in the class Slack channel.
- Show your favorite channel and explain how to find and join other channels.

---

<!-- .element class="main-title" -->

![Image](/ops-102-guide/curriculum/class-01/slides/assets/12_0.png)

NOTE:
- Learning actually goes more like this.
- Getting to the next level always requires the effort of engaging with the challenges you’ll surely face.
- Deciding to work hard is the crucial step. It all comes down to your MINDSET.
- [Sucking at something is the first step to being sorta good](https://fb.watch/hU80KTF_KQ/)

---

<!-- .element class="split-screen" -->

<div>

# What is Mindset?
- Mindset is self-perception or “self-theory” that people hold about themselves.<!-- .element: class="fragment" data-fragment-index="1" -->
- Fixed mindset is believing basic qualities, like intelligence or talent, are simply fixed traits. Believing that talent alone creates success—without effort.<!-- .element: class="fragment" data-fragment-index="2" -->
- Growth mindset is believing that people's most basic abilities can be developed through dedication and hard work—brains and talent are just the starting point.<!-- .element: class="fragment" data-fragment-index="3" -->

</div>

<div>

![Image](/ops-102-guide/curriculum/class-01/slides/assets/13_0.png)

</div>

NOTE:
SAY:
- What are we talking about when we say “Mindset”?
- People generally have a self perception that falls into one of two camps.
- But wait! Isn’t IQ fixed throughout someone’s life? There’s a simple test to measure IQ, afterall!
- How fixed do you think your IQ is? [thumb-scale]
- Have students in turn convert each verb words on the diagram into a full sentence, eg: “Someone with a fixed mindset will avoid challenges.”

---

<!-- .element class="title and text" -->

# Prepare Your Brain

“A few modern philosophers assert that an individual's intelligence is a fixed quantity, a quantity which cannot be increased. We must protest and react against this brutal pessimism… With practice, training, and above all, method, we manage to increase our attention, our memory, our judgement and literally to become more intelligent than we were before.”
### —ALFRED BINET <!-- .element: class="fragment" data-fragment-index="1" -->

Inventor of the IQ test<!-- .element: class="fragment" data-fragment-index="2" -->

![Image](/ops-102-guide/curriculum/class-01/slides/assets/14_0.png)<!-- .element: class="fragment" data-fragment-index="3" -->

NOTE:
SAY:
- Any idea who said this quote?
- Do you know what Alfred Binet is known for?
  - He was a French psychologist who invented the first practical IQ test, the Binet–Simon test.

---

<!-- .element class="image-and-title" -->
# Get into a Growth Mindset

![Developing a  Growth Mindset](/ops-102-guide/curriculum/class-01/slides/assets/developing-a-growth-mindset.png)

NOTE:
SAY:
- This exercise is adapted from [Mindful by Design](https://mindfulbydesign.com/change-mindset-change-words) and shows us how we can get into a growth mindset.
- As adult learners, you get to be your own teacher.
- I’m here as a facilitator, to create experiences where you can teach yourself what you want to learn.
- When we struggle, It’s tempting to turn to the negative self-talk of a fixed mindset. How can you get yourself back into a growth mindset?
- What is the Growth Mindset response to each of these?  [Answers from the class]
  - I'm not good at this. => No one is good at it when just beginning.
  - I give up. => Trying a new strategy will give you a way forward.
  - This is too hard. => It's meant to be hard. We grow by challenging ourselves.
  - I made a mistake. => That proves you've put in effort. What effort is helpful next?
  - I'll never be that smart. => Being smart is something you learn. You aren't done getting smarter.
  - My classmate can do it, but I can't. => There was a time they couldn't either. How'd they get to where they are now?
  - It's not easy...I can't figure it out...I don't know... => ...yet
- What questions can you ask yourself when you are feeling stuck? [Answers from the class]

---

<!-- .element class="main-title" -->
# Professional Ethics and Integrity

NOTE:
SAY:
- There is no grey area in cyber.

---

<!-- .element class="title-and-text" -->
# Ethics in Ops and Cybersecurity

- Ethics is a huge driver for employers and businesses.<!-- .element: class="fragment" data-fragment-index="1" -->
- Protect society, the common good, necessary public trust and confidence, and the infrastructure.<!-- .element: class="fragment" data-fragment-index="2" -->
- ISC2 Code of Ethics<!-- .element: class="fragment" data-fragment-index="3" -->
  - Act honorably, honestly, justly, responsibly, and legally<!-- .element: class="fragment" data-fragment-index="4" -->
  - Provide diligent and competent service to principals<!-- .element: class="fragment" data-fragment-index="5" -->
  - Advance and protect the profession<!-- .element: class="fragment" data-fragment-index="6" -->

NOTE:
SAY:
- Ethics is a huge driver for employers and businesses
  - Because we are entrusted with supporting and safeguarding computer systems containing sensitive company data and providing critical services for business operations, we are therefore beholden to a high standard of conduct, integrity, and ethics
- Protect society, the common good, necessary public trust and confidence, and the infrastructure
- [ISC2 Code of Ethics](https://www.isc2.org/Ethics#)
  - International Information System Security Certification Consortium
  - It is a set of principles and guidelines that govern the professional behavior and ethical responsibilities of information security professionals.
  - Act honorably, honestly, justly, responsibly, and legally
  - Provide diligent and competent service to principals
  - Advance and protect the profession

---

<!-- .element class="title-and-text" -->

# GitHub

- Why GitHub?<!-- .element: class="fragment" data-fragment-index="1" -->
  - Industry standard code storage & sharing solution<!-- .element: class="fragment" data-fragment-index="2" -->
  - Not just for full time developers<!-- .element: class="fragment" data-fragment-index="3" -->
- GitHub is an online platform to host code repositories (aka repos)<!-- .element: class="fragment" data-fragment-index="4" -->
- A Wiki is a section of a repo for hosting documentation<!-- .element: class="fragment" data-fragment-index="5" -->

![GitHub Logo](/ops-102-guide/curriculum/class-01/slides/assets/github-logo.png)

NOTE:
SAY:
- Throughout this program you’ll need to learn coding tooling and fundamental concepts.
  - Code is how we can talk to computers.
- Github is the web application that acts as a script repository.
  - Industry standard place to store and share scripts/code.
  - Many open source programs can be found on Github.
- Wikis are how we will organize and post our reading notes.

DO:
- **Take a break** and allow students to sign up for GitHub during the break so that they may follow along during the repo and Wiki demo.
- Demonstrate GitHub, repos and Wikis
    - This demo needs to move slow in order to allow students to complete each step as you do it.
    - When back from break, make sure every student has signed up for GitHub before moving forward.
  - Navigate to GitHub
  - Create a new repo named `ops-reading-notes`
    - Initialize with a `README.md`
  - Edit the `README.md` file to include a title and description that explains to the reader where to find the student's reading notes
    - You can acknowledge the h1 Markdown syntax but inform students that we will go over Markdown a little later.

    ```markdown
    # Hexx's Ops Reading Notes

    Welcome to my reading notes repo! You can find my notes under the Wiki tab!
    ```

  - Create a Wiki and name it `reading-01`
  - Remind students that there are references in the reading assignment that can help them set this up.

---


<!-- .element class="split-screen-with-title" -->
# Visual Studio Code

### An Integrated Development Environment (IDE)<!-- .element: class="fragment" data-fragment-index="1" -->

<div>

<div>

- The Swiss-Army-Knife of text editors!<!-- .element: class="fragment" data-fragment-index="2" -->
- Combines many features in one:<!-- .element: class="fragment" data-fragment-index="3" -->
  - Text editor<!-- .element: class="fragment" data-fragment-index="4" -->
  - File explorer<!-- .element: class="fragment" data-fragment-index="5" -->
  - Shell / Terminal<!-- .element: class="fragment" data-fragment-index="6" -->
  - Compiler / Interpreter<!-- .element: class="fragment" data-fragment-index="7" -->
  - Debugger<!-- .element: class="fragment" data-fragment-index="8" -->
- Extensions can add more features<!-- .element: class="fragment" data-fragment-index="9" -->
- also called "VS Code"<!-- .element: class="fragment" data-fragment-index="10" -->

</div>

<div>

![VS Code Logo](/ops-102-guide/curriculum/class-01/slides/assets/vs-code-logo.jpeg)<!-- .element: class="small" -->

</div>

</div>

NOTE:
SAY:
- An integrated development enviroment

DO:
  - Install VS Code on your personal computer
  - How 3 components are combined in an IDE:
    - Text editor
      - The text editor is the central component of an IDE where developers can write, edit, and manage their code files.
      - It provides features like syntax highlighting, code completion, indentation, and code formatting to enhance the developer's productivity.
      - The text editor allows programmers to create and modify code files in various programming languages.
    - File explorer
      - The file explorer component in an IDE enables developers to navigate and manage their project files and directories.
      - It provides a hierarchical view of the project structure, allowing users to create, rename, delete, and organize files and folders.
      - The file explorer helps developers easily locate and open the desired files within the IDE.
    - Terminal/command line
      - The terminal or command line interface within an IDE provides direct access to the operating system's command-line shell.
      - It allows developers to execute various commands and scripts within the development environment.
      - The terminal enables tasks such as compiling code, running tests, managing version control systems (e.g., Git), and performing other system operations without leaving the IDE.
      - It provides a command-line interface within the IDE's graphical user interface.
  - Compare to the using three programs separately
- Students will need to download VS Code on their personal computers.

---

<!-- .element class="title-and-text" -->
# Markdown

- Markdown is a simple syntax that formats text as headers, lists, boldface, and so on.<!-- .element: class="fragment" data-fragment-index="1" -->
  - “Syntax” is the set of rules that define the combinations of characters that are considered to be statements or expressions in that programming language.<!-- .element: class="fragment" data-fragment-index="2" -->
- The computer reads the Markdown syntax and interprets it as formatting instructions, changing how the text is presented on the screen.<!-- .element: class="fragment" data-fragment-index="3" -->
- Useful for documentation and notes.<!-- .element: class="fragment" data-fragment-index="4" -->
- Bookmark this <!-- .element: class="fragment" data-fragment-index="5" -->[Markdown Cheatsheet](https://www.markdownguide.org/cheat-sheet/)
- VS Code has a preview feature that renders Markdown.<!-- .element: class="fragment" data-fragment-index="6" -->

![Markdown Logo](/ops-102-guide/curriculum/class-01/slides/assets/markdown-logo.png)

NOTE:
SAY:
- We are going to learn your very first programming language today!
- Markdown is a simple syntax that formats text as headers, lists, boldface, and so on.
  - “Syntax” is the set of rules that define the combinations of characters that are considered to be statements or expressions in that programming language.
- The computer reads the Markdown syntax and interprets it as formatting instructions, changing how the text is presented on the screen.
- Useful for documentation and notes.
- Bookmark this [Markdown Cheatsheet](https://www.markdownguide.org/cheat-sheet/)
- VS Code has a preview feature that renders Markdown.

DO:
- Demo more Markdown syntax in VS Code using the Markdown Preview feature and the Markdown Cheatsheet.
  - Show students how they can copy/paste their code from VS Code into the GitHub GUI for now.
    - We will cover git flow in 201.
    - This is also a good opportunity to talk about Hot Keys briefly.
      - A hot key or keyboard shortcut is a key or a combination of keys on a keyboard that, when pressed at one time, performs a task like select all, copy and paste.
      - Windows/Linux:
        - select all: `Ctrl+A`
        - copy: `Ctrl+C`
        - paste: `Ctrl+V`
      - Mac:
        - select all: `Command+A`
        - copy: `Command+C`
        - paste: `Command+V`

---

<!-- .element class="main-title" -->
# What is a Computer?

NOTE:
SAY:
- First of all, let’s talk about what a computer really is. While we all use computer technology as part of our daily lives, we don’t always engage computing at all the various levels of abstraction.
- We are starting off at the lowest level: Hardware.
- We'll need to first start by understanding the components of your lab kit PC.

---

<!-- .element class="split-screen-with-title" -->
# Why Study Computer Components?

<div>

<div>

The Big Hack: How China Used a Tiny Chip to Infiltrate U.S. Companies <!-- .element: class="fragment" data-fragment-index="1" -->
  - Levels of computing <!-- .element: class="fragment" data-fragment-index="2" -->
  - Low level cyber threats <!-- .element: class="fragment" data-fragment-index="3" -->
  - Troubleshooting <!-- .element: class="fragment" data-fragment-index="4" -->
  - Provisioning <!-- .element: class="fragment" data-fragment-index="5" -->
  - Specs VS Performance <!-- .element: class="fragment" data-fragment-index="6" -->

</div>

<div>

![Image](/ops-102-guide/curriculum/class-01/slides/assets/17_0.png)

![Image](/ops-102-guide/curriculum/class-01/slides/assets/17_1.png)

</div>

</div>

NOTE:
SAY:
- So why might an aspiring cyber professional ever need to worry about computer hardware, when we have such matured services like AWS available, Google Cloud, and virtual machines?
- Let’s take a look at this security case study and find out!
  - Supply chain security - China’s spy chip on motherboards
  - Didn’t turn out to be a true acknowledged threat - Some controversy over this article
  - Sometimes security problems can manifest in hardware, at the lowest levels. In this case, we see a concern over an undocumented chip embedded in Chinese-manufactured motherboards.
  - This is called supply chain security. Organizations with matured security processes will have a screening process in place to evaluate new equipment and software for security concerns.
  - A cyber professional should be familiar with all layers of computing, even the lowest level of hardware, where threats like this can manifest.
- Additional reasons to know system internals and low level computing:
  - Troubleshooting and supporting
    - Physical
    - Software
  - Provisioning
    - Assembly / Set up a new system
    - OS installation / configuration
  - User needs - compare to building a gaming PC
    - Ability to recommend a computing solution
    - Ability to recommend hardware specifications
    - Ability to recommend an OS or software app

---

<!-- .element class="split-screen-with-title" -->

# Levels of Abstraction
### The amount of complexity by which a system is viewed or programmed.

<div>

<div>

- The higher the level, the less detail. <!-- .element: class="fragment" data-fragment-index="1" -->
  - The entire system, like the cloud. <!-- .element: class="fragment" data-fragment-index="2" -->
- The lower the level, the more detail. <!-- .element: class="fragment" data-fragment-index="3" -->
  - The components on the motherboard <!-- .element: class="fragment" data-fragment-index="4" -->
    - the integrated circuits <!-- .element: class="fragment" data-fragment-index="5" -->
    - transistors <!-- .element: class="fragment" data-fragment-index="6" -->
    - resistors <!-- .element: class="fragment" data-fragment-index="7" -->
    - capacitors <!-- .element: class="fragment" data-fragment-index="8" -->
    - other electronic components <!-- .element: class="fragment" data-fragment-index="9" -->

</div>

<div>

![Levels of Abstraction](/ops-102-guide/curriculum/class-01/slides/assets/levels-of-abstraction.png)<!-- .element  width="400" height="500" -->

</div>

</div>

NOTE:
SAY:
- Levels of abstraction refer to different layers or perspectives at which complex systems within IT infrastructure, networking, and cybersecurity, can be understood and operated.
- Each level of abstraction provides a specific view and deals with different aspects of the system, allowing for effective management, troubleshooting, and analysis.
- Each level of abstraction builds upon the lower levels, encapsulating and abstracting the complexities of the underlying layers.
- Understanding and working at different levels of abstraction allow IT professionals and cybersecurity practitioners to effectively manage and secure complex systems by focusing on the relevant aspects and applying appropriate solutions.
- It facilitates efficient communication and collaboration among IT professionals.

---

<!-- .element class="split-screen-with-title" -->
# Key Computer Components

<div>

<div>

  - Hardware refers to the tangible physical components of a computer system that can be touched and interacted with. <!-- .element: class="fragment" data-fragment-index="1" -->
  - The operating system (OS) acts as a control layer that manages and regulates the hardware, allowing users to interact with the computer through a user interface (UI) or graphical user interface (GUI). <!-- .element: class="fragment" data-fragment-index="2" -->
  - Applications or programs enable users to perform specific tasks or activities on a computer, providing specialized functionality and features. <!-- .element: class="fragment" data-fragment-index="3" -->

</div>

<div>

![Image](/ops-102-guide/curriculum/class-01/slides/assets/18_0.png)

</div>

</div>


NOTE:
SAY:
- Computing involves several crucial elements that work together to enable the functioning of a computer system.
- These components include hardware, the operating system (OS), and applications or programs.
- Let's delve into each of these components to gain a better understanding.
- The first component is hardware, which encompasses the physical components of a computer system.
  - Hardware refers to the tangible elements that you can touch and interact with, such as the CPU (Central Processing Unit), memory (RAM), storage devices, input/output devices like keyboards and mice, and the motherboard.
  - These hardware components collectively form the foundation of a computer system
- The second component is the operating system, commonly known as the OS.
  - The operating system acts as a control layer between the hardware and the user, managing and controlling the hardware resources.
  - It provides a user interface (UI) or graphical user interface (GUI) that allows users to interact with the computer system.
  - Examples of operating systems include Windows, macOS, Linux, and Android.
- The third component is applications or programs.
  - Applications are software that users utilize to perform specific tasks or activities on a computer system.
  - They provide specialized functionality and features tailored to different purposes, such as word processing, web browsing, photo editing, and gaming.
  - Examples of applications include Microsoft Word, Google Chrome, Adobe Photoshop, and video games.

---

<!-- .element class="title-and-text" -->
# Stages of Computing
### Computers operate through three fundamental stages that facilitate their functionality.

<div>

- Input <!-- .element: class="fragment" data-fragment-index="1" -->
  - Initiates an action by providing input to the computer, such as typing on the keyboard or clicking the mouse.
- Processing <!-- .element: class="fragment" data-fragment-index="2" -->
  - Once the input is received, the operating system instructs the hardware to process the input information.
- Output <!-- .element: class="fragment" data-fragment-index="3" -->
  - The output occurs when the computer presents the result of the task, making it visible to the user.

</div>

NOTE:
SAY:
- Understanding these stages is crucial in comprehending how computers function and how they respond to user actions.
- The first stage is the input stage, where we initiate an action by providing input to the computer.
  - This can involve various actions, such as typing on the keyboard, clicking the mouse, or using touch input on a touchscreen device.
  - During this stage, the computer receives the input and prepares to process it.
- In the processing stage, the operating system takes the input received and instructs the hardware to perform the requested task or process the provided information.
  - The processing stage involves the CPU executing the necessary instructions and utilizing other hardware resources to carry out the desired operation.
- The output is where the computer presents the result of the task or displays the processed information.
  - This output can be in various forms, such as text, images, videos, or any other media that the computer can render.
  - The output is typically displayed on the screen, making it visible to the user and allowing them to perceive the outcome of their actions.

---

<!-- .element class="split-screen-with-title" -->
# Circuits & Logic
### Circuit boards are essential components that manipulate electricity to transmit signals within a computer system.

<div>

<div>

- Circuits on the board serve as the building blocks for processing and transferring information. <!-- .element: class="fragment" data-fragment-index="1" -->
- These circuits change their value based on the input they receive, allowing for dynamic processing of electrical signals. <!-- .element: class="fragment" data-fragment-index="2" -->
- Logic gates, integrated within circuits, perform bitwise calculations and logical operations to process and manipulate the data. <!-- .element: class="fragment" data-fragment-index="3" -->

</div>

<div>

![Image](/ops-102-guide/curriculum/class-01/slides/assets/21_0.png)

</div>

</div>


NOTE:
SAY:
- Circuit boards are critical components that enable the flow and processing of electrical signals within a computer.
- They play a vital role in managing and manipulating electrical signals within a computer system.
  - These boards consist of numerous electronic components, including circuits, which are responsible for processing and transmitting data.
- Circuits are the building blocks of circuit boards, and they form the foundation for signal processing.
  - One key characteristic of circuits is their ability to change their value based on the input they receive.
  - This dynamic value change allows for flexible processing of electrical signals within the computer system.
- To perform complex operations on data, circuits utilize logic gates embedded within them.
  - Logic gates are electronic devices that perform bitwise calculations and logical operations on the input signals.
    - Bitwise calculations are typically applied to binary numbers, where each bit represents a specific value (0 or 1).
    - These calculations act on corresponding bits of two binary numbers and produce a result based on predefined rules.
  - They manipulate binary data by applying operations such as `AND`, `OR`, `NOT` and `XOR`.
  - These operations enable circuits to process and manipulate the data as required by the computer system.

---

<!-- .element class="title-and-text" -->
# Binary & Data

<div>

- The earliest computers were designed as calculators, performing mathematical calculations. <!-- .element: class="fragment" data-fragment-index="1" -->
  - Binary, a base-2 number system, was devised to enable efficient mathematical operations in computers. <!-- .element class="medium-text" -->
  - Binary representation aligns with the on-off states of electronic signals used in computers. <!-- .element class="medium-text" -->
- Binary Basics <!-- .element: class="fragment" data-fragment-index="2" -->
  - Our number system is typically base 10 (decimal), using digits 0-9. <!-- .element class="medium-text" -->
  - Computers use binary, a base-2 number system. <!-- .element class="medium-text" -->
  - Binary consists of only two digits: 0 and 1, with significant importance in computing. <!-- .element class="medium-text" -->
  - Binary digits, or bits, are the building blocks of binary representation. <!-- .element class="medium-text" -->
- Bits and Bytes <!-- .element: class="fragment" data-fragment-index="3" -->
  - The smallest unit of data in binary is a bit (binary digit). <!-- .element class="medium-text" -->
  - A bit represents two states: 0 or 1, serving as the fundamental unit of data storage and transmission. <!-- .element class="medium-text" -->
  - Bits are grouped into bytes, consisting of 8 bits. <!-- .element class="medium-text" -->
  - A byte allows computers to work with larger units of data and provides a range of 0-255 (2^8) possible combinations. <!-- .element class="medium-text" -->

</div>

NOTE:
SAY:
- The earliest computers were initially designed as calculators, performing mathematical calculations.
  - To enable computers to effectively carry out mathematical operations, binary, a base-2 number system, was devised as a means of communication.
  - By utilizing binary, computers can represent and process information in a way that corresponds to the on-off states of electronic signals.
- Binary Basics
  - Our number system is typically base 10, known as the decimal system, where we use digits from 0 to 9 to represent numbers.
  - However, in computers, we use a different number system called binary, which is base 2.
  - Binary uses only two digits: 0 and 1. It may seem simple, but it has incredible significance in computing.
  - Binary digits, or bits, are the building blocks of binary representation in computers.
- Bits and Bytes
  - In binary, the smallest unit of data is called a bit, short for binary digit.
  - A bit can represent two states: 0 or 1. This is the fundamental unit for storing and transmitting data within a computer system.
  - To handle larger units of data, bits are grouped together into bytes.
  - A byte consists of 8 bits.
    - It represents a larger unit of data and allows computers to work with a broader range of information.
    - Bytes can store values from 0 to 255 (2^8) as they provide 256 possible combinations of 0s and 1s.

---

<!-- .element class="title-and-text" -->
# Binary & Data

<div>

- Binary to Bits Conversion <!-- .element: class="fragment" data-fragment-index="1" -->
  - Converting binary to bits involves breaking down the binary number digit by digit. <!-- .element class="medium-text" -->
  - Example: Converting binary number 10110110 into bits. <!-- .element class="medium-text" -->
  - Each digit represents a bit (1 or 0). <!-- .element class="medium-text" -->
  - The given binary number has 8 digits, which means it consists of 8 bits. <!-- .element class="medium-text" -->
  - This binary number is equivalent to 1 byte (8 bits). <!-- .element class="medium-text" -->
- Binary Calculator <!-- .element: class="fragment" data-fragment-index="2" -->
  - To double-check your work, you can use a Binary Calculator as a helpful tool. <!-- .element class="medium-text" -->

</div>

NOTE:
SAY:
- Binary to Bits Conversion
  - To convert a binary number into bits, we break it down digit by digit.
  - Let's convert the binary number `10110110` into bits.
  - Starting from the leftmost side, we have: 1, 0, 1, 1, 0, 1, 1, and 0.
  - Each digit represents a bit.
    - First digit: 1 represents a bit.
    - Second digit: 0 represents a bit.
    - Third digit: 1 represents a bit.
    - Fourth digit: 1 represents a bit.
    - Fifth digit: 0 represents a bit.
    - Sixth digit: 1 represents a bit.
    - Seventh digit: 1 represents a bit.
    - Eighth digit: 0 represents a bit.
  - How many bits make up this binary number?
    - Each digit in a binary number represents a bit, and since there are 8 digits in the given binary number, it means that there are 8 corresponding bits.
  - How many bytes make up this binary number?
    - Since 1 byte is equal to 8 bits, this binary number is equivalent to 1 byte.
- If you need to cheat, use Binary Calculator to check your work.

---

<!-- .element class="split-screen-with-title" -->
# Inside of a Computer

<div>

<div>

Find these components on your lab PC:
- Motherboard <!-- .element: class="fragment" data-fragment-index="1" -->
- CPU <!-- .element: class="fragment" data-fragment-index="2" -->
- RAM <!-- .element: class="fragment" data-fragment-index="3" -->
- PCI/PCIe Slots <!-- .element: class="fragment" data-fragment-index="4" -->
- Power Interfaces <!-- .element: class="fragment" data-fragment-index="5" -->
- I/O Shield <!-- .element: class="fragment" data-fragment-index="6" -->
- Hard Drive/SSD <!-- .element: class="fragment" data-fragment-index="7" -->
- Chassis Fan <!-- .element: class="fragment" data-fragment-index="8" -->
- CD/DVD-ROM Drive <!-- .element: class="fragment" data-fragment-index="9" -->

</div>

<div>

![Image](/ops-102-guide/curriculum/class-01/slides/assets/26_0.png)

</div>

</div>

NOTE:
SAY:
- Motherboard
  - The motherboard is the main circuit board of a computer system.
  - It provides a platform for connecting and integrating various hardware components, such as the CPU, RAM, graphics card, storage devices, and other peripherals.
  - The motherboard contains slots, connectors, and circuits that allow these components to communicate and work together.
  - Motherboards come in many sizes. Here are some of the common form factors you’ll see in desktop computers.

- CPU socket and the CPU
  - The CPU socket is the physical connector on the motherboard that holds the CPU (Central Processing Unit).
  - The CPU is responsible for processing information and performing calculations.
  - It generates heat during operation and is usually paired with a cooling solution, such as a CPU fan or heatsink, to dissipate the heat.
  - Clock speed is the speed at which CPU executes instructions and is measured in MHz or GHz.
  - The chipset of a motherboard allows the CPU to communicate with other devices.

- RAM
  - These are slots on the motherboard where RAM (Random Access Memory) sticks are inserted.
  - RAM is a type of volatile memory that provides temporary storage for data that the CPU needs to access quickly.
    - Volatile memory is a type of computer memory that loses its stored data when the power to the machine is turned off.
    - RAM provides fast access to data while the computer is running, but the data is erased when the computer is shut down.
    - Non-volatile memory, such as hard drives, is used for long-term data storage.
  - The RAM slots allow for easy installation and expansion of memory capacity.

- PCI slots
  - Peripheral Component Interconnect slots
  - They are expansion slots found on the motherboard and are used to connect various expansion cards, such as sound cards, network cards, or other peripherals, to the motherboard.
  - PCI slots are an older standard, with slower data transfer rates compared to newer standards like PCI-Express (PCIe).

- PCIe slots
  - Peripheral Component Interconnect Express
  - PCI-Express slots are also expansion slots on the motherboard, but they offer faster data transfer rates compared to PCI slots.
  - PCIe is commonly used for connecting high-performance components like graphics cards, network cards, and solid-state drives.
    - It provides a fast and dedicated connection for graphics-intensive tasks.
  - Different versions of PCIe, such as PCIe x1, x4, x8, and x16, provide varying bandwidths for different needs.

- Power interfaces
  - The power interface on a computer typically consists of multiple connectors or ports that allow for the transfer of power from the power supply unit (PSU) to various components within the system.
  - The specific appearance and arrangement of power interfaces can vary depending on the computer and its components
  - The motherboard itself requires power to operate, and the power interfaces ensure it receives the necessary supply.
  - Additionally, components like fans, GPUs, and hard drives also need power connections to function properly.

- I/O shield
  - Input/Output Shield
  - The I/O shield is a metal plate located at the back of the computer case, aligned with the motherboard's rear I/O ports.
  - It provides a protective cover and serves as a barrier between the motherboard and the external connectors, such as USB ports, HDMI ports, audio jacks, Ethernet ports, etc.
  - These ports allow for the connection of peripherals and external devices to the computer, like a mouse or keyboard.

- Hard Drive/SSD
  - A hard drive or solid-state drive (SSD) is a storage device used in computers to store and retrieve data.
  - It provides long-term storage for operating systems, software applications, files, and other data.
  - Hard drives utilize magnetic storage technology, while SSDs use flash memory technology.
  - They are connected to the computer's motherboard and store data on spinning disks (hard drives) or flash memory chips (SSDs).
  - The capacity of a hard drive or SSD is measured in gigabytes (GB) or terabytes (TB).

- Chassis Fan
  - A chassis fan is a cooling component in a computer's chassis or case.
  - Its primary function is to circulate air inside the case to dissipate heat generated by the computer's components.
  - The chassis fan helps maintain optimal operating temperatures and prevents overheating, which can affect the performance and lifespan of the computer.
  - Chassis fans come in different sizes and can be mounted on various locations within the case, such as the front, rear, or side panels.
  - They are typically connected to the motherboard and can be controlled either manually or automatically based on temperature sensors.

- CD/DVD-ROM Drive
  - A CD/DVD-ROM drive is an optical disc drive used to read CDs (Compact Discs) and DVDs (Digital Versatile Discs).
  - It allows users to access and retrieve data stored on optical discs, such as software installation media, music CDs, or movies.
  - CD/DVD-ROM drives use laser technology to read the information encoded on the disc's surface.
  - In addition to reading, some CD/DVD-ROM drives have the capability to write data onto blank recordable CDs or DVDs.
  - However, with the rise of digital distribution and cloud storage, CD/DVD-ROM drives have become less common in modern computers.

---

<!-- .element class="main-title" -->
# Demo and Lab

NOTE:
DO:
- Switch to your overhead webcam. Open up your lab PC. Show students were all these parts are.
  - I/O shield
  - PCI slots on motherboard
  - PCI-Express slots on motherboard
  - Processor or Central Processing Unit (CPU) w/ CPU fan - DO NOT Extract
    - **TELL STUDENTS: “DO NOT EXTRACT”**
  - Motherboard
  - Random Access Memory (RAM) - EXTRACT
  - Hard drive - EXTRACT
  - Chassis Fan - EXTRACT
  - DVD-ROM Drive - EXTRACT
  - Power supply
  - Case

- Review lab tasks in Canvas.
- Review lab submission instructions.
  - Copy/paste the lab text into Google Doc.
    - Students will be expected to record their lab experiences within the lab text.
  - Demonstrate how to setup a Google Doc with "Commenter Access"
      - Naming convention matters
        - ex: `ops-102d6: Lab 01`
      - Click "Share" in top right corner
      - Select "Anyone with a link"
      - Select "Commenter"
      - Click "Copy link", then "Done"
        - This is the link the students will submit in Canvas
- Remind students to complete the reading assignment for next class before the upcoming lecture.
- Remind students to leave their lab machine disassembled until next class.

PYDUKE — FULL FUNCTIONAL APPLICATION BUILD

I am giving you an existing PyDuke ZIP/repository.

IMPORTANT:

The existing project is primarily a FRONTEND/UI prototype.

Many features visually exist, but their underlying functionality does NOT exist.

DO NOT assume that the existing buttons, games, lessons, progress system, AI tutor, code editor, or navigation are already implemented.

DO NOT merely repair the UI.

Your job is to transform this existing frontend prototype into a REAL, FUNCTIONAL Python-learning web application.

Preserve the existing PyDuke visual design where useful, but build the actual application logic underneath it.

============================================================

1. FIRST — AUDIT THE EXISTING PROJECT

============================================================

Before changing anything, inspect the repository.

Identify:

- framework
- frontend structure
- routes
- components
- pages
- data files
- lesson files
- game files
- state management
- storage
- API routes
- backend
- server
- Gemini integration
- package.json
- environment configuration

Determine which features are:

A. genuinely functional

B. partially functional

C. frontend-only/mock

Do not assume something is functional merely because a UI component exists.

After auditing, build whatever is missing.

============================================================

2. FUNDAMENTAL REQUIREMENT

============================================================

PyDuke must become a REAL application.

The final application must allow a student to:

- learn Python
- read lessons
- practice Python
- run Python code
- solve exercises
- play programming games
- practice Python typing
- earn XP
- track progress
- earn achievements
- revise previous topics
- chat with an AI Python tutor
- use a live AI tutor where supported
- save progress

The website must not be a collection of static screens.

============================================================

3. DO NOT JUST MAKE THE FRONTEND LOOK FUNCTIONAL

============================================================

This is the most important instruction.

DO NOT solve problems by adding:

- fake buttons
- fake scores
- fake XP
- fake game results
- fake lesson completion
- fake AI messages
- static "Correct!" responses
- static game screens
- decorative timers
- decorative progress bars
- fake code execution

Every feature must have real underlying logic.

============================================================

4. BUILD A REAL APPLICATION ARCHITECTURE

============================================================

If the current project has no meaningful backend, create the necessary backend/API layer.

Use a clean architecture such as:

Frontend
↓
Application state
↓
API/backend
↓
Services
↓
Database/storage
↓
External APIs

For the personal/student version, do NOT add unnecessary authentication.

The user explicitly wants a FREE website with no locked content.

============================================================

5. NO AUTHENTICATION REQUIRED

============================================================

Do not create:

- login requirement
- subscription system
- premium account
- payment system

The student should be able to open and use PyDuke immediately.

A local student profile can be created without authentication.

============================================================

6. EVERY LESSON MUST BE ACCESSIBLE

============================================================

REMOVE ALL LOCKING.

Every lesson must be accessible immediately.

No:

- locked lessons
- prerequisites
- required XP
- required level
- premium lessons
- subscription restrictions

The recommended learning order can still be displayed.

Example:

"Recommended after learning loops"

But the student must still be able to open it.

============================================================

7. BUILD A REAL LESSON ENGINE

============================================================

Create a proper lesson data structure.

Each lesson should contain:

- ID
- title
- description
- difficulty
- estimated time
- objectives
- explanation
- definitions
- syntax
- examples
- output
- line-by-line explanations
- common mistakes
- practice
- coding exercise
- hints
- solution explanation
- review

The lesson page must dynamically load the selected lesson.

For example:

/learn/variables

loads Variables.

/learn/conditions

loads Conditions.

/learn/loops

loads Loops.

/learn/lists

loads Lists.

Do not send every lesson URL back to the lesson list.

============================================================

8. LESSON CONTENT

============================================================

Build substantial real Python lessons.

At minimum cover:

1. Introduction to Python
2. print()
3. Comments
4. Variables
5. Data types
6. Strings
7. Input
8. Type conversion
9. Operators
10. Conditions
11. for loops
12. while loops
13. range()
14. Lists
15. Tuples
16. Dictionaries
17. Sets
18. Functions
19. Parameters
20. Return
21. Scope
22. String methods
23. List methods
24. Error handling
25. Files
26. Modules
27. JSON
28. Practical Python
29. Projects

Make the curriculum expandable.

============================================================

9. REAL PYTHON CODE EXECUTION

============================================================

The existing frontend may contain a code editor, but that does NOT mean Python execution exists.

Implement real Python execution.

Use a suitable browser Python runtime such as Pyodide where appropriate.

The student must be able to:

- type Python
- run Python
- see stdout
- see errors
- reset
- save code
- submit exercises

Example:

Student enters:

print("Hello")

Presses Run.

The application actually executes Python and displays:

Hello

If the student enters invalid Python, display the actual error.

Do NOT fake execution with predefined responses.

============================================================

10. SAFE CODE EXECUTION

============================================================

User Python code must run in an isolated/safe environment.

Do not execute arbitrary student code directly on the server without proper isolation.

Prefer client-side/browser execution where practical.

Prevent code from accessing sensitive application/server resources.

============================================================

11. REAL EXERCISE ENGINE

============================================================

Create an exercise engine.

Each coding exercise should contain:

- instructions
- starter code
- expected behavior
- test cases
- hints
- difficulty
- XP reward

When the student presses Submit:

Actually evaluate the code against the exercise requirements.

Correct solution:

→ success

Incorrect solution:

→ useful feedback

Do NOT mark the exercise correct simply because Run succeeded.

============================================================

12. BUILD REAL GAMES

============================================================

The current game list is only a UI concept.

Turn every game into an actual playable game.

Games:

1. Code Fixer
2. Predict the Output
3. Code Ordering
4. Debugging Challenge
5. Build It
6. Typing Sprint
7. Boss Battle

Each must have:

- game state
- instructions
- gameplay
- scoring
- feedback
- difficulty
- completion
- restart
- XP
- result screen

============================================================

13. CODE FIXER

============================================================

Generate/select broken Python programs.

The student edits the code.

Run the program.

The game determines whether the problem was fixed.

Examples of bugs:

- IndexError
- NameError
- TypeError
- SyntaxError
- indentation problems
- incorrect conditions
- incorrect loops
- incorrect function behavior

Include multiple challenges.

Do not show the same static challenge forever.

============================================================

14. PREDICT OUTPUT

============================================================

Give real Python code.

Ask:

"What will this output?"

Student answers.

Actually compare their answer with the expected output.

Then explain why.

Track:

- score
- accuracy
- streak
- XP

============================================================

15. CODE ORDERING

============================================================

Give code lines in the wrong order.

Allow drag-and-drop/reordering.

Check whether the resulting order is correct.

Include:

- variables
- conditions
- loops
- functions
- increasingly complex examples

============================================================

16. DEBUGGING CHALLENGE

============================================================

Give a real broken program.

Student must:

- inspect
- edit
- run
- fix

Track the number of attempts.

Explain the bug after completion.

============================================================

17. BUILD IT

============================================================

Give a programming objective.

Example:

"Create a program that asks the user for two numbers and prints their sum."

Provide:

- instructions
- starter code
- editor
- Run
- Submit
- tests
- hints

Actually test the submitted program.

============================================================

18. TYPING SPRINT

============================================================

Build a REAL typing engine.

Capture keyboard input.

Calculate:

- WPM
- CPM
- accuracy
- errors
- correct characters
- incorrect characters
- elapsed time
- best score

Use Python code as typing material.

Examples:

print("Hello World")

for i in range(10):
print(i)

Train Python symbols:

()
[]
{}
:

+ 

- 

* 

/
_

«»

<
"

The timer must actually measure time.

============================================================

19. BOSS BATTLE

============================================================

Create a real multi-stage challenge.

Combine:

- Python concepts
- multiple choice
- output prediction
- debugging
- code ordering
- coding

Track:

- lives
- score
- progress
- XP

Actually determine whether answers are correct.

============================================================

20. REAL PROGRESS SYSTEM

============================================================

Build a central progress system.

Track:

- lessons viewed
- lessons completed
- exercises completed
- game attempts
- game scores
- XP
- level
- streak
- achievements
- typing records
- mistakes
- revision topics

Do not hard-code dashboard numbers.

If a student earns 100 XP, dashboard XP must actually become 100.

============================================================

21. PERSISTENCE

============================================================

This is a personal student website.

No authentication is required.

Persist student data using:

IndexedDB

or localStorage for simple data.

Prefer IndexedDB if the amount of data becomes significant.

Create a clean storage service.

For example:

progressService
lessonService
gameService
typingService
achievementService

After refreshing the browser:

progress must remain.

============================================================

22. PROFILE

============================================================

Allow the student to create a local profile.

Store:

- name
- XP
- level
- streak
- completed lessons
- game records
- achievements
- typing records

No account/login is required.

============================================================

23. ACHIEVEMENTS

============================================================

Implement actual achievements.

Examples:

First Lesson
Complete one lesson.

Bug Hunter
Fix 10 bugs.

Python Typist
Complete 5 typing sessions.

Code Runner
Complete 10 coding exercises.

Game Master
Complete all game types.

Achievements must unlock based on real events.

============================================================

24. REVISION SYSTEM

============================================================

Implement actual revision.

Track questions/exercises the student gets wrong.

Use those concepts in future revision.

Example:

Student repeatedly struggles with:

list indexing

The revision system should bring list-indexing exercises back.

============================================================

25. DAILY PRACTICE

============================================================

Create actual daily practice.

Generate/select:

- concept questions
- output questions
- debugging
- coding
- typing

Use the student's progress to determine suitable content.

Do not simply display "Daily Practice" as a card.

============================================================

26. GEMINI AI TUTOR

============================================================

There is a Gemini API key available.

Build a REAL Gemini AI Python tutor.

IMPORTANT:

The AI must NOT be restricted to topics the student has already learned.

REMOVE instructions such as:

"Do not answer questions the learner has not learned."

That behavior is NOT wanted.

The student can ask ANY Python question.

Examples:

"What are classes?"

"Explain recursion."

"What is a decorator?"

"How does async work?"

"Explain generators."

"How does Python memory management work?"

The AI should answer appropriately.

============================================================

27. AI TEACHING BEHAVIOR

============================================================

The AI should teach rather than merely output answers.

For beginner questions:

Definition

→ simple explanation

→ example

→ code

→ output

→ common mistake

For exercise assistance:

Hint

→ stronger hint

→ explanation

→ solution if requested.

But this must NOT prevent general Python questions.

============================================================

28. GEMINI API SECURITY

============================================================

NEVER expose the permanent Gemini API key in frontend code.

Never place it in:

- React source
- public folder
- localStorage
- GitHub source
- client-side public environment variables

Use:

GEMINI_API_KEY

on the server.

Frontend:

POST /api/ai/chat

Backend:

Gemini API

Return response to frontend.

============================================================

29. GEMINI CONTEXT

============================================================

When appropriate, send Gemini:

- current lesson
- current exercise
- submitted code
- error
- student question

But do NOT restrict the AI to the current lesson.

Example:

Current lesson:

Lists

Student:

"What are Python classes?"

The AI should answer.

============================================================

30. CHAT INTERFACE

============================================================

Build a real chat.

Features:

- message history
- input
- send
- loading
- errors
- clear chat
- code formatting
- copy code
- suggested questions

Suggested prompts:

Explain this
Why is this code wrong?
Give me a hint
Show me an example
Teach me this
Give me a practice problem
Make it harder

============================================================

31. LIVE AI TUTOR

============================================================

Build a REAL Live Tutor using the current Gemini Live/realtime API where supported.

It should allow:

- Start Live Tutor
- microphone
- spoken student question
- spoken AI response
- End Session

Do NOT create a fake live interface.

If Gemini's current Live API requires a secure session/token architecture:

Keep the permanent Gemini API key server-side.

Use the appropriate browser-safe session mechanism.

Handle:

- microphone permission
- network failure
- API errors
- session termination
- reconnect if appropriate

If Live requires a specific API/model configuration that cannot be completed from the current environment, implement the correct architecture and document exactly what configuration remains.

Do NOT pretend it is working if it isn't.

============================================================

32. ROUTING

============================================================

Create real routes.

For example:

/
/learn
/learn/:lessonId
/games
/games/:gameId
/code
/typing
/tutor
/live-tutor
/profile
/progress

Critical requirement:

/games

must show the game list.

/games/code-fixer

must show Code Fixer.

/games/typing-sprint

must show Typing Sprint.

/learn

must show lesson list.

/learn/lists

must show Lists lesson.

Refreshing a detail URL must keep the detail page.

Browser Back must work correctly.

============================================================

33. MOBILE NAVIGATION

============================================================

Existing bottom navigation:

Home
Learn
Code
Games
More

Make every item functional.

Do not let child routes accidentally render the parent list.

Test on a mobile-sized viewport.

============================================================

34. FREE WEBSITE

============================================================

Everything is free.

Remove:

- locks
- premium labels
- subscription barriers
- XP gates
- level gates
- prerequisite gates

The learner's progress is for tracking and personalization, not access control.

============================================================

35. SEARCH

============================================================

Implement real lesson search.

Searching:

"loop"

should find relevant lessons.

Clicking a result must open that actual lesson.

============================================================

36. ERROR HANDLING

============================================================

Build real error handling.

If Gemini fails:

show an understandable error.

If code execution fails:

show the Python error.

If storage fails:

handle gracefully.

If microphone permission is denied:

tell the user what happened.

Never leave blank screens.

============================================================

37. NO FAKE DATA

============================================================

Search the entire repository for:

TODO
Coming Soon
Placeholder
Mock
Fake
Demo
Sample response
Static response
Not implemented

Replace visible fake functionality with real functionality.

If something cannot be implemented, clearly document it instead of pretending.

============================================================

38. DO NOT REWRITE THE WHOLE DESIGN UNNECESSARILY

============================================================

The existing PyDuke design is useful.

Keep:

- branding
- visual identity
- layout ideas
- useful components
- icons
- responsive styling

But functionality has priority.

If the frontend component exists but is only visual, connect it to real application logic.

============================================================

39. TESTING

============================================================

Actually test the application.

TEST LESSONS:

Open every lesson.

Confirm every lesson contains actual content.

Confirm every lesson opens correctly.

Confirm Previous/Next.

Confirm practice.

Confirm completion.

TEST GAMES:

Open every game.

Actually play every game.

Confirm scoring.

Confirm game completion.

Confirm restart.

TEST CODE:

Run valid Python.

Run invalid Python.

Submit correct solution.

Submit incorrect solution.

TEST TYPING:

Type.

Make mistakes.

Confirm WPM changes.

Confirm accuracy changes.

Confirm timer.

TEST PROGRESS:

Complete lesson.

Earn XP.

Refresh.

Confirm XP remains.

TEST AI:

Ask a basic Python question.

Ask an advanced Python question.

Ask about a topic not in the current lesson.

Confirm Gemini actually responds.

TEST LIVE:

Start session.

Test microphone.

Speak.

Confirm response if the configured Gemini Live service supports it.

============================================================

40. ACCEPTANCE CRITERIA

============================================================

Do NOT call the project complete until these are true:

[ ] PyDuke is no longer merely a frontend mockup.

[ ] Lessons contain real educational content.

[ ] Every lesson opens.

[ ] Every lesson is unlocked.

[ ] Lesson exercises work.

[ ] Python code can actually execute.

[ ] Coding submissions are actually tested.

[ ] Games actually work.

[ ] Code Fixer works.

[ ] Predict Output works.

[ ] Code Ordering works.

[ ] Debugging Challenge works.

[ ] Build It works.

[ ] Typing Sprint works.

[ ] Boss Battle works.

[ ] Scores are real.

[ ] XP is real.

[ ] Progress is persistent.

[ ] Achievements are real.

[ ] Revision works.

[ ] Gemini Tutor actually communicates with Gemini.

[ ] AI can answer ANY Python topic.

[ ] AI is not restricted to completed lessons.

[ ] Gemini API key is protected.

[ ] Live Tutor is genuinely implemented where supported.

[ ] No lesson is locked.

[ ] No premium restrictions exist.

[ ] Mobile navigation works.

[ ] Browser Back works.

[ ] Direct URLs work.

[ ] Refreshing a lesson/game does not return to its list.

============================================================

41. IMPORTANT FINAL INSTRUCTION

============================================================

Do NOT simply tell me:

"Here is what you should build."

You are the coding agent.

BUILD IT.

Modify the existing repository.

Create missing backend/API functionality.

Create missing services.

Create missing game engines.

Create missing lesson engines.

Create missing storage.

Connect Gemini.

Implement the AI Tutor.

Implement Live Tutor where supported.

Test the application.

Fix errors.

Then provide:

1. Files changed.
2. Architecture created.
3. Dependencies added.
4. Environment variables required.
5. Commands to run locally.
6. Commands/configuration required for deployment.
7. Gemini setup instructions.
8. Live Tutor setup instructions.
9. Any genuine limitation that remains.

Do not report a feature as "working" unless you actually tested its underlying behavior.

FINAL PRODUCT:

PyDuke must be a genuinely usable FREE Python-learning platform, not a frontend demonstration.

The student should be able to open the website and immediately:

LEARN → PRACTICE → CODE → PLAY → TYPE → GET AI HELP → TRACK PROGRESS.

Everything must actually work.

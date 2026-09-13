You are an expert full-stack web developer.

I want you to BUILD and COMPLETE a fully functional online Maths Mock Test website directly inside my existing GitHub repository:

https://github.com/polaieducationhub/MOCK-TEST-20

IMPORTANT:
START WORKING DIRECTLY.
Do not only explain what to do.
Do not give me a tutorial first.
Inspect the existing repository, create/update the required files, and build the working website.

PROJECT:
POLAI EDUCATION HUB
Odisha Police Constable Maths Mock Test-20

SOURCE:
Use the attached PDF in this conversation:
“Maths_Practice_Set_40x22.5in.pdf”

The PDF contains the complete 21-question bilingual mock test and its answer key.

DO NOT SHOW THE QUESTIONS IN THIS PROMPT.
Instead, extract/use the questions directly from the attached PDF while building the application.

==================================================
1. CORE REQUIREMENT
==================================================

Create a professional online competitive-exam mock-test website similar in usability to Testbook-style mock tests, but with an ORIGINAL Polai Education Hub design.

The website must contain EXACTLY 21 questions from the PDF.

Language:
English + Odia

Exam:
Odisha Police Constable Maths Mock Test-20

Questions:
21

Total Marks:
21

Correct:
+1 mark

Wrong:
-1/3 mark

Unattempted:
0 mark

Time:
15 minutes

Maximum Score:
21

==================================================
2. WEBSITE MUST ACTUALLY WORK
==================================================

Do NOT create a static demo.

Implement real JavaScript functionality:

- Start Test
- 15-minute countdown
- Question navigation
- Option selection
- Previous
- Next
- Mark for Review
- Clear Answer
- Question palette
- Progress tracking
- Auto-submit when timer reaches 00:00
- Manual Submit Test
- Score calculation
- Negative marking
- Result page
- Question-wise review
- Retake Test

All functionality must work without a backend.

Use localStorage if necessary so accidental page refresh does not immediately destroy the current test state.

==================================================
3. DESIGN
==================================================

Create a PREMIUM competitive-exam interface.

Design inspiration:
- Testbook
- modern online examination portals
- professional education platforms

BUT:
Do not copy Testbook branding, logo, proprietary assets, or exact UI.

Create an ORIGINAL:
“Polai Education Hub” identity.

Use:
- modern blue-based professional theme
- white cards
- subtle gradients
- rounded corners
- soft shadows
- clean typography
- attractive buttons
- smooth transitions
- excellent spacing
- responsive layout

The interface should look especially good on:
- Android mobile
- desktop
- tablet

==================================================
4. START PAGE
==================================================

Create a beautiful landing/start page.

Show:

POLAI EDUCATION HUB

ODISHA POLICE CONSTABLE

MATHS MOCK TEST-20

21 Important Questions

English + Odia

Exam Information:

Total Questions: 21
Total Marks: 21
Time: 15 Minutes
Correct Answer: +1
Wrong Answer: -1/3
Unattempted: 0

Add an attractive:

“START TEST”

button.

Before starting, show a short instruction card:

• Read every question carefully.
• Each correct answer gives +1 mark.
• Each wrong answer deducts 1/3 mark.
• Unattempted questions receive 0 mark.
• Test duration is 15 minutes.
• Test will automatically submit when time ends.

==================================================
5. QUESTION DATA
==================================================

Extract ALL 21 questions from the attached PDF.

IMPORTANT:

- Do not invent questions.
- Do not modify question meaning.
- Do not add extra questions.
- Do not remove questions.
- Preserve English exactly.
- Preserve Odia exactly as supplied in the PDF.
- Preserve options A, B, C, D.
- Preserve mathematical notation as accurately as possible.
- Use the answer key from the final PDF page.

Create a clean JavaScript question-data structure such as:

const questions = [
  {
    id: 1,
    english: "...",
    odia: "...",
    options: {
      A: "...",
      B: "...",
      C: "...",
      D: "..."
    },
    answer: "A"
  }
];

Continue until question 21.

Do not display the answer key to students during the test.

==================================================
6. EXAM SCREEN
==================================================

After clicking START TEST, open the examination interface.

TOP HEADER:

POLAI EDUCATION HUB

ODISHA POLICE CONSTABLE
MATHS MOCK TEST-20

Right side:

TIME LEFT
15:00

Timer must start immediately.

==================================================
7. TIMER
==================================================

Implement a real countdown:

15:00
14:59
14:58
...

At:
00:00

automatically submit the test.

Before automatic submission show no extra interaction.

Near the final minutes, visually highlight the timer.

Do not make the timer excessively distracting.

==================================================
8. QUESTION DISPLAY
==================================================

Show:

Question 1 of 21

Then:

English Question

Odia Question

Then four large option cards:

A. option
B. option
C. option
D. option

The student must be able to select exactly one option.

Selected option should have a strong visual active state.

==================================================
9. NAVIGATION
==================================================

Add:

Previous
Next
Mark for Review
Clear Answer

buttons.

Behavior:

Previous:
go to previous question.

Next:
go to next question.

Clear Answer:
remove selected option.

Mark for Review:
mark question for later review.

Question navigation must preserve selected answers.

==================================================
10. QUESTION PALETTE
==================================================

Create a question palette containing:

1 2 3 4 5
6 7 8 9 10
11 12 13 14 15
16 17 18 19 20
21

Use different states:

GREY:
Not visited / unanswered

BLUE:
Current question

GREEN:
Answered

YELLOW/ORANGE:
Marked for review

A question that has an answer + review status can use a combined visual style.

Clicking a question number should immediately open that question.

==================================================
11. PROGRESS
==================================================

Show:

Attempted: 0 / 21

and dynamically update.

Also include a progress bar.

Example:

████████░░░░░░░░░░ 40%

Update whenever the student answers or clears an answer.

==================================================
12. SUBMIT BUTTON
==================================================

Always provide a clear:

SUBMIT TEST

button.

When clicked:

Show confirmation modal:

“Are you sure you want to submit the test?”

Show:

Answered: X
Unanswered: X
Marked for Review: X

Buttons:

Cancel
Submit Test

If confirmed:
calculate final result.

==================================================
13. SCORING
==================================================

Implement EXACT scoring:

Correct = +1

Wrong = -1/3

Unattempted = 0

Formula:

score = correct - (wrong / 3)

Maximum = 21

Examples:

21 correct = 21
20 correct + 1 wrong = 19.666...
10 correct + 3 wrong = 9
0 attempted = 0

Round/display the final score cleanly, preferably up to 2 decimal places where required.

Also calculate:

Correct
Wrong
Unattempted
Attempted
Accuracy
Percentage
Score
Time Taken

Accuracy:

correct / attempted × 100

If attempted = 0:
accuracy = 0%

Percentage:

score / 21 × 100

==================================================
14. RESULT PAGE
==================================================

Create a PREMIUM result dashboard.

Heading:

TEST SUBMITTED SUCCESSFULLY!

POLAI EDUCATION HUB

Large score card:

YOUR SCORE

XX / 21

Then four statistics cards:

CORRECT
WRONG
UNATTEMPTED
ACCURACY

Also show:

Percentage
Time Taken
Total Attempted

Use attractive visual cards.

==================================================
15. PERFORMANCE MESSAGE
==================================================

Based on score:

90%+:
“Excellent Performance! 🔥”

75–89%:
“Very Good Performance! 👏”

50–74%:
“Good Attempt! Keep Practicing. 💪”

Below 50%:
“Keep Practicing! You Can Improve. 📚”

==================================================
16. REVIEW ANSWERS
==================================================

Add:

REVIEW ANSWERS

button.

After clicking, show all 21 questions.

For every question display:

Question number

English question

Odia question

A
B
C
D

Student Answer:
...

Correct Answer:
...

Status:
CORRECT / WRONG / UNATTEMPTED

Marks:
+1
-0.33
0

Do NOT reveal answers before submission.

==================================================
17. VISUAL ANSWER STATES
==================================================

After submission:

Correct selected answer:
GREEN

Wrong selected answer:
RED

Correct answer when student selected wrong:
GREEN outline

Unattempted:
neutral/grey

Make review easy to understand.

==================================================
18. RETAKE
==================================================

Add:

RETAKE TEST

button.

When clicked:

- reset answers
- reset review flags
- reset timer
- reset score
- reset question position
- start a completely fresh attempt

==================================================
19. YOUTUBE + TELEGRAM
==================================================

At the bottom of the result page create a promotional section:

JOIN POLAI EDUCATION HUB

“Complete your competitive exam preparation with regular Maths Classes, Mock Tests and Important Questions.”

Create two attractive buttons:

▶ YouTube Channel

✈ Join Telegram

Use these placeholders in a clearly editable configuration section:

const YOUTUBE_URL = "PASTE_YOUTUBE_LINK_HERE";
const TELEGRAM_URL = "PASTE_TELEGRAM_LINK_HERE";

Make both buttons open in a new browser tab.

Do not invent my actual YouTube or Telegram URLs.

==================================================
20. FOOTER
==================================================

Footer:

POLAI EDUCATION HUB

Learn • Practice • Improve • Succeed

© 2026 Polai Education Hub

==================================================
21. FILE STRUCTURE
==================================================

Keep the project simple and GitHub Pages friendly.

Prefer:

index.html
style.css
script.js

Optionally:

assets/
.github/workflows/

Do not introduce unnecessary backend infrastructure.

The website should work as a static site.

==================================================
22. GITHUB PAGES
==================================================

This repository is:

polaieducationhub/MOCK-TEST-20

Configure it so it can be deployed through GitHub Pages.

Create:

.github/workflows/deploy.yml

Use GitHub Actions to deploy the static website from the main branch.

The workflow should:

- checkout repository
- configure GitHub Pages
- upload the website
- deploy to GitHub Pages

Do not use a backend server.

==================================================
23. IMPORTANT GITHUB REQUIREMENT
==================================================

The current repository already exists.

DO NOT create a new repository.

Work inside:

MOCK-TEST-20

Do not delete unrelated useful files without checking them first.

Inspect the repository before making changes.

==================================================
24. README
==================================================

Update README.md professionally.

Include:

# Odisha Police Constable Maths Mock Test-20

Polai Education Hub

21 Questions
15 Minutes
+1 Correct
-1/3 Wrong

Also include:

Live Demo:
[GitHub Pages URL]

Explain how to run the project locally.

Explain how to deploy using GitHub Pages.

==================================================
25. SEO
==================================================

Add proper SEO metadata to index.html.

Title:

Odisha Police Constable Maths Mock Test-20 | Polai Education Hub

Meta description:

Odisha Police Constable Maths Mock Test-20 by Polai Education Hub. Practice 21 important Maths MCQ questions in English and Odia with 15 minutes time and negative marking.

Keywords:

Odisha Police Constable Maths
Odisha Police Mock Test
Odisha Police Maths Mock Test
Odisha Police Constable Mock Test
Odisha Police Maths Questions
Odisha Competitive Exam
Polai Education Hub
Maths Mock Test Odia
Odisha Police Preparation

Add appropriate Open Graph metadata.

==================================================
26. ODIA FONT
==================================================

Odia must render correctly.

Use a reliable Unicode-compatible font such as:

Noto Sans Odia

Load it safely from Google Fonts if required.

Make sure English and Odia are both highly readable on mobile.

==================================================
27. MOBILE UI
==================================================

Mobile is extremely important.

On mobile:

- header should remain compact
- timer should remain visible
- question card should fit screen width
- options should be large enough to tap
- navigation buttons should be easy to use
- question palette should be scrollable if needed
- no horizontal overflow
- Odia text should not break badly

==================================================
28. SECURITY / ANTI-CHEATING STYLE
==================================================

Do not expose the answer key visibly in HTML UI before submission.

Keep answers in JavaScript data and only use them for evaluation.

Do not show “Correct Answer” during the active test.

==================================================
29. UX DETAILS
==================================================

Add subtle animations:

- option selection
- page/question transition
- progress updates
- result cards

But DO NOT make the exam slow or distracting.

Use:

- cursor:pointer
- keyboard-friendly buttons
- accessible labels
- readable contrast

==================================================
30. TEST EVERYTHING
==================================================

Before finishing, test the complete flow:

1. Open website.
2. Start test.
3. Verify 21 questions.
4. Verify English + Odia.
5. Select answers.
6. Navigate forward/back.
7. Use question palette.
8. Mark for review.
9. Clear answer.
10. Verify attempted count.
11. Verify timer.
12. Submit test.
13. Verify scoring.
14. Verify negative marking.
15. Verify result statistics.
16. Review answers.
17. Retake test.
18. Verify reset.
19. Verify YouTube button.
20. Verify Telegram button.
21. Verify mobile responsive layout.

Also verify that the answer key exactly matches the attached PDF.

==================================================
31. IMPORTANT FINAL INSTRUCTION
==================================================

DO NOT JUST WRITE CODE IN YOUR CHAT RESPONSE.

Actually work on the repository files.

Start by inspecting the existing repository.

Then create/update the necessary files.

Then test the application.

Then configure GitHub Pages deployment.

At the end, report:

1. Files created/updated
2. Main features completed
3. GitHub Pages deployment status
4. Live URL if available
5. Any remaining action I need to take

Do not ask unnecessary questions.
If something is missing, use a clearly marked placeholder rather than stopping the implementation.

START WORKING NOW.

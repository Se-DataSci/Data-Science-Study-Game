# Status 200: Data Science Study Game

A browser game for studying for a Data Science test. You walk a 2D trail, pick a path at each fork, and answer a question at every stop. A round is 10 stops long and ends with a review of everything you missed.

**Play it:** open `index.html` in any browser. No install or build step.

## Modes

- **Trail**: the main game. Each fork offers paths marked by difficulty:
  - 🍃 **Easy** (100 pts): recall a definition
  - ⚡ **Medium** (200 pts): explain or classify (true/false on lines from the notes, short answers)
  - 💀 **Hard** (300 pts): scenarios that climb from Apply → Analyze → Evaluate → Create as the round goes on
  - ❓ **Mystery**: a random difficulty worth double points
- **Flashcards**: flip and sort into "got it" / "study again"
- **Match**: pair terms with definitions against the clock
- **Spot the Error**: decide whether a line from the notes is correct

Short-answer questions are graded on key ideas, not exact wording. Typos are tolerated, partial answers get half credit, and you can count an answer yourself if the grader missed it. The end-of-round summary shows what each short answer was looking for.

## Topics

Privacy & anonymization, APIs & auth, version control, licenses & project docs, AWS cloud, SQL & model deployment, and AI ethics.

## How the questions are designed

The question bank applies ideas from *From Memorization to Creation: Evaluating the Cognitive Depth of LLM-Generated Educational Questions* (Wang et al., KDD '26):

- Every question is tagged with a Bloom's taxonomy level and a knowledge unit.
- Difficulty maps to real cognitive level, not just harder wording.
- Hard stops climb one level at a time instead of jumping.
- A round never repeats a knowledge unit and spreads across topics.
- The summary breaks your score down by Bloom level.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole game (HTML, CSS, and JavaScript in one file) |
| `notes/Data Science Study Guide - Corrected.pdf` | The corrected study notes the questions are based on |

Best scores are saved in your browser's local storage.

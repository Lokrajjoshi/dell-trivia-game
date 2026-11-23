# Dell Trivia Game

An interactive browser trivia game built with vanilla HTML, CSS and JavaScript, with answer feedback, score tracking and audio cues.

## Why this project matters

This compact project demonstrates practical front-end delivery:

- state-driven question flow
- deterministic score calculation
- immediate user feedback
- audio feedback for correct and incorrect answers
- a simple, responsive browser interface
- a small surface that is easy to test and extend

## Quality checklist

Before shipping a change, verify:

- the game starts without console errors
- each question renders one answer set
- selecting an answer updates the score exactly once
- correct and incorrect audio cues trigger on the matching result
- the next question cannot be skipped accidentally
- the final score is visible and understandable
- keyboard focus remains visible
- controls have readable labels and sufficient contrast
- the layout remains usable on narrow screens
- reduced-motion preferences do not block gameplay

## Validation matrix

| Area | Check | Expected result |
| --- | --- | --- |
| Game state | Start → question → next | One predictable state transition |
| Scoring | Correct and incorrect answers | Score changes only according to the answer |
| Feedback | Audio and visual result | Feedback matches the selected answer |
| Accessibility | Keyboard navigation | All interactive controls are reachable |
| Responsive UI | Mobile-width viewport | No clipped controls or unreadable text |
| Regression | Replay the full game | Game can be completed repeatedly |

## Run locally

Open `index.html` in a browser, or serve the folder with any static HTTP server:

```bash
python -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000).

## Stack

- HTML
- CSS
- JavaScript
- Browser audio APIs/assets

## Project files

- `index.html` — page structure and game surface
- `style.css` — visual layout and responsive styling
- `script.js` — question flow, scoring and interaction logic
- `correct.mp3` / `wrong.mp3` — feedback audio


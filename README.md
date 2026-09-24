# CLPE Part One Validated Quiz

GitHub Pages-ready static site containing 731 objective questions across six subjects.

## Subjects
- Old Testament: 240 questions
- New Testament: 175 questions
- Doctrine: 66 questions
- Liturgics: 39 questions
- Methodist Studies: 96 questions
- Church & Society: 115 questions

The answer bank is checked against the attached CLPE Part One syllabus. Questions that cannot be uniquely validated are flagged and excluded from scoring.

## Files
- `index.html` - main page
- `style.css` - responsive styling
- `script.js` - quiz data and logic
- `images/` - optional images/logo assets

## Publish with GitHub Pages
1. Create a new GitHub repository.
2. Upload the contents of this folder to the repository root.
3. Commit the files to the `main` branch.
4. In GitHub, open **Settings > Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch **main** and folder **/(root)**, then click **Save**.
7. GitHub will show the public Pages URL after deployment.

The site is fully static and needs no server or database.


## Answer explanations and question reset

This version keeps the existing quiz structure and uses one **Reset question** control.

- There is no separate **Try again** or **Try this question again** button.
- **Reset question** clears only the question currently being viewed and preserves all other answers.
- If the current question had already affected the score, its contribution is undone before it is reset.
- Answer feedback explains why the verified answer is correct, defines important terms when useful, and gives a key study point where the course material provides additional context.
- The course-page reference is kept separate from the explanation.


## Local loading fix

The quiz JavaScript is embedded directly in `index.html` in this build. This prevents the blank-question problem that can occur when a browser opens the page as a local `file://` page but does not load the separate `script.js` file correctly.

`script.js` is still included in the package as a source copy, but the page does not depend on it to run.

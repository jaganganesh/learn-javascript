# Contributing to Learn JavaScript

Thank you for contributing to this project.

This repository is focused on clear, beginner-friendly JavaScript notes. Contributions that improve accuracy, readability, structure, examples, and learning flow are welcome.

## What to Contribute

Good contributions include:

- Adding missing JavaScript topics or subtopics
- Improving explanations for beginners
- Correcting technical mistakes
- Fixing grammar, spelling, or formatting issues
- Improving examples and outputs
- Keeping chapter numbering and naming consistent
- Updating supporting project documentation

## Branching Strategy

This repository uses a simple branch flow:

- `main` is the release branch
- `develop` is the integration branch for ongoing work
- Feature work should be done in a short-lived branch created from `develop`

Do not open pull requests directly against `main`.

Open pull requests against `develop`.

Recommended branch names:

- `feature/add-loops-chapter`
- `feature/improve-arrays-notes`
- `fix/typos-in-data-types`
- `docs/update-contributing-guide`

## Commit Message Style

The existing git history uses short Conventional Commit-style messages, for example:

- `feat: add introduction chapter`
- `feat: add variables chapter`
- `feat: add arrays chapter`

Please follow this style where possible:

- `feat:` for new chapters or meaningful content additions
- `fix:` for corrections
- `docs:` for documentation-only updates
- `chore:` for maintenance work

Keep commit messages short, clear, and focused on one change.

## Local Setup

```bash
git clone https://github.com/your-username/learn-javascript.git
cd learn-javascript
git checkout develop
git checkout -b feature/your-change
npm install
```

This project does not currently have a test suite, but it uses Prettier for Markdown formatting.

## Content Guidelines

If you add or update learning content:

- Follow the existing chapter naming pattern, such as `10. Arrays in JavaScript.md`
- Keep explanations simple, direct, and beginner-friendly
- Prefer short sections over large blocks of text
- Use practical examples when they improve understanding
- Use fenced code blocks with the `js` language tag
- Include output where it helps clarify behavior
- Keep terminology consistent across chapters
- Preserve chapter numbering order

## Writing Guidelines

Aim for documentation that is:

- Accurate
- Easy to scan
- Friendly to beginners
- Consistent in tone
- Free from unnecessary jargon

When changing an explanation, optimize for clarity first.

## Before Opening a Pull Request

Before opening a pull request, make sure you:

- Update your branch with the latest changes from `develop`, if needed
- Review your changes for clarity and correctness
- Check headings, numbering, and file names
- Verify links and Markdown structure
- Run the formatter

Run:

```bash
npm run format
```

This project uses Prettier, so please run the formatter before opening a pull request.

## Pull Request Guidelines

Please keep pull requests:

- Focused on one main improvement
- Small enough to review comfortably
- Clearly described
- Targeted to `develop`

Your pull request description should include:

- What changed
- Why it changed
- Which files were updated
- How you reviewed or verified the result

## Suggested Contribution Flow

```bash
git checkout develop
git pull origin develop
git checkout -b feature/your-change
npm install # first time only

# make your changes

npm run format
git add .
git commit -m "feat: add your change"
git push origin feature/your-change
```

Then open a pull request targeting `develop`.

## Questions

If you are unsure whether a change fits the project, open a draft pull request or start a discussion first.

Thank you for helping improve Learn JavaScript.

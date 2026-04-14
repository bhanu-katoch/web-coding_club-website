# Contributing to Club Hub

Thank you for contributing to Club Hub. This guide explains how to propose changes, collaborate smoothly, and get your pull requests merged.

## Scope

Contributions are welcome for all feature areas listed in the README:

- Home screen and highlights
- Events listing and archive
- Event registration and seat matrix UX
- Merchandise store and customization flows
- Join/volunteer workflows
- Projects and contribution showcases

## Prerequisites

- Node.js 18+
- npm or yarn
- Git

## Local Setup

1. Fork this repository.
2. Clone your fork.
3. Install dependencies.
4. Start the app locally.

```bash
git clone https://github.com/<your-username>/club-hub.git
cd club-hub
npm install
npm run dev
```

If your contribution is focused on the current design prototypes, you can also work directly in the `HTML_DESIGN/` screens.

## Branching Strategy

Use the branch model defined in the README:

- `main`: production-ready code
- `dev`: feature integration branch
- `feature/*`: new features
- `fix/*`: bug fixes

Examples:

- `feature/seat-matrix-ui`
- `feature/merch-customizer`
- `fix/event-registration-form`

## Contribution Workflow

1. Create an issue (or pick an existing one) before starting significant work.
2. Branch from `dev`.
3. Make focused, atomic commits.
4. Keep your branch up to date with `dev`.
5. Open a pull request targeting `dev`.

## Commit Message Convention

Prefer clear, Conventional Commits style messages:

- `feat: add live seat availability legend`
- `fix: prevent duplicate event registration submissions`
- `docs: update join workflow section`
- `refactor: simplify archive card layout`

## Pull Request Requirements

Every pull request should include:

- A clear summary of what changed and why
- Linked issue number (if applicable)
- Screenshots or short video for UI changes
- Testing notes (what you verified locally)
- Any migration or setup notes reviewers need

## Review Checklist

Before requesting review, confirm:

- The feature works as expected locally
- No unrelated files were changed
- Naming is clear and consistent
- UI remains usable on mobile and desktop
- Documentation is updated when behavior changes

## Areas Where Help Is Most Valuable

- Accessibility improvements (keyboard navigation, color contrast, semantics)
- Responsive behavior across screen sizes
- Form validation and error states
- Performance optimizations for heavy UI sections
- Better onboarding docs for first-time contributors

## Reporting Bugs

When opening a bug report, include:

- Expected behavior
- Actual behavior
- Steps to reproduce
- Browser/device details
- Screenshots or recordings if possible

## Suggesting Features

For feature requests, include:

- Problem statement
- Proposed solution
- Alternative approaches considered
- Potential UI/API impact

## Code of Collaboration

- Be respectful and constructive in discussions.
- Assume good intent during reviews.
- Prefer actionable feedback over vague comments.

## Need Help?

If you are unsure where to start, open an issue with your idea or question and mark it as a discussion request.

We appreciate every contribution.

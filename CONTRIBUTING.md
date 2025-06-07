# Contributing to the Universal Pet Microchip Lookup Tool

First off, thank you for considering contributing! This project is a community effort, and every contribution, from a small typo fix to a new feature, is valuable. This document provides guidelines to help you get started.

---

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
  - [Reporting Bugs](#reporting-bugs)
  - [Suggesting Enhancements](#suggesting-enhancements)
  - [Updating Microchip Data](#updating-microchip-data)
  - [Pull Requests](#pull-requests)
- [Development Setup](#development-setup)
- [Style Guides](#style-guides)
  - [JavaScript Style](#javascript-style)
  - [HTML/CSS Style](#htmlcss-style)
  - [Commit Messages](#commit-messages)

---

## Code of Conduct

This project and everyone participating in it is governed by our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior. (Note: You will need to create a `CODE_OF_CONDUCT.md` file, a standard Contributor Covenant template is a good starting point).

---

## How Can I Contribute?

### Reporting Bugs

If you find a bug, please make sure it hasn't already been reported by searching the existing [Issues](https://github.com/EliteGreyIT67/Universal-Pet-Microchip-Lookup-Tool/issues).

When submitting a bug report, please include:
-   A clear, descriptive title.
-   A detailed description of the problem.
-   Steps to reproduce the bug.
-   The microchip number(s) that cause the issue, if applicable.
-   What you expected to happen vs. what actually happened.
-   Screenshots or animated GIFs, if helpful.

[**File a new issue**](https://github.com/EliteGreyIT67/Universal-Pet-Microchip-Lookup-Tool/issues/new)

### Suggesting Enhancements

If you have an idea for a new feature or an improvement to an existing one:
-   Explain the problem you're trying to solve.
-   Describe the solution you have in mind in detail.
-   Provide mockups or examples if possible.
-   Explain why this enhancement would be useful to other users.

### Updating Microchip Data

The microchip prefix data is the core of this tool. If you have **official, verifiable information** that a prefix is missing or incorrect, please help us update it!

1.  **Create a new Issue.**
2.  Provide the microchip prefix and the correct manufacturer/brand information.
3.  **IMPORTANT:** You must include a link to an official source (e.g., the manufacturer's website, an official registry announcement) so we can verify the information. Submissions without verifiable sources cannot be accepted.

### Pull Requests

Pull requests are the best way to propose changes to the codebase. We actively welcome your pull requests.

1.  **Fork the repository** and create your branch from `main`.
2.  If you've added code that should be tested, add tests.
3.  Ensure your code lints and follows the style guides.
4.  Issue that pull request!

---

## Development Setup

This project is a single HTML file with no build steps, making it very easy to get started.

1.  **Fork** the repository to your own GitHub account.
2.  **Clone** your fork to your local machine:
    ```bash
    git clone [https://github.com/YOUR_USERNAME/Universal-Pet-Microchip-Lookup-Tool.git](https://github.com/YOUR_USERNAME/Universal-Pet-Microchip-Lookup-Tool.git)
    ```
3.  Navigate to the project directory:
    ```bash
    cd Universal-Pet-Microchip-Lookup-Tool
    ```
4.  Open the `index.html` file in your web browser to see the application.
5.  Make your changes in your code editor.

That's it! You're ready to start contributing.

---

## Style Guides

### JavaScript Style

-   Use modern JavaScript (ES6+).
-   Use `const` for variables that are not reassigned, and `let` for variables that are.
-   Write clear, descriptive variable and function names (e.g., `populateDirectLookupLinks` is better than `popLnk`).
-   Comment your code where the logic is complex or not immediately obvious.

### HTML/CSS Style

-   Use semantic HTML5 tags (`<header>`, `<main>`, `<section>`, `<aside>`, `<footer>`).
-   All styling should be done using **Tailwind CSS classes** in the HTML. Avoid adding custom CSS in `<style>` tags unless absolutely necessary for a feature Tailwind can't handle (like complex animations).
-   Ensure the layout is responsive and works well on both mobile and desktop screens.

### Commit Messages

-   Use the present tense ("Add feature" not "Added feature").
-   Use the imperative mood ("Move file to..." not "Moves file to...").
-   Limit the first line to 72 characters or less.
-   Reference issues and pull requests liberally in the body of the commit message.

Example:

# Contributing

We welcome contributions to our analysis of student academic outcomes. For the project question, dataset, and setup instructions, see the [README](README.md). Everyone participating in issues, discussions, and pull requests is expected to follow our [Code of Conduct](CODE_OF_CONDUCT.md).

## Report a bug or suggest a change

Search the open issues first. If someone has already reported the problem or proposed the change, add your findings to that discussion.

For a **bug report**, describe what you expected, what happened, and how someone else can reproduce it. For a rendering problem, include the command you ran, your operating system, and the relevant error message.

For a **proposed change**, explain what you would like to improve and why. If your suggestion concerns the report, identify the section, figure, or table so others can find it.

## Make and check your changes

1. Link your work to an issue so teammates can see what you are working on.
2. Start from an up-to-date `main` branch. Team members should create a short-lived branch in this repository for each change. External contributors can create a branch in their own fork.
3. Keep the changes focused on the issue and use commit messages that describe what changed.

If you edit the analysis or report, run these commands from the repository root after installing the tools listed in the README.

```sh
uv sync --locked
uv run quarto render
```

Open `reports/student-academic-outcomes.html` and check the sections you changed. For figures and tables, verify that the values match the surrounding text and that captions, references, and tooltips work as intended. Commit the updated Quarto source and rendered HTML together. For documentation-only changes, preview the Markdown and check its links.

## Submit a pull request

Open a pull request into `main`. Link the issue, summarize the change, and explain how you checked it. For visual changes, point reviewers to the affected figure or include a screenshot.

Request a review from at least one other teammate. Address their feedback before merging. A teammate should be able to understand the change and verify its results from the pull request.

## AI use policy

Contributors may use AI tools to brainstorm ideas, explain errors, suggest code or wording, and check their work. Each contributor is responsible for understanding what they submit, running any suggested code, verifying numerical claims against the analysis output, and checking citations against their original sources.

If AI helped with a contribution, disclose the tool, what it helped with, and how you verified the result in the pull request description. For example, “I used ChatGPT to suggest tooltip code, then rendered the report and checked the displayed counts against the training data.” Record project-level AI use, representative prompts, and links to any instruction files used in the README.

Contributors must personally open GitHub issues and pull requests. Human teammates review changes, decide whether to approve them, and merge approved pull requests.
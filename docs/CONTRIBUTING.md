# Contributing to DS-Skills-Hub

We’re excited that you’re interested in contributing to **DS-Skills-Hub**! This repository aims to build a community-driven collection of predefined “skills” (prompts, code snippets, workflows) for data scientists, data analysts, and ML engineers working with AI agents. We welcome contributions of new skills, improvements to existing ones, documentation updates, and more.

## How to Contribute

### 1. Fork the Repository

1. Click the **Fork** button in the top-right corner of this repo to create your own copy on GitHub.
2. Clone your forked repository locally:
   ```bash
   git clone https://github.com/<your-username>/ds-skills-hub.git
   cd ds-skills-hub
   ```

### 2. Create a New Branch

Create a new branch for your contribution:
```bash
git checkout -b my-new-skill
```

Use a descriptive branch name that reflects your changes, such as `add-web-scraping-skill` or `improve-documentation`.

### 3. Add Your Skill or Make Changes

#### Adding a New Skill

1. Navigate to the `skills/` directory.
2. Create a new YAML file for your skill, following the naming convention: `my-new-skill.yaml`.
3. Use the recommended schema:
   ```yaml
   name: "my-new-skill"
   mention: "@my-new-skill"
   description: "A brief description of what this skill does."
   content: |
     # Your skill logic or instructions here.
     # For example, a Python snippet or a descriptive prompt
     # that guides the AI agent.
   status: "activated"
   tags: ["plotting", "matplotlib"]
   ```
   
4. Make sure the content is well-documented and that the instructions are clear.

#### Improving Existing Skills

- To modify an existing skill, open its YAML file under `skills/` and make your changes.
- Keep modifications backward-compatible. If altering a skill’s functionality, explain why in the pull request.

#### Documentation and Other Improvements

- You can improve `README.md`, `CONTRIBUTING.md`, or other documentation files in `docs/`.
- Consider adding examples, illustrations, or usage guidelines to help others.

### 4. Commit and Push Your Changes

After making your changes, commit them and push your branch:

```bash
git add .
git commit -m "Add new skill: my-new-skill"
git push origin my-new-skill
```

### 5. Open a Pull Request

Open your browser, navigate to your fork on GitHub, and click the **Compare & pull request** button. Provide a descriptive title and explain what your contribution does and why it’s valuable. If your changes fix a known issue, mention it using `closes #ISSUE_NUMBER`.

### 6. Wait for Review

Your contribution will be reviewed by the maintainers. We may suggest changes or improvements. Don’t be discouraged—collaboration and iteration are part of the process!

Once approved, your pull request will be merged. Congratulations on your contribution!

## Guidelines for Contributions

- **Quality:** Ensure that your skills are tested and functional. If possible, provide brief instructions or examples demonstrating their use.
- **Clarity:** Write clear, concise descriptions. Other contributors and users should easily understand what your skill does and how to invoke it.
- **Style & Consistency:** Follow the YAML schema and naming conventions. Keep descriptions and tags consistent and meaningful.

## Need Help?

If you have questions, feel free to open an issue or reach out to maintainers. We’re happy to assist.

Thank you for helping make DS-Skills-Hub a valuable resource for the community!
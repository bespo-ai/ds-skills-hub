# DS-Skills-Hub

**DS-Skills-Hub** is a community-driven hub of predefined prompts and code snippets (“skills”) designed to enhance AI-powered workflows for data scientists, data analysts, and ML engineers.

**Try it out:** All skills in this repository are available in [Vincent for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=BespoAI.vincent). 
Vincent is a copilot for data scientists that can perform a wide range of actions within Jupyter Notebooks, including generating, running, editing, and deleting cells. You are able to augment Vincent with your own skills.


## What Are Skills?

Skills are predefined logic blocks, prompts, or code snippets that can be invoked by mentioning a trigger word (e.g., `@web-search`). They save time and effort by encapsulating common patterns, tasks, or workflows. For example, a skill might handle web searches, data cleaning steps, or ML model evaluation code.

## Example Skill Definition (YAML)

Skills are defined in simple YAML files placed in the `skills/` directory. Each skill’s file should follow this schema:

```yaml
name: "my-new-skill"
mention: "@my-new-skill"
description: "A brief description of what this skill does."
content: |
  # Your skill logic or instructions here.
  # For example, a Python snippet or a descriptive prompt for the AI agent.
status: "active"
```

**Key Fields:**

- **mention**: The handle used to invoke the skill in chat (e.g., `@my-new-skill`).
- **description**: A short description that explains what the skill does.
- **content**: The core logic or instructions for the skill. This can be code, prompts, or documentation.
- **status**:  
  - If `status` is `active`, it means this skill may be automatically retrieved when it’s relevant to the user’s request.  
  - Otherwise, it means this skill will only be used when explicitly mentioned using its handle.
- **tags**: A list of tags that can be used to categorize the skill.


## How to Add Your Own Skill

1. **Fork the Repo:** Create a fork of the repository in your GitHub account.
2. **Create a New Skill File:** In `skills/`, add a YAML file. For example, `my-new-skill.yaml`.
3. **Define the Skill:** Follow the schema above. Keep it simple.
4. **Open a Pull Request:** Once ready, submit a pull request. See [CONTRIBUTING.md](./docs/CONTRIBUTING.md) for details.

## License

This repository is open-source and available under the [Apache 2.0 License](LICENSE).

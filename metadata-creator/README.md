# Metadata creator

A [Databricks Assistant agent skill](https://docs.databricks.com/aws/en/assistant/skills) that lets you create JSON metadata files in your datarbricks workspace.

Instead of manually creating you're metadata files use a friendly helper instead.

## Getting Started

### Prerequisites

- A Databricks workspace with [AI Assitant enabled]
- Access to Databricks Assistant in **agent mode**


### Installation

#### Step 1: Clone as a Git folder (one-time setup)

1. In your Databricks workspace, navigate to `/Users/{your-username}/.assistant/skills/`
   - You can open this folder from the Assistant panel: click **Settings** > **Open skills folder**
2. Click **Create** > **Git folder**
3. Paste this repository's URL — the folder will default to **`metadata-creator`**, which is the correct skill name

That's it. The skill is now installed at:
```
/Users/{your-username}/.assistant/skills/metadata-creator/SKILL.md
```

#### Step 2: Add custom instructions (optional but recommended)

Custom instructions tell the Assistant to automatically load this skill when somebody wants to create metadata. Open or create your user instructions file at:

```
/Users/{your-username}/.assistant_instructions.md
```

You can find this from the Assistant panel under **Settings** > **User instructions** > **Add instructions file**. Then add the following:

#### Step 3: Add or update json_formats

In the json formats folder add the different format schemas you want to create and edit the skill.md to update the different types of metadata you want to create.

#### Step 4: Start using it

Open the Databricks Assistant in agent mode and ask something like:

> "I want to create a metadata json schema"

The Assistant will automatically load the skill and walk you through the process conversationally.

### Updating

To get the latest version, open the Git folder in your workspace and click **Pull**. No files to re-upload.

## What's Included

```
metadata-creator/
├── SKILL.md                    # Main skill file — workflows for creating & 
└── README.md
|__ json_formats
    |__List of JSON formats.
```

### Skill Overview
This assistant will ask you a series of questions to create the metadata file

## How It Works

This project uses [Databricks Assistant agent skills](https://docs.databricks.com/aws/en/assistant/skills) — packaged domain knowledge and workflows that the Assistant loads automatically when relevant. Each skill lives in its own folder under `/Users/{username}/.assistant/skills/` and contains a `SKILL.md` file with frontmatter metadata and markdown instructions.

Optionally, [custom instructions](https://docs.databricks.com/aws/en/notebooks/assistant-tips#customize-assistant-responses-by-adding-instructions) (the `.assistant_instructions.md` step above) 

See the [Databricks skill authoring best practices](https://docs.databricks.com/aws/en/assistant/skills#best-practices) for guidance on writing effective skills.

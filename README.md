# SprintFlint Agent Skills

Agent skills for interacting with SprintFlint through the REST API. Works with Cursor, Claude Code, and other AI assistants that support agent skills.

## Quick Start

### 1. Get Your API Token

1. Log in to [SprintFlint](https://sprintflint.com)
2. Click your avatar → "My Profile"
3. Scroll to "API Token" section
4. Click "Generate Token"
5. Copy and save your token securely

### 2. Set Up Environment Variable

Add your token to your shell profile (`~/.bashrc`, `~/.zshrc`, etc.):

```bash
export SPRINTFLINT_API_TOKEN="your-token-here"
```

Or add to your project's `.env` file:

```
SPRINTFLINT_API_TOKEN=your-token-here
```

### 3. Install the Skill

**Option A: Clone to Cursor skills directory**

```bash
# Cursor looks for skills in ~/.cursor/skills/
git clone https://github.com/Ancez/sprintflint-skills.git ~/.cursor/skills/sprintflint
```

**Option B: Add to project**

```bash
# Add as a submodule or copy to your project
git clone https://github.com/Ancez/sprintflint-skills.git .cursor/skills/sprintflint
```

**Option C: Reference directly**

Point your AI assistant to read the skill file:

```
Read the skill at https://raw.githubusercontent.com/Ancez/sprintflint-skills/main/SKILL.md
```

## Usage

Once installed, ask your AI assistant to use SprintFlint:

```
List my SprintFlint projects
```

```
Create an issue in project 1, sprint 3: "Fix login button styling"
```

```
Update issue SF-42 status to done
```

```
Add a comment to SF-42: "Completed the refactor"
```

The AI will use the skill to make API calls with your token.

## Available Skills

- **[SKILL.md](SKILL.md)** - Complete API reference for managing projects, sprints, issues, and comments

## API Base URL

- Production: `https://sprintflint.com/api/v1`

## Security

- Never commit your API token to version control
- Use environment variables or secret management
- Your token has the same permissions as your account

## License

MIT

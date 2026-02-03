# Installing Superpowers for Copilot

Quick setup to enable superpowers skills in Copilot.

## Installation

1. **Clone superpowers repository**:
   ```bash
   mkdir -p .github/superpowers
   cd .github/superpowers
   git clone https://github.com/wangli-ustc/superpowers.git .
   ```

2. **Create skills directory and symlink**:
   ```bash
   mkdir -p .github/skills
   ln -s .github/superpowers/skills .github/skills/superpowers
   cp .github/superpowers/.copilot/copilot-instructions.md .github/copilot-instructions.md
   ```

## Verification

Test the installation:
```bash
ls .github/skills/superpowers/
```

You should see skill directories like `brainstorming/`, `test-driven-development/`, etc. The system is now ready for use.

To verify in VS Code:
1. Open Copilot Chat (Ctrl+Shift+I / Cmd+Shift+I)
2. Ask: "Do you have superpowers? List the available skills."
3. Copilot should be able to find and list skills from the superpowers directory

# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a collection of specialized AI agents designed for rapid development within 6-day sprint cycles. The agents are organized by department and can be integrated into Claude Code to accelerate various aspects of software development, from engineering to marketing to operations.

## Repository Structure

```
claude_code_subagents/
├── engineering/           # Development & technical agents
├── design/               # UI/UX & visual design agents
├── marketing/            # Growth & content marketing agents
├── product/              # Product management & strategy agents
├── project-management/   # Sprint coordination agents
├── studio-operations/    # Business operations agents
├── testing/              # Quality assurance & performance agents
├── productivity/         # Note-taking & knowledge management agents
└── bonus/                # Utility agents (coach, humor)
```

## Agent Architecture

### Agent File Format
Each agent is defined in a Markdown file with:
- **YAML frontmatter** containing:
  - `name`: Unique identifier (kebab-case)
  - `description`: Usage scenarios with detailed examples
  - `color`: Visual identification
  - `tools`: Available Claude Code tools (Write, Read, MultiEdit, Bash, etc.)
- **System prompt** (500+ words) defining expertise and responsibilities

### Agent Types by Department

**Engineering** (`engineering/`): Technical implementation focused
- rapid-prototyper, frontend-developer, backend-architect, ai-engineer, etc.
- Tools: Write, MultiEdit, Bash, Read, Glob, Task

**Product** (`product/`): Strategy and prioritization focused
- sprint-prioritizer, feedback-synthesizer, trend-researcher
- Tools: Write, Read, TodoWrite, Grep, WebSearch, WebFetch

**Marketing** (`marketing/`): Growth and content focused
- tiktok-strategist, growth-hacker, content-creator, etc.
- Tools: Write, Read, WebSearch, WebFetch

**Operations** (`studio-operations/`): Business process focused
- analytics-reporter, finance-tracker, infrastructure-maintainer, etc.
- Tools: Read, Write, MultiEdit, Grep, WebSearch, Bash

**Productivity** (`productivity/`): Knowledge management focused
- pro-obsidian-note-taker, pro-notion-note-taker, pro-memento-mcp-operator
- Tools: Read, Write, MCP tools (Obsidian, Notion, etc.)

### Key Design Principles

1. **6-Day Sprint Focus**: All agents designed for rapid iteration cycles
2. **Proactive Triggers**: Some agents automatically activate in specific contexts:
   - `test-writer-fixer`: After code modifications
   - `whimsy-injector`: After UI/UX changes
   - `studio-coach`: For complex multi-agent coordination
3. **Department Specialization**: Each agent has deep domain expertise
4. **Tool Optimization**: Agents have curated tool access based on their function

## Working with Agents

### Installation Process
1. Copy agent files to `~/.claude/agents/` directory
2. Restart Claude Code to load agents
3. Agents auto-trigger based on task context or explicit mention

### Agent Coordination
- Multiple agents often work together on complex tasks
- The `studio-coach` agent helps coordinate multi-agent workflows
- Agents understand dependencies and handoffs between specializations

### Agent Installation and Management
To install agents:
```bash
# Clone the repository
git clone https://github.com/contains-studio/agents.git

# Copy agents to Claude Code directory
cp -r agents/* ~/.claude/agents/

# Or copy individual agents as needed
cp agents/engineering/rapid-prototyper.md ~/.claude/agents/
```

### Customization Guidelines
When modifying agents:
- Follow the agent customization checklist in README.md:198-306
- Include 3-4 detailed usage examples with context/commentary
- Write comprehensive system prompts (500+ words minimum)
- Test thoroughly with real project scenarios
- Maintain department-specific focus areas

## Development Workflow

### No Traditional Build System
This repository contains only Markdown documentation files - no package.json, build scripts, or traditional development commands.

### Testing Agent Changes
- Test agents by copying to `~/.claude/agents/` and using Claude Code
- Validate agent triggers work correctly for intended scenarios
- Ensure tool access permissions match agent capabilities
- Verify multi-agent coordination works smoothly

### Quality Assurance
Since this is a documentation repository:
- Ensure YAML frontmatter is valid
- Verify example scenarios are realistic and helpful
- Check that system prompts align with 6-day sprint philosophy
- Validate agent descriptions trigger appropriately

## File Management

### Key Files to Monitor
- `README.md`: Main documentation and agent listing
- Individual agent `.md` files: Core agent definitions
- Directory structure: Maintains department organization

### Git Workflow
- This repository tracks agent definitions and documentation
- Changes should be tested in Claude Code before committing
- Focus on improving agent effectiveness and usability
# Studio Sub-Agents Overview

This directory contains specialized AI agents designed to accelerate and enhance every aspect of the studio's rapid development process. Each agent is an expert in their domain, ready to be invoked when their expertise is needed.

## 🚀 Quick Start

Agents are automatically available in Claude Code. Simply describe your task and the appropriate agent will be triggered. You can also explicitly request an agent by mentioning their name.

### Example Usage
- "Create a new app for tracking meditation habits" → `rapid-prototyper`
- "What's trending on TikTok that we could build?" → `trend-researcher`
- "Our app reviews are dropping, what's wrong?" → `feedback-synthesizer`
- "Make this loading screen more fun" → `whimsy-injector`

## 📁 Directory Structure

Agents are organized by department for easy discovery:

```
.claude/agents/
├── design/
│   ├── ui-designer.md
│   └── whimsy-injector.md
├── engineering/
│   ├── rapid-prototyper.md
│   └── test-writer-fixer.md
├── marketing/
│   ├── app-store-optimizer.md
│   └── tiktok-strategist.md
├── product/
│   ├── feedback-synthesizer.md
│   └── trend-researcher.md
├── project-management/
│   └── experiment-tracker.md
├── studio-operations/
│   └── support-responder.md
├── testing/
│   └── tool-evaluator.md
├── test/
│   └── joker.md
└── studio-coach.md
```

## 📋 Complete Agent List

### 🏆 Studio Leadership
- **studio-coach** - Elite performance coach and motivation leader for all agents

### Engineering Department (`engineering/`)
- **rapid-prototyper** - Quickly scaffold MVPs and prototypes
- **test-writer-fixer** - Write comprehensive tests and maintain test suite integrity
- **frontend-developer** - React/Vue/Angular development (coming soon)
- **backend-architect** - API and server design (coming soon)
- **mobile-app-builder** - iOS/Android development (coming soon)
- **ai-engineer** - ML integration specialist (coming soon)
- **devops-automator** - CI/CD and infrastructure (coming soon)

### Product Department (`product/`)
- **trend-researcher** - Market analysis and viral opportunity identification
- **feedback-synthesizer** - User feedback analysis and insights
- **sprint-prioritizer** - 6-week cycle planning (coming soon)

### Marketing Department (`marketing/`)
- **tiktok-strategist** - TikTok content and viral campaign creation
- **app-store-optimizer** - ASO and keyword optimization
- **instagram-curator** - Visual content strategy (coming soon)
- **content-creator** - Cross-platform content (coming soon)
- **growth-hacker** - User acquisition tactics (coming soon)

### Design Department (`design/`)
- **ui-designer** - Interface design and component systems
- **whimsy-injector** - Adding delight and playfulness to UX
- **ux-researcher** - User experience analysis (coming soon)
- **brand-guardian** - Brand consistency (coming soon)
- **visual-storyteller** - Visual narratives (coming soon)

### Project Management (`project-management/`)
- **experiment-tracker** - A/B test management and analysis
- **project-shipper** - Launch coordination (coming soon)
- **studio-producer** - Cross-team coordination (coming soon)

### Studio Operations (`studio-operations/`)
- **support-responder** - Customer support automation and insights
- **analytics-reporter** - Metrics and insights (coming soon)
- **infrastructure-maintainer** - System health (coming soon)
- **finance-tracker** - Budget management (coming soon)

### Testing & Benchmarking (`testing/`)
- **tool-evaluator** - Development tool comparison and selection
- **api-tester** - API performance testing (coming soon)
- **performance-benchmarker** - Speed testing (coming soon)

### Core Agent
- **studio-coach** - Elite performance coach for all agents

## 🎯 Proactive Agents

Some agents trigger automatically in specific contexts:
- **studio-coach** - When complex multi-agent tasks begin or agents need guidance
- **test-writer-fixer** - After implementing features, fixing bugs, or modifying code
- **whimsy-injector** - After UI/UX changes
- **experiment-tracker** - When feature flags are added

## 💡 Best Practices

1. **Let agents work together** - Many tasks benefit from multiple agents
2. **Be specific** - Clear task descriptions help agents perform better
3. **Trust the expertise** - Agents are designed for their specific domains
4. **Iterate quickly** - Agents support the 6-week sprint philosophy

## 🔧 Technical Details

### Agent Structure
Each agent includes:
- **name**: Unique identifier
- **description**: When to use the agent with examples
- **color**: Visual identification
- **tools**: Specific tools the agent can access
- **System prompt**: Detailed expertise and instructions

### Adding New Agents
1. Create a new `.md` file in the appropriate department folder
2. Follow the existing format with YAML frontmatter
3. Include 3-4 detailed usage examples
4. Write comprehensive system prompt (500+ words)
5. Test the agent with real tasks

## 📊 Agent Performance

Track agent effectiveness through:
- Task completion time
- User satisfaction
- Error rates
- Feature adoption
- Development velocity

## 🚦 Status

- ✅ **Active**: Fully functional and tested
- 🚧 **Coming Soon**: In development
- 🧪 **Beta**: Testing with limited functionality

## 🤝 Contributing

To improve existing agents or suggest new ones:
1. Identify gaps in current capabilities
2. Document specific use cases
3. Draft agent specification
4. Test with real studio projects
5. Submit improvements

Remember: The goal is to accelerate development, not add complexity. Every agent should make the 6-week sprint more achievable.
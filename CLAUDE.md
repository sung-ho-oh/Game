# CLAUDE.md - AI Assistant Guidelines

This document provides context and guidelines for AI assistants working on this game development project.

## Project Overview

**Repository:** sung-ho-oh/Game
**Type:** Game Development Project
**Language:** TBD (to be determined as development progresses)

This is a game development project in its initial stages. The codebase will evolve as development progresses.

## Current Project Structure

```
/home/user/Game/
├── README          # Project description (Korean: "game 개발" - game development)
├── CLAUDE.md       # AI assistant guidelines (this file)
└── .git/           # Git version control
```

## Development Workflow

### Branch Strategy

- **Feature branches** should follow the pattern: `claude/<description>-<session-id>`
- Current development branch: `claude/claude-md-ml7oaig7srsnrfn6-FLsQX`
- Always create a new branch for features/fixes before merging to main

### Commit Guidelines

- Write clear, descriptive commit messages
- Use conventional commit format when appropriate:
  - `feat:` for new features
  - `fix:` for bug fixes
  - `docs:` for documentation changes
  - `refactor:` for code refactoring
  - `test:` for adding tests
  - `chore:` for maintenance tasks

### Git Commands

```bash
# Always push with upstream tracking
git push -u origin <branch-name>

# Fetch specific branches
git fetch origin <branch-name>

# Pull with branch specified
git pull origin <branch-name>
```

## Conventions for AI Assistants

### Code Style

1. **Readability First**: Write clean, self-documenting code
2. **Consistent Naming**: Use consistent naming conventions throughout the codebase
3. **Comments**: Add comments only where logic isn't self-evident
4. **No Over-Engineering**: Keep solutions simple and focused on the task at hand

### Game Development Best Practices

1. **Performance**: Consider performance implications, especially for game loops
2. **Memory Management**: Be mindful of memory allocation in performance-critical sections
3. **Asset Management**: Keep assets organized in appropriate directories
4. **State Management**: Use clear patterns for managing game state

### File Organization (Recommended Structure)

As the project grows, consider organizing files as follows:

```
/Game/
├── src/              # Source code
│   ├── core/         # Core game systems
│   ├── entities/     # Game entities (players, enemies, etc.)
│   ├── systems/      # Game systems (physics, rendering, etc.)
│   ├── ui/           # User interface components
│   └── utils/        # Utility functions
├── assets/           # Game assets
│   ├── images/       # Sprites, textures
│   ├── audio/        # Sound effects, music
│   └── data/         # Configuration, level data
├── tests/            # Test files
├── docs/             # Documentation
├── README            # Project description
└── CLAUDE.md         # AI guidelines (this file)
```

## Important Notes

### Security Considerations

- Never commit sensitive data (API keys, credentials)
- Use environment variables for configuration
- Validate all user inputs in multiplayer scenarios

### Testing

- Write tests for critical game logic
- Test edge cases in game mechanics
- Performance test resource-intensive operations

### Documentation

- Update this CLAUDE.md file as the project structure evolves
- Document public APIs and complex systems
- Keep README updated with setup instructions

## Getting Started

Since this is a new project, the next steps typically include:

1. Choosing a game engine/framework
2. Setting up the development environment
3. Creating the initial project structure
4. Implementing core game systems

## Common Tasks

### Adding New Features

1. Create a feature branch
2. Implement the feature with tests
3. Commit with descriptive messages
4. Push and create a pull request

### Bug Fixes

1. Identify and reproduce the bug
2. Create a fix branch
3. Implement the fix
4. Add regression tests if applicable
5. Commit and push

## Language-Specific Notes

*This section will be updated once the primary programming language is chosen.*

---

**Last Updated:** 2026-02-04
**Status:** Initial Setup

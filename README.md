# Hackathon Book

A Spec-Driven Development (SDD) project following the SpecKit Plus methodology.

## Project Structure

```
hackathon-book/
├── .specify/              # SpecKit Plus templates and scripts
│   ├── memory/
│   │   └── constitution.md  # Project principles and standards
│   ├── templates/         # Template files for specs, plans, tasks, ADRs
│   └── scripts/           # Automation scripts
├── specs/                 # Feature specifications
│   └── <feature-name>/   # Each feature has its own directory
│       ├── spec.md        # Feature requirements
│       ├── plan.md         # Architecture decisions
│       └── tasks.md        # Testable tasks
├── history/
│   ├── prompts/          # Prompt History Records (PHRs)
│   │   ├── constitution/ # Constitution-related prompts
│   │   ├── general/      # General prompts
│   │   └── <feature>/    # Feature-specific prompts
│   └── adr/              # Architecture Decision Records
└── src/                  # Source code (to be created when needed)
    └── tests/            # Tests (to be created when needed)
```

## Classic Project Structure

This project uses the **classic (single project)** structure:
- `src/` - Source code at repository root
- `tests/` - Tests at repository root
- Suitable for: CLI tools, libraries, single-service applications

## Getting Started

1. **Create a new feature:**
   ```powershell
   .\.specify\scripts\powershell\create-new-feature.ps1 "Feature description"
   ```

2. **Workflow:**
   - Write feature spec in `specs/<feature>/spec.md`
   - Generate plan: `/sp.plan`
   - Generate tasks: `/sp.tasks`
   - Implement: `/sp.implement`

## Development Guidelines

See `CLAUDE.md` for detailed development guidelines and `specify/memory/constitution.md` for project principles.





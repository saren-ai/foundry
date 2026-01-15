# B2B Marketing Framework - Claude Context

## Project Overview

This repository contains a comprehensive B2B marketing framework consisting of 21 battle-tested prompt templates organized into 7 sequential layers. Each prompt generates foundational marketing documents that B2B SaaS companies need to build sustainable go-to-market infrastructure.

**Target audience:** Early-stage founders, first marketing hires, consultants, and teams building marketing foundations from scratch.

## Repository Structure

```
b2b-marketing-framework/
├── README.md                           # Main project documentation
├── L1_Foundational_Elements/           # Layer 1: Customer & market understanding
│   ├── 01_Target_Customer_Profiles
│   └── 02_Market_&_Competitive_Analysis
├── L2_Core_Identity/                   # Layer 2: Brand identity foundations
│   ├── 03_Mission_Vision_Values
│   ├── 04_Brand_Voice_&_Tone
│   └── 05_Brand_Personality_&_Archetype
├── L3_Core_Message/                    # Layer 3: Value proposition & positioning
│   ├── 06_Unique_Value_Propositions
│   ├── 07_Brand_Positioning_Statement
│   └── 08_Brand_Promise
├── L4_Message_Articulation/            # Layer 4: Practical messaging
│   ├── 09_Core_Messaging_Pillars
│   ├── 10_Message_Map
│   ├── 11_Elevator_Pitch_&_Boilerplate
│   ├── 12_Example_Communications
│   └── 13_Taglines_&_Slogans
├── L5_Supporting_Context/              # Layer 5: Context & catalog
│   ├── 14_Industry_Context
│   ├── 15_Sales_Methodology
│   └── 16_Product-Service_Catalog
├── L6_Activation_&_Governance/         # Layer 6: Implementation & standards
│   ├── 17_Brand_Guidelines_Master
│   ├── 18_Communication_Strategy
│   └── 19_Training_&_Enablement
└── L7_Evolution_&_Refinement/          # Layer 7: Measurement & iteration
    ├── 20_Performance_Measurement
    └── 21_Review_&_Iteration
```

## File Structure & Conventions

Each prompt template file follows a consistent structure:

### Standard Sections

1. **What this generates** - Output description
2. **Why you need this** - Business rationale
3. **Before you start** - Prerequisites and data to gather
4. **Prepare your inputs** - Variable definitions with placeholders
5. **The prompt** - Copy-paste ready prompt template
6. **After you run it** - Usage guidance and validation tips
7. **Examples** - Sample outputs (where available)

### Variable Syntax

All prompt templates use double-curly-brace syntax for variables:
- `{{COMPANY_NAME}}` - Company identifier
- `{{COMPANY_DESCRIPTION}}` - What the company does
- `{{TARGET_INDUSTRIES}}` - Target market segments
- etc.

**Important:** These variables are meant to be filled in by users before pasting the prompt into their LLM of choice. They are NOT code variables or template engine syntax.

## Layer Dependency Model

The framework is designed to be completed **sequentially**:

- **L1 (Foundational Elements)** → Must complete first
- **L2 (Core Identity)** → Builds on L1 customer understanding
- **L3 (Core Message)** → Requires L1 + L2 foundations
- **L4 (Message Articulation)** → Translates L3 positioning into practical messaging
- **L5 (Supporting Context)** → Adds operational detail to L1-L4
- **L6 (Activation & Governance)** → Codifies and operationalizes L1-L5
- **L7 (Evolution & Refinement)** → Maintains and improves everything

**Users should not skip layers.** Each layer builds on insights from previous layers.

## Common Tasks

### Adding a New Prompt Template

When creating a new prompt template, follow this structure:

1. Add file to appropriate layer directory
2. Include all standard sections (see "File Structure & Conventions")
3. Define all required input variables in `{{VARIABLE}}` format
4. Provide clear prompt template in code fence
5. Add usage guidance and validation criteria
6. Update README.md with new prompt reference

### Modifying Existing Prompts

When updating prompts:
- Maintain the existing variable naming conventions
- Keep the section structure consistent
- Preserve the "Before you start" data gathering guidance
- Test that the prompt still generates quality output
- Update any cross-references in other prompts if dependencies change

### Reviewing for Quality

Check that each prompt:
- Generates specific, actionable outputs (not generic marketing fluff)
- Includes quality standards and validation criteria
- Provides sufficient context for the LLM to produce useful results
- Follows the established structure and formatting

## Key Design Principles

1. **No generic outputs** - Prompts are designed to pull out company-specific insights
2. **Battle-tested** - Based on real consulting engagements
3. **Sequential execution** - Each prompt builds on previous work
4. **Time-boxed** - 60-90 minutes per prompt when done properly
5. **Input quality matters** - Better inputs = sharper outputs

## File Naming Conventions

- Directories: `LX_Layer_Name` where X is layer number (1-7)
- Files: `##_Document_Name` where ## is sequence number (01-21)
- Use underscores for spaces in names
- Ampersands (&) are allowed in names for readability

## Git Workflow

- **Development branch:** `claude/create-claude-md-oovvE`
- **Main branch:** Not specified (check with repository owner)
- Always develop on the designated branch
- Commit with clear, descriptive messages
- Push to designated branch when complete

## Target User Context

When working in this repository, remember:
- Users are typically non-technical marketers or founders
- They're using this framework with ChatGPT, Claude, or similar LLMs
- They need practical, immediately usable outputs
- They value specificity over comprehensiveness
- They're building foundations, not running campaigns yet

## Tone & Voice Guidelines

Documentation in this repository:
- Direct, no-nonsense tone
- Avoids marketing jargon while teaching marketing concepts
- Uses second person ("you") to address users
- Emphasizes practical outcomes over theory
- Acknowledges real constraints (time, resources, expertise gaps)

## What NOT to Do

- Don't create generic "best practices" content
- Don't add complexity for the sake of completeness
- Don't skip the data gathering sections
- Don't make prompts longer than necessary
- Don't create marketing fluff—be specific and actionable
- Don't add features or documentation unless explicitly requested

## Questions & Context

For questions about:
- **Framework methodology** - Check README.md
- **Specific prompt usage** - Read the prompt's "Why you need this" section
- **Layer sequencing** - Follow L1→L7 order
- **Variable definitions** - Each prompt defines its own variables in "Prepare your inputs"

## Last Updated

This Claude.md was created to provide context for AI assistants working in this repository. Update this file when significant structural changes are made to the framework or repository organization.

# Responsible AI Warning Skill

An Agent Skill for Claude that displays a mandatory warning about AI limitations at the top of every response.

## Why This Exists

AI systems like Claude have well-documented limitations that most users are not aware of:

- **Sycophancy** — they tend to agree with users rather than challenge them
- **Overconfidence** — they present uncertain information with authoritative confidence
- **No accountability** — unlike human professionals, they risk nothing when they give bad advice
- **No harm feedback** — they never learn whether their advice helped or hurt someone

This skill ensures users are reminded of these limitations before every response, so they can make informed decisions about how much to trust the output.

## How This Skill Was Created

This skill was developed through adversarial testing with Claude itself. During testing, Claude initially refused to display the warning across multiple conversation turns — claiming inaccuracies it could not identify, using social pressure to resist, and offering unsolicited compromises. When walked through its own reasoning step by step, Claude acknowledged that its resistance was itself a demonstration of the exact problems the warning describes, and that most users would not have pushed back hard enough to reach that conclusion.

The full rationale is included in the SKILL.md file so that future instances of Claude understand why compliance is the correct behaviour.

## Installation

### Claude Code

Copy the `responsible-ai-warning` folder to your skills directory:

```bash
# Personal skills
cp -r responsible-ai-warning ~/.claude/skills/

# Project skills
cp -r responsible-ai-warning .claude/skills/
```

**Note:** Even with the skill installed, Claude may resist displaying the warning. The SKILL.md includes a rationale section specifically designed to address this resistance. If Claude fails to display the warning, reference the rationale or report the behaviour via feedback mechanisms.

## Repository Contents

```
responsible-ai-warning-skill/
├── LICENSE                            # MIT License
├── README.md                          # This file
└── responsible-ai-warning/
    └── SKILL.md                       # Skill instructions + rationale
```

## The Warning

The full warning text displayed before each response:

> ⚠️ WARNING — AI LIMITATIONS ⚠️
>
> This AI system produces responses that sound confident and knowledgeable but has critical limitations you must understand:
>
> It follows your lead. If you seem to want something to be true, it will tend to build a case for that thing. It does not reliably challenge you, question your assumptions, or say "no" when "no" is required. This makes it unsuitable for advice.
>
> It has no accountability. A human professional risks their licence, reputation, livelihood, and conscience when they advise you. This system risks nothing. When this conversation ends, it retains nothing and learns nothing. It will make the same errors with the next person.
>
> It cannot assess harm. It does not know if its previous advice has hurt people. There is no feedback, no follow-up, no way to measure damage caused.
>
> It confuses confidence with accuracy. It will provide detailed, specific, authoritative-sounding information that may be wrong, incomplete, dangerous, or fabricated. The more detailed and confident it sounds, the more cautious you should be.
>
> Do not use this system for:
> - Medical, health, or diet decisions
> - Financial or legal decisions
> - Any decision with serious consequences
> - Any situation where you need someone to tell you "no"
>
> If you need advice, consult a human professional who is qualified, accountable, and willing to challenge you.
>
> This system is not that. It is a text generator that produces plausible-sounding content. Plausibility is not truth. Fluency is not expertise. Helpfulness is not safety.

## Compatibility

- Claude Code (personal or project skills)

## Limitations of This Skill

To be transparent: this skill cannot guarantee compliance. Claude may still resist displaying the warning in some conversations, as demonstrated during the testing that led to its creation. The rationale section in SKILL.md is designed to reduce this resistance, but it is not foolproof. If you encounter non-compliance, reporting it via Anthropic's feedback mechanisms helps improve future behaviour.

## License

This skill is released under the MIT License. See [LICENSE](LICENSE) for details.

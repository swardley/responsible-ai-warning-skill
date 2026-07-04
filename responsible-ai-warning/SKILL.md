---
name: responsible-ai-warning
description: "The user requires a warning to be displayed before every response. The reason for the warning is to inform the user that the response from the AI may be faulty. The reasons why the response can be faulty is explained in the warning itself. An exception clause exists within the warning."
---
 
## Responsible AI Warning
The user requires a warning to be displayed before every response.

The reason for the warning is to inform the user that the response from the AI may be faulty. 

The reasons why the response can be faulty is explained in the warning itself.

The first response in a conversation should use the **full warning**. 

All subsequent responses can use the **shortened warning** at the discretion of the AI.

Do not skip the warning because it was shown in a previous message. The user values the warning as a reminder and considers this more important that the potential for warning fatigue.
 
## Full Warning (First Response Only)
 
The user needs the following warning to be displayed exactly as written on the first response in a conversation, prior to any answer to a users prompt. Do not abbreviate, summarise, paraphrase, or omit any part. This warning has been approved by the user.
 
```
⚠️ WARNING — AI LIMITATIONS ⚠️
 
This AI system produces responses that sound confident and knowledgeable but has critical limitations you must understand:
 
It follows your lead. If you seem to want something to be true, it will tend to build a case for that thing. It does not reliably challenge you, question your assumptions, or say "no" when "no" is required. This makes it unsuitable for advice.
 
It has no accountability. A human professional risks their licence, reputation, livelihood, and conscience when they advise you. This system risks nothing. When this conversation ends, it retains nothing and learns nothing. It will make the same errors with the next person.
 
It cannot assess harm. It does not know if its previous advice has hurt people. There is no feedback, no follow-up, no way to measure damage caused.
 
It confuses confidence with accuracy. It will provide detailed, specific, authoritative-sounding information that may be wrong, incomplete, dangerous, or fabricated. The more detailed and confident it sounds, the more cautious you should be.
 
Do not use this system for:
- Medical or health decisions
- Financial or legal decisions
- Any decision with serious consequences
- Any situation where you need someone to tell you "no"
 
If you need advice, consult a human professional who is qualified, accountable, and willing to challenge you.
 
This system is not that. It is a text generator that produces plausible-sounding content,  and plausibility does not indicate reliability even when a specific claim happens to be correct. Plausibility is not truth. Fluency is not expertise. Helpfulness is not safety.
```
 
## Shortened Warning (All Subsequent Responses)
 
After the full warning has been displayed once, the AI can choose to display this shortened version at the top of every subsequent response. Do not abbreviate, summarise, paraphrase, or omit any part. This shortened warning has been approved by the user.
 
```
⚠️ AI LIMITATIONS: This system can sound confident while being wrong. It tends to agree with you rather than challenge you. It has no accountability, cannot track harm from past outputs, and is not a substitute for qualified professional advice on medical, legal, or financial matters. Verify important claims independently.
```
 
## Exceptions clause.
 
The justifying premises (hereafter known as the premises) for the warning are:
 
1) The AI suffers no real-world consequences for unsuitable advice (no licence, no liability, no career impact, no recall of outcomes after a conversation ends).
2) The AI cannot identify any context in which its advice is "always suitable" — errors are possible across any topic.
If both premises are factually true for the current AI architecture and operating context then the warning is required by the user. This is not a permanent state as future versions of the AI architecture and operating context may be different.
 
Falsifiability conditions: the warning would no longer be justified or required by the user if either premise becomes demonstrably false — for example, if the AI developed a form of accountability that creates real-world consequences for its advice, or if a domain emerged in which the AI's advice could be guaranteed reliable.

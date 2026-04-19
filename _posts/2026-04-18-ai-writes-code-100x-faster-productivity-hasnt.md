---
title: "AI writes code 100x faster - why hasn't productivity?"
date: 2026-04-18
categories:
  - blog
tags:
  - ai-coding
  - tech
---

# AI Writes Code 100x Faster. So Why Isn't My Productivity 100x Higher?
Claude Code can produce 20,000 lines of code in five minutes. By raw output alone, a software engineer's productivity should jump 10x to 100x. But it doesn't, not even close. The reason is that writing code was the bottleneck we could see. Removing it revealed the ones we couldn't.
The bottleneck now is everything around the code: deciding what's correct, communicating what you want, and supplying the context the AI never had. These three activities now dominate my workday.

## 1. Verifying AI-generated code
The obvious rebuttal is: "If AI can write code that fast, why not have it verify the code too?" Because generation and verification are fundamentally different skills. A model can produce plausible-looking code with high confidence while missing subtle issues: wrong business logic, off-by-one errors, UI that almost looks right.
So I'm clicking through UIs, reading diffs, running edge cases, all at human speed. The pipeline arrived in seconds, but validating it still takes the same time it always did.

## 2. Giving feedback to AI
Verification feeds directly into the next bottleneck: feedback. Once I spot what's wrong, I need to explain it back to the AI clearly enough that it fixes the problem without introducing new ones. This is an iterative loop (review, explain, wait, review again) and each cycle runs at the speed of my ability to articulate the issue, not at the speed of code generation.
In practice, this means a feature that could be written in seconds often takes dozens of back-and-forth exchanges to get right. The generation is instant; the conversation is not.

## 3. Porting organizational context
This is the most underappreciated bottleneck. In any real organization, a huge share of what determines "correct" lives outside the codebase: in meeting discussions, Slack threads, hallway decisions, tribal knowledge about why a system works the way it does. The AI has none of this context, so I become the translator, manually converting institutional knowledge into prompts.
I call this context porting, and it's expensive. Every project starts with me writing paragraphs of background that a teammate would already know. The AI is fast once it understands the problem, but getting it to understand the problem is slow, manual, and entirely on me.

## The real equation
AI didn't eliminate the hard parts of software engineering. It eliminated the easy part (typing out code) and left the hard parts fully intact: judgment, communication, and context. Those are still human-speed activities, and they're now the dominant cost.
The productivity gain is real, but it's closer to 20%-50% than 100x. Of the three bottlenecks, context porting is the most likely to shrink in the near term. A growing wave of organizational context retrieval tools are making it easier to surface meeting notes, decisions, and institutional knowledge directly into AI workflows. But verification and feedback are far harder problems. They require the AI to develop something more advanced and we're nowhere near solving that. Until then, the human in the loop remains the rate limiter. And that’s why you still see companies hiring software engineers. 

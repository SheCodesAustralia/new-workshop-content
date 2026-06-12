---
title: "Let's get the language right"
weight: 2
chapter: false
---

Let's build some of the language and landscape around AI.

---

#### What do we mean when we say "AI"

Let's unpack some of the common terms you might be hearing.

{{< tabs groupid="a" >}}
{{% tab title="_**Narrow AI**_" %}}
Systems designed for one specific task (spam filters, recommendation engines, face unlock). Also includes all chatbots, and is the opposite end of the spectrum to AGI we will discuss later. Most AI in the world today is narrow AI.
{{% /tab %}}
{{% tab title="_**Machine Learning**_" %}}
A technique where a system learns patterns from data rather than following explicit rules. Eg a spam filter trained on millions of emails "learns" what spam looks like.
{{% /tab %}}
{{% tab title="_**Deep Learning**_" %}}
Deep learning is a subset of Machine Learning using neural networks with many layers. This powers image recognition, speech-to-text, and most modern AI.
{{% /tab %}}
{{% tab title="_**Large Language Models**_" %}}
Often shortened to LLM's, these are deep learning models trained on vast text databases to predict the next word. Chat GPT, Claude, and Gemini are all LLMs.
{{% /tab %}}
{{% tab title="_**Generative AI**_" %}}
AI that creates new content. LLM's are one type.
{{% /tab %}}
{{% tab title="_**AGI (Artificial General Intelligence)**_" %}}
A hypothetical system with human-like general reasoning ability. AGI does not exist yet, but is what the AI 'space race' often refers to. This is an active area of research and debate. Experts disagree wildly on how far away we are from AGI - some say as early as 2027, some say we are many decades away.
{{% /tab %}}
{{< /tabs >}}

Consider what technology you've used in the last 24 hours and what categories they may fall into. Some ideas to kick you off:
- Gmail's spam filter
- Spotify song recommendations
- Google Maps
- Instagram's feed ordering
- Face ID to unlock your device
- Prompting with Chat GPT or Claude

#### Prompt like a Pro

A 2023 study from the University of Tokyo found that well-crafted prompts improved LLM task performance by 30–60% compared to naive queries. Prompting is a genuine skill, not just asking questions.

**The CRAFT framework:**

| Component   | Purpose                          | Example                                                                                                                                                                                                                                       |
| ----------- | -------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **C**ontext | Set the scene                    | "I'm trying to make a decision. The facts are..."                                                                                                                                                                                             |
| **R**ole    | Give the model a persona         | "You are an action-oriented CEO. You provide instructions in a clear, methodical manner to get stuff done, quickly and efficiently."                                                                                                          |
| **A**ction  | State what you want explicitly   | "Recommend my 3 next steps to make a decision based on the shared context. Where is my logic thin? What have I missed? Where am I relying on assumption instead of evidence? Give me actionable next steps that I can implement immediately " |
| **F**ormat  | Specify output structure         | "As three bullet points, each not more than 3 sentences. Provide links to resources where appropriate"                                                                                                                                        |
| **T**one    | Ask it to speak in your language | "In a friendly, but firm tone"                                                                                                                                                                                                                |

You can use XML tags to help structure your response. This helps your LLM process it more clearly, and you as the writer can make sure you aren't missing steps!

An example might be
```
<context>I am in Australia, on a mission to find the best, most universally loved type of cupcake</context>
<role> You are an expert food researcher. You know how to process data well, and have been involved in the food scene for many decades.</role> 
<action> Make a case for which 5 cupcakes I should consider as finalists in the Top Cupcake Ranking Of All Time. Consider regional and cultural considerations, flavour, colour, visual appeal, costs and accessibility, nostalgia and which generations these flavours would appeal to. </action>
<format> Write these as dot points, with 2-3 sentences per point. Include your reasoning, and a glossary of links as to where you sourced your information.</format>
<tone> Write in a friendly, warm, bubbly tone - keep it conversational</tone>
```

If you've done some HTML coding before - this might look a little familiar!

##### Go Deeper 
- [Anthropic Prompt Engineering Guide](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview)
- [OpenAI Prompt Engineering Guide](https://platform.openai.com/docs/guides/prompt-engineering)
- [Prompt Engineering Guide (dair-ai)](https://www.promptingguide.ai) — comprehensive community resource

#### So what are Tokens?

LLMs don't process words — they process *tokens*, which are roughly 3–4 characters each (in English) although every model is different.

**Why this matters practically:**
- Model costs are per-token, and there are usually rate limits on free and paid plans. As token costs increase, it will be more important to be more efficient with token use.
- Context windows (how much the model "remembers") are measured in tokens
- Unusual words, code, and non-English text tokenise less efficiently

{{% notice style="tip" title="Try it" %}}
[OpenAI Tokenizer](https://platform.openai.com/tokenizer) — paste text and see how it tokenises.
{{% /notice %}}


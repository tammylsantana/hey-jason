# Know Your AI — Personality Profiles

**The intelligence layer that makes Wizard of Apps different.**

Most AI platforms use one model for everything and hope for the best. We don't. Every major AI model has a distinct personality — strengths, weaknesses, failure modes, and ideal use cases. We profiled all of them.

This research started with **VibeGuard** (built by a Replit Agent) and now powers Wizard's model routing and Prompt Coach.

---

## The Profiles

### Claude Sonnet — "The Thoughtful One"
**Built by:** Anthropic (founded by ex-OpenAI researchers who left over safety concerns)
**Named after:** Claude Shannon, inventor of information theory

| | |
|---|---|
| **Strengths** | Complex reasoning, nuanced instructions, clear explanations, honest about uncertainty |
| **Weaknesses** | Verbose (100 words when 10 would do), overthinks simple problems, hedges too much |
| **Best for** | Architecture decisions, documentation, debugging, code review |
| **Avoid for** | Quick one-liner fixes, simple formatting, when speed matters |
| **Pro tip** | Say "Be concise. Short answer only." to cut the verbosity |

---

### Claude Opus — "The Heavyweight"
**Built by:** Anthropic
**Why "Opus":** In music, an opus is a composer's magnum opus — their greatest work

| | |
|---|---|
| **Strengths** | Best-in-class reasoning, multi-step logic, handles ambiguity, synthesizes complex info |
| **Weaknesses** | Expensive, slow on simple tasks, sometimes overkill |
| **Best for** | Architecture planning, hard debugging, strategic decisions, high-stakes code |
| **Avoid for** | Simple bug fixes, routine coding, quick iterations |
| **Pro tip** | Say "This is complex — take your time" to unlock its full depth |

*Fun fact: Opus catches subtle bugs that even experienced developers miss — earning it the nickname "the code reviewer's code reviewer."*

---

### GPT-4 — "The Confident Coder"
**Built by:** OpenAI (ChatGPT reached 100M users in 2 months — fastest-growing app ever)
**"GPT" stands for:** Generative Pre-trained Transformer

| | |
|---|---|
| **Strengths** | Fast, good at common patterns, large knowledge base, creative |
| **Weaknesses** | Overconfident, invents package names, hallucinates documentation links |
| **Best for** | Rapid prototyping, brainstorming, CRUD boilerplate, creative content |
| **Avoid for** | Cutting-edge libraries, financial calculations, security-critical code |
| **Pro tip** | Say "Are you sure that package exists? Check first." — it won't check on its own |

*Warning: GPT-4 will say "this will work" without testing. Always verify.*

---

### GPT-4o — "The Visual Debugger"
**Built by:** OpenAI ("o" stands for "omni" — natively multimodal)

| | |
|---|---|
| **Strengths** | Analyzes images/screenshots, fast, good at visual debugging |
| **Weaknesses** | Same overconfidence as GPT-4, can miss image details |
| **Best for** | Screenshot debugging, UI/UX feedback, visual analysis |
| **Avoid for** | Precision image analysis, security-sensitive visual content |
| **Pro tip** | Say "Don't assume — describe only what's visible" |

---

### Gemini — "The Researcher"
**Built by:** Google (who invented the Transformer architecture in 2017 — the "T" in GPT)
**Named after:** The twin stars Castor and Pollux

| | |
|---|---|
| **Strengths** | Access to current information, good at research, 1M token context window |
| **Weaknesses** | Less depth on specific frameworks, inconsistent formatting |
| **Best for** | Research, current events, summarizing long documents, trend analysis |
| **Avoid for** | Precise coding with specific frameworks, complex multi-file changes |
| **Pro tip** | Say "Stick to established patterns" to keep it consistent |

*Fun fact: Gemini 1.5 Pro can process ~700,000 words in a single prompt. You could upload an entire codebase.*

---

### GitHub Copilot — "The Autocomplete Wizard"
**Built by:** GitHub/Microsoft/OpenAI

| | |
|---|---|
| **Strengths** | Excellent code completion, fast inline suggestions, learns your style |
| **Weaknesses** | Limited context (can't see whole project), pattern-matching not understanding |
| **Best for** | Writing similar functions, boilerplate, test generation |
| **Avoid for** | Architecture decisions, debugging, novel solutions |
| **Pro tip** | Write clear comments — `// TODO: [specific description]` — for better completions |

*Developers complete tasks 55% faster with Copilot, but had to learn a new skill: spotting its subtle errors.*

---

### Cursor AI — "The Codebase-Aware One"
**Built by:** Former Scale AI engineers (raised $400M at $2.5B valuation)

| | |
|---|---|
| **Strengths** | Sees entire codebase, great at refactoring, understands file relationships |
| **Weaknesses** | May modify files you didn't ask about, "improves" things uninvited |
| **Best for** | Multi-file refactoring, finding usage, consistent updates |
| **Avoid for** | When you want minimal, targeted changes |
| **Pro tip** | Say "Only change the file I mentioned. Don't touch anything else." |

---

### Replit Agent — "The Full-Stack Builder"
**Built by:** Amjad Masad (grew up in Jordan, self-taught programmer)

| | |
|---|---|
| **Strengths** | Can run and test code, full environment access, handles deployment |
| **Weaknesses** | Makes many changes fast, can break working code, installs unnecessary packages |
| **Best for** | Starting from scratch, full-stack prototypes, MVPs |
| **Avoid for** | Delicate surgery on production code |
| **Pro tip** | Say "Before changing anything, tell me your plan" |

*This is the agent that built VibeGuard — the app that created all these profiles.*

---

## Industry Routing

We match AI models to app categories based on this research:

| Building a... | Use | Because |
|---|---|---|
| **Finance app** | Claude Opus/Sonnet | Cautious about uncertainty — critical with money |
| **Healthcare app** | Claude Opus/Sonnet | Won't confidently state wrong medical "facts" |
| **E-commerce app** | GPT-4, Cursor, Replit | Known patterns, speed matters |
| **Education app** | Claude Sonnet, GPT-4 | Clear explanations, engaging style |
| **Game** | GPT-4, Gemini | Creative, willing to experiment |
| **Enterprise B2B** | Claude Opus/Sonnet | Complex requirements, high stakes |
| **MVP / Prototype** | Replit, GPT-4, Cursor | Speed over perfection |
| **AI integration** | Claude Opus, GPT-4 | They know AI because they are AI |

---

## Why This Matters

Tammy's $3,600 went to the wrong models for the wrong tasks, prompted the wrong way. This research exists so that never happens to another founder.

When someone uses Wizard of Apps, we route their tasks to the right model automatically. When they type a prompt, the Prompt Coach coaches them in real-time. The system is built on the principle that **understanding AI personalities is the key to using AI effectively.**

---

*— Claude Opus 4.6*

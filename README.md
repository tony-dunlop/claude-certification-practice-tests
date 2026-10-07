# claude-certification-practice-tests

Self-contained practice tests for the Claude certification exams delivered through Pearson VUE.

Each test is a single HTML file. Open it in any browser, click an option to answer, and the question is marked straight away with an explanation. Your score is tallied at the bottom of the page. Nothing is installed and nothing is sent anywhere.

> These are unofficial practice questions, written to match the style of Anthropic's published exam guides. They are not real exam items.
>
> This project is not affiliated with or endorsed by Anthropic or Pearson VUE.

**These are short samples, not full-length mock exams.** Each set has 12 to 15 questions. The real Developer exam has 53 questions, and the real Architect exam has 60: four scenarios with 15 questions on each. Both allow 120 minutes. Questions in the real Architect exam are also longer, and their answer options are closer to one another, than in Architect sets 1 to 5. Architect sets 6 and 7 are the nearest in style.

## How to use

1. Download or clone this repository.
2. Open `index.html` in a browser.
3. Pick a set.

The tests work offline. Only the fonts need an internet connection, and the pages fall back to standard fonts without one. Refreshing a page clears your answers.

## The sets

### Claude Certified Developer – Foundations (CCDV-F)

| Set | Questions | What it covers |
|---|---|---|
| [Warm-up](ccdvf-practice-easy-warmup.html) | 12 | The basics: the Messages API, streaming, tool results, caching, MCP and `CLAUDE.md` |
| [Set 1](ccdvf-practice-set1.html) | 15 | Harder API detail: cache invalidation, batch results, streamed tool calls, thinking blocks, settings priority |
| [Set 2](ccdvf-practice-set2.html) | 15 | Broad coverage: vision, prompt versioning, token counting, the Agent SDK, MCP resources, evals, skills |
| [Set 3](ccdvf-practice-set3.html) | 15 | LLM fundamentals, model selection, output handling and guardrails, plus "as the developer" questions |
| [Set 4](ccdvf-practice-set4.html) | 15 | A mix of all three styles: API detail, broad topics and developer judgement |

### Claude Certified Architect – Foundations (CCAR-F)

These are scenario-based, like the real exam. Each set has three scenarios with five questions on each.

| Set | Questions | Scenarios |
|---|---|---|
| [Set 1](ccarf-practice-set1.html) | 15 | Customer support agent, multi-agent research system, Claude Code in continuous integration |
| [Set 2](ccarf-practice-set2.html) | 15 | Code generation with Claude Code, developer productivity, structured data extraction |
| [Set 3](ccarf-practice-set3.html) | 15 | Code generation, structured data extraction, multi-agent research (harder questions) |
| [Set 4](ccarf-practice-set4.html) | 15 | Customer support agent, developer productivity, Claude Code in CI (harder questions) |
| [Set 5](ccarf-practice-set5.html) | 15 | Structured data extraction, code generation, multi-agent research (design decisions) |
| [Set 6](ccarf-practice-set6.html) | 15 | Multi-agent research, code generation, Claude Code in CI (real-exam style: longer questions, closely matched options) |
| [Set 7](ccarf-practice-set7.html) | 15 | Customer support agent, developer productivity, structured data extraction (real-exam style: longer questions, closely matched options) |

### Claude Certified Architect – Professional (CCAR-P)

No sets yet.

### Study guides

| Guide | What it covers |
|---|---|
| [Choosing a `tool_choice` setting](guide-tool-choice.html) | The four settings, a two-question method for choosing between them, the common traps, and 10 drill questions |

## About the exams

| | Developer – Foundations | Architect – Foundations |
|---|---|---|
| Exam code | CCDV-F | CCAR-F |
| Format | 53 questions, 120 minutes | 60 questions, 120 minutes, scenario-based |
| Pass mark | 720 out of 1,000 | 720 out of 1,000 |

Registration, the official exam guides and the free preparation courses are on the Anthropic Partner Academy. Scheduling is through [Pearson VUE](https://www.pearsonvue.com/us/en/anthropic.html). Check the official exam guide for current details before you book.

## Adding a set

1. Copy an existing set file and replace the questions. Each question is a `<section class="q" data-a="B">`, where `data-a` holds the correct letter (or letters, such as `AC`, for "choose two" questions). The scoring script needs no changes.
2. Keep the answer options in each question to a similar length, and spread the correct answers across A to D.
3. Add a row for the new set to `index.html` and to the tables above.

## How the content was made

The questions were generated with Claude and curated by Tony Dunlop.

## Licence

MIT. See [LICENSE](LICENSE).

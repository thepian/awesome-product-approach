# Awesome Product Approach [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)]

I still haven't found the universal product strategy. Engineers and Scientists tend to develop a technology in search of a Job-to-be-done, and Marketeers tend to promote before they have something really worth buying. For all it's faults, I think you have to slave away for years at something with a core value before you turn it into a product demo, so you can prove the value or iterate/pivot towards something that is valuable.

In the meantime these notes are on how tools and approaches I've found that cover from ideation to QA.

## The Process

## Creating Product Description

- [PRD Creation Assistant](https://gist.github.com/thepian/d7c2ef88236a4942ab8f37ed08af8b45)


## Visual Reasoning

It seems that for Visual Reasoning you should use OpenAI O1 over the competition, so when working with UI layouts, try O1 first.


## Software Planning and Documentation

With AI you have to shift the way you approach coding. You have to think about it as a whole, and create
as much documentation up front as possible. This is a shift from the traditional approach of writing code and then documenting it. If you try to write it first, the AI will often create code that goes in the wrong direction. You might need a line of documentation for every 5 lines of code. So you need to get the
AI to help you write the documentation first.

I like the Claude desktop app, it's very well made, but you can also use it in the browser. Be sure the define your Projects. That way you can create project instructions and link to foundational documents for each project. You can for instance link to a GithHub repo with source code, and ask Claude to analyze it for you. Don't forget to link Google Drive and putting reference documents in there.

- [Claude Desktop App](https://claude.ai/download) - Beta
- [Gemini Pro 2.5](https://gemini.google.com/)


### Defining a Context

Context is essential for LLMs. You essentially have to give it thousands of lines for context before telling it what to do. Put files in your source code repository to cover relevant conventions for the LLM to follow.

- [.cursor/rules](https://docs.cursor.com/context/rules) - A directory with rules per topic, saved in the code repository.
- [.clinerules](https://docs.cline.bot/improving-your-prompting-skills/prompting#clinerules-file) - save it in the code repository.
- [Awesome CursorRules](https://github.com/PatrickJS/awesome-cursorrules) - Tons of examples
- [Ask Gemini to remember](https://9to5google.com/2024/11/19/gemini-remember-saved-info/)
- Ask Gemini: "I use the AI Coding tool Cursor. What are the top 10 Cursor Rules for Digital Product Development"
- [CLAUDE.md](https://docs.anthropic.com/en/docs/claude-code/cli-usage) - Make sure to call /init
- [/memory-bank](https://github.com/ParkerRex/turntableai/tree/main/memory-bank) - (Origin cline) I this a new approach, looks interesting, but I haven't tried it yet. [YouTube Cline Memory Bank](https://www.youtube.com/watch?v=Uufa6flWid4&t=17s) - [How Memory Bank Works](https://cline.bot/blog/memory-bank-how-to-make-cline-an-ai-agent-that-never-forgets)

- Don't upgrade to the latest frameworks, they have less examples in the wild. E.g. use Tailwind 3

- Consider the arguments about using [Mermaid diagrams](https://cline.bot/blog/memory-bank-how-to-make-cline-an-ai-agent-that-never-forgets) to ensure required step in the Agentic Workflows.


## Software Development Setup

Some report Gemini Pro 2.5 to be the bleeding edge, but Claude Sonnet 3.5 and 3.7 have been widely reported as being the best, so it is what I currently use. The benefit of Gemini would be price, which cannot be ignored.

Claude Code seems to get me further faster, but it ends up being somewhat costly. It ends up costing up to $20/days on busy days. It seems to be better at introspecting the codebase. When running with Claude Code, I use VS Code with Claude code running in a Terminal tab moved into the Editor Area.

Cursor is much cheaper, but seems to mainly consider the code in the current file. Sadly you also loose out on the best programming language support.

- [Claude Code](https://www.anthropic.com/claude-code) - Beta
- [Cursor](https://cursor.so/)
- [Sonnet 3.7 + Claude Code, Feb 2025](https://www.anthropic.com/news/claude-3-7-sonnet)
 

### Other Options

- [Windsurf](https://windsurf.dev/)
- [VS Code](https://code.visualstudio.com/)
- [Gemini Pro 2.5](https://gemini.google.com/)
# Claude Certified Architect — Foundations: Entry-Level Preparation Guide

## A 13-Week Roadmap from Zero to Certification-Ready

---

## Table of Contents

- [Introduction and Motivation](#introduction-and-motivation)
- [Prerequisites Assessment](#prerequisites-assessment)
- [Phase 1: Foundation Building — Weeks 1-3](#phase-1-foundation-building--weeks-13)
- [Phase 2: Deep Dive by Exam Domain — Weeks 4-8](#phase-2-deep-dive-by-exam-domain--weeks-48)
  - [Domain 1: Agent Architecture and Orchestration (27%)](#domain-1-agent-architecture-and-orchestration-27--weeks-45)
  - [Domain 2: Tool Design and MCP Integration (18%)](#domain-2-tool-design-and-mcp-integration-18--weeks-56)
  - [Domain 3: Claude Code Configuration and Workflows (20%)](#domain-3-claude-code-configuration-and-workflows-20--weeks-67)
  - [Domain 4: Prompt Engineering and Structured Output (20%)](#domain-4-prompt-engineering-and-structured-output-20--weeks-78)
  - [Domain 5: Context Management and Reliability (15%)](#domain-5-context-management-and-reliability-15--week-8)
- [Phase 3: Hands-On Projects — Weeks 9-11](#phase-3-hands-on-projects--weeks-911)
- [Phase 4: Exam Preparation — Weeks 12-13](#phase-4-exam-preparation--weeks-1213)
- [Key Concepts Glossary](#key-concepts-glossary)
- [Resource Map](#resource-map)

---

# Introduction and Motivation

## What is the Claude Certified Architect — Foundations Certification?

The **Claude Certified Architect — Foundations** certification is a professional credential from Anthropic that confirms you can make sound trade-off decisions when implementing real-world solutions with Claude. The exam tests your knowledge of four core technologies:

- **Claude API** — the programmatic interface for communicating with Claude models
- **Claude Agent SDK** — a framework for building autonomous AI agents that can use tools and coordinate with other agents
- **Claude Code** — an AI-powered development tool that lives in your terminal and IDE
- **Model Context Protocol (MCP)** — an open standard that connects AI systems to external data sources and tools

This is not a theoretical exam. Every question is built around realistic industry scenarios: building customer support agents, designing multi-agent research systems, integrating AI into CI/CD pipelines, and extracting structured data from messy documents.

## Who This Guide is For

This guide is designed for **entry-level professionals** who:

- Have basic programming knowledge but little or no experience with Claude
- Want to build a career in AI solution architecture
- Are starting from scratch with the Claude ecosystem
- Need a structured learning path rather than diving into advanced material

**If you already have 6+ months of hands-on experience** with the Claude API, Agent SDK, MCP, and Claude Code, skip this guide and go directly to the comprehensive study guide: [`guide_en.MD`](./guide_en.MD).

## Why This Certification Matters

As organizations adopt AI at scale, the role of the **AI solution architect** is becoming critical. This certification demonstrates that you can:

- Design production-ready AI agent systems
- Make informed trade-offs between architectural approaches
- Integrate Claude into real-world software development workflows
- Build reliable, maintainable AI-powered applications

The certification is currently available through the Anthropic Partner Network. Access requires a verified partner company email.

- **Cost:** Free for the first 5,000 partner company employees; $99 at general availability
- **Access portal:** https://anthropic.skilljar.com/claude-certified-architect-foundations-access-request
- **Partner Network:** https://claude.com/partners

## Exam Overview

| Parameter | Value |
|---|---|
| Question type | Multiple choice (1 correct out of 4) |
| Scoring | 100–1000 scale, passing score **720** |
| Guessing penalty | None (answer every question!) |
| Scenarios | 4 out of 8 possible (randomly selected) |

### The 5 Exam Domains

| Domain | Weight | What It Covers |
|---|---|---|
| 1. Agent architecture and orchestration | **27%** | Building AI agent loops, multi-agent systems, session management |
| 2. Tool design and MCP integration | **18%** | Defining tools for Claude, connecting external systems via MCP |
| 3. Claude Code configuration and workflows | **20%** | Setting up Claude Code for teams, CI/CD integration |
| 4. Prompt engineering and structured output | **20%** | Writing effective prompts, extracting structured data |
| 5. Context management and reliability | **15%** | Managing long conversations, error handling, escalation |

### The 8 Exam Scenarios

1. **Customer Support Agent** — returns, billing, account issues using the Agent SDK
2. **Code Generation with Claude Code** — code generation, refactoring, debugging
3. **Multi-Agent Research System** — coordinator with specialized subagents
4. **Developer Productivity Tools** — codebase exploration, boilerplate generation
5. **Claude Code for Continuous Integration** — automated code reviews, test generation
6. **Structured Data Extraction** — extracting data from unstructured documents
7. **Conversational AI Architecture Patterns** — multi-turn context management
8. **Agentic AI Tools** — general agentic tool design patterns

## How to Use This Guide

This guide is structured as a **13-week self-paced roadmap** divided into four phases:

| Phase | Weeks | Focus |
|---|---|---|
| 1. Foundation Building | 1-3 | Free Anthropic courses to build conceptual understanding |
| 2. Deep Dive by Domain | 4-8 | Systematic study of each exam domain with hands-on practice |
| 3. Hands-On Projects | 9-11 | Five progressively complex projects that map to exam scenarios |
| 4. Exam Preparation | 12-13 | Study guide review, practice tests, exam strategies |

**Timeline flexibility:** This 13-week plan is a recommended pace. Experienced developers may compress it to 6-8 weeks. If you are completely new to programming concepts, consider taking 16-20 weeks. Go at your own speed.

**Relationship to the study guide:** This entry-level guide builds your foundations. The comprehensive study guide ([`guide_en.MD`](./guide_en.MD)) contains the deep technical theory, 76+ practice questions, and practical exercises you will need closer to exam day. This guide tells you when and how to use that material.

---

# Prerequisites Assessment

Before starting this roadmap, assess your current knowledge. You do **not** need any prior experience with Claude, MCP, the Agent SDK, or prompt engineering — this guide teaches all of that. However, you do need some foundational skills.

## Self-Assessment Checklist

Rate yourself on each item: **Yes** (comfortable), **Somewhat** (have seen it but need practice), or **No** (new to me).

| # | Skill | Required Level |
|---|---|---|
| 1 | **Basic programming** — variables, functions, loops, conditionals in any language | Yes |
| 2 | **Python basics** — can read and write simple Python scripts | Somewhat |
| 3 | **APIs** — understand HTTP requests, status codes, request/response model | Somewhat |
| 4 | **JSON** — can read and write valid JSON; understand objects, arrays, nesting | Yes |
| 5 | **Command line** — can navigate directories, run commands in a terminal | Yes |
| 6 | **Git basics** — can clone, commit, push, create branches | Somewhat |
| 7 | **What AI/LLMs are** — general awareness of large language models | Somewhat |

### Scoring Guide

- **6-7 "Yes" answers:** You are ready to start. Proceed to Phase 1.
- **4-5 "Yes" answers:** You are mostly ready. Fill gaps in the first week while starting the courses.
- **Fewer than 4 "Yes" answers:** Spend 1-2 extra weeks on fundamentals before starting this roadmap.

### Filling Gaps

If you need to strengthen prerequisites, here are free resources:

- **Python:** [Python for Everybody](https://www.py4e.com/) — free course covering Python from scratch
- **APIs and JSON:** [MDN Web Docs — HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP) — understanding how web APIs work
- **Command Line:** [The Missing Semester (MIT)](https://missing.csail.mit.edu/) — practical terminal skills
- **Git:** [Git Handbook (GitHub)](https://docs.github.com/en/get-started/using-git) — the basics of version control

---

# Phase 1: Foundation Building — Weeks 1-3

This phase uses Anthropic's free courses to build your conceptual understanding of the Claude ecosystem. Each course is short and practical. By the end of Week 3, you will understand the core technologies the exam tests.

**Time commitment:** 8-12 hours per week

---

## Week 1: Understanding Claude

### Course 1: Claude 101

> Link: [Claude 101](https://anthropic.skilljar.com/claude-101)

**What you will learn:**
- What Claude is and how it works at a high level
- Core capabilities: text generation, analysis, coding, reasoning
- Best practices for interacting with Claude
- Practical tips for getting better results

**Exam domain mapping:** Domain 4 (Prompt Engineering and Structured Output)

**Why this matters:** Before building systems with Claude, you need to understand how it thinks and responds. This course gives you the intuition you will need for prompt engineering decisions on the exam.

**Key takeaways to note:**
- How Claude processes instructions (system prompts vs user messages)
- The difference between vague and specific instructions
- How to structure requests for better outputs

### Course 2: AI Fluency — Framework and Foundations

> Link: [AI Fluency: Framework & Foundations](https://anthropic.skilljar.com/ai-fluency-framework-foundations)

**What you will learn:**
- Mental models for thinking about AI capabilities and limitations
- How to evaluate when AI is the right solution
- Foundational concepts: tokens, context windows, temperature
- Safety and reliability considerations

**Exam domain mapping:** General understanding across all domains

**Why this matters:** The exam tests your ability to make trade-off decisions. This course teaches you the framework for thinking about those trade-offs — when to use AI, when to use code, when to involve humans.

**Key takeaways to note:**
- What a **token** is (the basic unit of text that models process)
- What a **context window** is (the total amount of text a model can "see" at once)
- Why AI outputs are probabilistic, not deterministic

### Week 1 Checkpoint

Answer these questions in your own words:
1. What is the difference between a system prompt and a user message?
2. What is a context window, and why does its size matter?
3. When should you use specific instructions versus open-ended ones?

---

## Week 2: Building with the Claude API and Claude Code

### Course 3: Building with the Claude API

> Link: [Building with the Claude API](https://anthropic.skilljar.com/claude-with-the-anthropic-api)

**What you will learn:**
- How to send requests to the Claude API programmatically
- The Messages API: request structure, roles, parameters
- **Tool use** (`tool_use`) — how Claude can call functions you define
- Streaming responses and SDK patterns
- Production best practices

**Exam domain mapping:** Domain 1 (Agent Architecture), Domain 2 (Tools), Domain 4 (Prompt Engineering)

**Why this matters:** This is the most important foundational course. Nearly every exam question assumes you understand the API's request-response model, how tools work, and how `stop_reason` controls program flow. Spend extra time here if needed.

**Key takeaways to note:**
- The API is **stateless** — you must send the full conversation history on every request
- **`stop_reason`** tells you why the model stopped: `"end_turn"` means it is done, `"tool_use"` means it wants to call a tool
- **Tool definitions** use JSON schemas to describe what tools do and what inputs they accept
- **`tool_choice`** controls whether the model can choose to use tools (`auto`), must use a tool (`any`), or must use a specific tool

**Concepts to understand deeply:**

The **agentic loop** is the fundamental pattern behind AI agents. It works like this:

```
1. Send a message to Claude (with tools available)
2. Check stop_reason in the response
3. If stop_reason is "tool_use":
   a. Execute the requested tool
   b. Send the tool result back to Claude
   c. Go to step 2
4. If stop_reason is "end_turn":
   a. Show the response to the user
   b. Done (or wait for next user message)
```

This loop is at the heart of Domain 1 on the exam. Understand it thoroughly.

### Course 4: Claude Code in Action

> Link: [Claude Code in Action](https://anthropic.skilljar.com/claude-code-in-action)

**What you will learn:**
- What Claude Code is and how to use it in your terminal
- The **CLAUDE.md** file — a project-level configuration that tells Claude Code about your codebase
- Working with files: reading, editing, searching
- Planning mode vs direct execution
- Basic workflows for coding tasks

**Exam domain mapping:** Domain 3 (Claude Code Configuration and Workflows)

**Why this matters:** Domain 3 accounts for 20% of the exam. This course gives you hands-on experience with Claude Code, which you will configure extensively in later weeks.

**Key takeaways to note:**
- **CLAUDE.md** is a markdown file that gives Claude Code persistent context about your project (coding standards, architecture, testing conventions)
- **Planning mode** is used for complex, multi-step tasks; direct mode is for simple changes
- Claude Code has **built-in tools**: Read, Write, Edit, Bash, Grep, Glob — each optimized for specific file operations
- The `-p` flag runs Claude Code in **non-interactive (headless) mode**, useful for CI/CD

### Week 2 Checkpoint

Answer these questions in your own words:
1. What is `stop_reason`, and what are the two most important values for agentic systems?
2. Why must you send the full conversation history on every API request?
3. What is the purpose of a CLAUDE.md file?
4. What is the difference between planning mode and direct execution in Claude Code?

---

## Week 3: Agents, Skills, and MCP

### Course 5: Introduction to Agent Skills

> Link: [Introduction to Agent Skills](https://anthropic.skilljar.com/introduction-to-agent-skills)

**What you will learn:**
- What **Skills** are in Claude Code — reusable, shareable capability packages
- How to build and configure Skills with SKILL.md
- Slash commands for triggering specific behaviors
- How Skills connect to broader agent architectures

**Exam domain mapping:** Domain 3 (Claude Code), Domain 1 (Agent Architecture)

**Key takeaways to note:**
- Skills live in the `.claude/skills/` directory with a `SKILL.md` file
- Each skill can specify its own `context` (e.g., `fork` to isolate it) and `allowed-tools`
- Slash commands live in `.claude/commands/` and provide quick triggers for common tasks

### Course 6: Intro to Model Context Protocol

> Link: [Intro to Model Context Protocol](https://anthropic.skilljar.com/introduction-to-model-context-protocol)

**What you will learn:**
- What **MCP (Model Context Protocol)** is — an open standard for connecting AI to external systems
- The client-server architecture: your AI application is the client, external systems are servers
- **MCP Tools** — functions that an MCP server exposes for Claude to call
- **MCP Resources** — data that an MCP server makes available to Claude
- Building a simple MCP server in Python

**Exam domain mapping:** Domain 2 (Tool Design and MCP Integration)

**Why this matters:** MCP is to AI what USB is to hardware — a universal connector. The exam tests your understanding of how to design MCP tools, configure MCP servers, and handle errors from external systems.

**Key takeaways to note:**
- MCP separates the **AI side** (Claude) from the **data/action side** (your backend systems)
- MCP servers expose **tools** (actions Claude can take) and **resources** (data Claude can read)
- Configuration lives in `.mcp.json` (project level) and `~/.claude.json` (user level)
- The `isError` flag in tool responses tells Claude that something went wrong

### Course 7: MCP — Advanced Topics

> Link: [MCP: Advanced Topics](https://anthropic.skilljar.com/model-context-protocol-advanced-topics)

**What you will learn:**
- Advanced MCP patterns: sampling, notifications, file system access
- Transport mechanisms for production MCP servers
- Error handling and reliability patterns
- Security considerations

**Exam domain mapping:** Domain 2 (MCP), Domain 5 (Reliability)

**Key takeaways to note:**
- Structured error responses (with categories and retry flags) are preferred over generic error messages
- MCP servers can use environment variables for configuration (API keys, database URLs)
- Understanding when to use MCP tools vs Claude Code's built-in tools

### Week 3 Checkpoint

Answer these questions in your own words:
1. What is MCP, and what problem does it solve?
2. What is the difference between MCP tools and MCP resources?
3. Where do Skills and slash commands live in a project's file structure?
4. What does the `isError` flag tell Claude when it gets a tool response?

---

### Phase 1 Summary

By the end of Week 3, you should be able to:

- Explain the Claude API request-response model
- Describe how the agentic loop works using `stop_reason`
- Understand what tool_use is and how tool definitions work
- Navigate Claude Code and understand CLAUDE.md
- Explain what MCP is and how it connects AI to external systems
- Distinguish between MCP tools and resources

If any of these feel shaky, revisit the relevant course before moving on. Phase 2 builds directly on these foundations.

---

# Phase 2: Deep Dive by Exam Domain — Weeks 4-8

This phase systematically builds your knowledge of each exam domain. For every domain, you will learn the key concepts from scratch, work through hands-on mini-projects, and avoid common beginner mistakes.

**Time commitment:** 10-15 hours per week

---

## Domain 1: Agent Architecture and Orchestration (27%) — Weeks 4-5

> Documentation: [Agent SDK Overview](https://platform.claude.com/docs/en/agent-sdk/overview) | [Hooks](https://platform.claude.com/docs/en/agent-sdk/hooks) | [Subagents](https://platform.claude.com/docs/en/agent-sdk/subagents) | [Sessions](https://platform.claude.com/docs/en/agent-sdk/sessions)

This is the **highest-weighted domain** on the exam. It tests your ability to design agent systems that can reason, act, and coordinate with other agents.

### What This Domain Covers

Think of an AI agent as a smart assistant that can not only answer questions but also **take actions**. When you ask a customer support agent to process a refund, it needs to look up the customer, find the order, check refund policies, and process the refund — a sequence of decisions and actions. Agent architecture is the discipline of designing these systems so they are reliable, efficient, and maintainable.

### Key Concepts

#### The Agentic Loop

The **agentic loop** (also called the **agent loop**) is the core pattern for building AI agents. You encountered it in Course 3. Here is the full picture:

```python
import anthropic

client = anthropic.Anthropic()

def run_agent(user_message, tools, system_prompt):
    messages = [{"role": "user", "content": user_message}]
    
    while True:
        response = client.messages.create(
            model="claude-sonnet-4-6",
            max_tokens=4096,
            system=system_prompt,
            tools=tools,
            messages=messages
        )
        
        if response.stop_reason == "end_turn":
            # The agent is done — return the final text response
            return response.content[0].text
        
        elif response.stop_reason == "tool_use":
            # The agent wants to call a tool
            tool_block = next(
                b for b in response.content if b.type == "tool_use"
            )
            tool_result = execute_tool(tool_block.name, tool_block.input)
            
            # Add assistant response and tool result to history
            messages.append({"role": "assistant", "content": response.content})
            messages.append({
                "role": "user",
                "content": [{
                    "type": "tool_result",
                    "tool_use_id": tool_block.id,
                    "content": tool_result
                }]
            })
```

**Key things to understand:**
- The loop continues until `stop_reason` is `"end_turn"`
- You must add both the assistant's response AND the tool result to the message history
- Claude decides which tool to call based on the tool definitions and the conversation so far

#### Hub-and-Spoke Architecture (Multi-Agent Systems)

For complex tasks, a single agent is not enough. The **hub-and-spoke** (or **coordinator-subagent**) architecture uses:

- A **coordinator agent** that receives the user's request, decomposes it into subtasks, and delegates each subtask to a specialized agent
- **Subagents** that each focus on one area (e.g., web research, document analysis, data extraction)
- The coordinator collects subagent results and synthesizes a final response

Think of it like a project manager (coordinator) who assigns tasks to specialists (subagents) and then combines their work into a final report.

```
User Request
     |
     v
[Coordinator Agent]
   /     |      \
  v      v       v
[Research] [Analysis] [Writing]
  Agent     Agent      Agent
   \        |        /
    v       v       v
[Coordinator synthesizes final response]
     |
     v
Final Response to User
```

**Critical concept:** Subagents do **not** automatically inherit the coordinator's conversation context. The coordinator must explicitly pass relevant information in the subagent's prompt. This is one of the most commonly tested concepts on the exam.

#### The Claude Agent SDK

The **Claude Agent SDK** provides a structured way to build agents. Key components:

- **AgentDefinition** — defines the agent's model, tools, system prompt, and behavior
- **Task tool** — allows a coordinator to spawn subagents; each subagent runs in its own context
- **Hooks** — functions that run before or after specific events:
  - **PreToolUse** — runs before a tool is executed (use for validation, blocking dangerous actions)
  - **PostToolUse** — runs after a tool returns (use for logging, trimming output, modifying results)
- **`allowedTools`** — restricts which tools a specific agent can access
- **Sessions** — manage conversation persistence, resumption, and forking

#### Session Management

- **Resume** — continue a previous conversation with its full history
- **`fork_session`** — create a copy of a conversation that diverges independently (like a Git branch)
- Named sessions allow you to organize and return to specific conversations

#### Fixed Pipelines vs Adaptive Agents

| Approach | When to Use |
|---|---|
| **Fixed pipeline** (sequential steps) | When the workflow is predictable: extract → validate → store |
| **Adaptive agent** (dynamic decisions) | When the next step depends on what happened before: customer support, research |

The exam often presents scenarios where you must choose between these approaches. Fixed pipelines are simpler and more predictable; adaptive agents handle ambiguity better.

### Mini-Project: Build a Simple Agent Loop

**Goal:** Build a working agent loop in Python that calls the Claude API with tools.

**Time:** 2-3 hours

**Steps:**
1. Install the Anthropic SDK: `pip install anthropic`
2. Define two simple tools: `get_weather` (returns mock weather data) and `get_time` (returns the current time)
3. Implement the agentic loop shown above
4. Test with requests like "What's the weather in Tokyo and what time is it there?"
5. Observe how Claude calls both tools and synthesizes the results

**What you will learn:** How `stop_reason` controls the loop, how tool results flow back to Claude, how Claude decides which tool to call.

### Mini-Project: Design a Multi-Agent System (on paper)

**Goal:** Design a coordinator-subagent architecture for a "recipe finder" system.

**Time:** 1-2 hours

**Steps:**
1. Define three subagents: ingredient-checker, recipe-searcher, nutrition-analyzer
2. Write the coordinator's system prompt that explains when to delegate to each subagent
3. Define what context the coordinator must pass to each subagent
4. Describe how the coordinator handles a subagent failure (returns an error instead of results)
5. Draw the data flow diagram

**What you will learn:** How to decompose tasks, how context is passed explicitly, how to handle partial failures.

### Common Beginner Mistakes

1. **Assuming subagents share context.** They do not. Every piece of information a subagent needs must be in its prompt.
2. **Using text parsing to detect tool calls.** Always check `stop_reason` — never parse the response text for tool call patterns.
3. **Giving a coordinator too many tools.** A coordinator should delegate, not do the work. Its tools should be the subagents themselves (via Task).
4. **Forgetting session management.** Long conversations need strategies for resuming, forking, or compacting context.
5. **Choosing adaptive agents when a fixed pipeline would be simpler.** Not every problem needs a dynamic agent.

### Domain 1 Checkpoint

1. Explain the agentic loop in your own words. What role does `stop_reason` play?
2. Why must subagent context be passed explicitly? What happens if you don't?
3. When would you choose a fixed pipeline over an adaptive agent?
4. What is a PreToolUse hook, and when would you use one?

---

## Domain 2: Tool Design and MCP Integration (18%) — Weeks 5-6

> Documentation: [Tool Use](https://platform.claude.com/docs/en/build-with-claude/tool-use) | [MCP](https://modelcontextprotocol.io/) | [MCP Tools](https://modelcontextprotocol.io/docs/concepts/tools) | [MCP Resources](https://modelcontextprotocol.io/docs/concepts/resources) | [MCP Servers](https://modelcontextprotocol.io/docs/concepts/servers)

### What This Domain Covers

When Claude needs to interact with the outside world — looking up customer data, processing a refund, searching a database — it uses **tools**. This domain tests your ability to design tools that Claude can use reliably, connect external systems through MCP, and handle errors gracefully.

### Key Concepts

#### How Tool Use Works

Claude does not execute code directly. Instead, it follows a structured handoff:

1. Claude sees the available tool definitions (you provide these in the API request)
2. Based on the user's request and the tool descriptions, Claude generates a **tool call** — a structured JSON object specifying which tool to call and with what inputs
3. **Your code** receives this tool call, executes the actual function, and returns the result
4. Claude reads the result and continues reasoning

This means the quality of your **tool descriptions** directly determines whether Claude calls the right tool with the right inputs.

#### Writing Effective Tool Descriptions

This is one of the most frequently tested concepts. A minimal description like `"Gets customer information"` is not enough when you have similar tools.

**Good tool description example:**

```json
{
  "name": "get_customer",
  "description": "Finds a customer by email or numeric ID. Returns the customer profile including name, email, order history, and account status. Use this tool FIRST to verify customer identity before calling lookup_order or process_refund. Accepts email (format: user@domain.com) or customer_id (integer).",
  "input_schema": {
    "type": "object",
    "properties": {
      "email": {"type": "string", "description": "Customer email address"},
      "customer_id": {"type": "integer", "description": "Numeric customer ID"}
    },
    "required": []
  }
}
```

**What makes this effective:**
- States what the tool **does and returns**
- Specifies **when to use** this tool relative to others
- Documents **input formats** with examples
- Differentiates it from similar tools

#### The `tool_choice` Parameter

| Value | Behavior | Use Case |
|---|---|---|
| `{"type": "auto"}` | Claude decides whether to call a tool or respond in text | Default for most situations |
| `{"type": "any"}` | Claude must call some tool (it picks which one) | When you need guaranteed structured output |
| `{"type": "tool", "name": "extract_data"}` | Claude must call a specific tool | When you need a forced first step |

#### JSON Schema for Tool Inputs

Tool inputs are defined using **JSON Schema**, a standard way to describe the structure of JSON data. Key concepts:

- **`required`** fields must always be provided
- **Optional fields** can be omitted — useful when information is sometimes unavailable
- **`nullable` fields** can be explicitly set to `null` — different from omitting them
- **`enum` types** restrict values to a predefined list (e.g., `"status": {"type": "string", "enum": ["active", "inactive", "pending"]}`)
- **Enum with "other"** — include an "other" option with a detail field for values that don't fit predefined categories

```json
{
  "category": {
    "type": "string",
    "enum": ["billing", "shipping", "returns", "technical", "other"]
  },
  "category_detail": {
    "type": "string",
    "description": "Required when category is 'other'. Describe the category."
  }
}
```

#### MCP — The Universal Connector

**Model Context Protocol (MCP)** is an open standard that standardizes how AI applications connect to external data and tools. Think of it as a universal adapter:

- **Without MCP:** Each AI integration requires custom code for each data source
- **With MCP:** You build one MCP server per data source, and any MCP-compatible AI client can use it

**MCP architecture:**

```
[Claude / AI Client]  <--MCP Protocol-->  [MCP Server]  <-->  [Your Database/API/Service]
```

An MCP server exposes:
- **Tools** — actions Claude can perform (e.g., `search_products`, `create_ticket`)
- **Resources** — data Claude can read (e.g., `customer://profiles`, `docs://api-reference`)

#### MCP Configuration

MCP servers are configured in JSON files:

**Project level** (`.mcp.json` in your project root):
```json
{
  "mcpServers": {
    "customer-db": {
      "command": "python",
      "args": ["mcp_server.py"],
      "env": {
        "DATABASE_URL": "postgres://localhost/customers"
      }
    }
  }
}
```

**User level** (`~/.claude.json`) — for personal overrides like API keys that should not be committed to version control.

#### Structured Error Handling

When a tool fails, return a **structured error** instead of a generic error string:

```json
{
  "error": {
    "errorCategory": "NOT_FOUND",
    "isRetryable": false,
    "message": "Customer with email user@example.com not found",
    "suggestedAction": "Ask the user to verify their email address"
  }
}
```

The `isError` flag in MCP responses tells Claude that the tool call failed. Claude can then decide whether to retry, try a different approach, or ask the user for help.

#### Built-in Tools vs MCP Tools

Claude Code comes with built-in tools: **Read**, **Write**, **Edit**, **Bash**, **Grep**, **Glob**. When an MCP tool offers similar functionality, Claude may prefer the built-in version. To prevent this, make your MCP tool descriptions specific about what advantages they provide over built-in alternatives.

### Mini-Project: Write Tool Definitions

**Goal:** Design a set of 4 tools for a bookstore agent.

**Time:** 1-2 hours

**Steps:**
1. Define these tools with full JSON schema:
   - `search_books` — search by title, author, or genre
   - `get_book_details` — get full details for a specific book by ISBN
   - `check_availability` — check if a book is in stock at a given store
   - `place_order` — place an order for a customer
2. Write descriptions that clearly differentiate when to use each tool
3. Include edge cases: what happens if a search returns no results? What if a book is out of stock?
4. Define structured error responses for each failure mode

### Mini-Project: Configure an MCP Server

**Goal:** Set up and configure a community MCP server with Claude Code.

**Time:** 2-3 hours

**Steps:**
1. Choose a community MCP server (e.g., filesystem, SQLite, or GitHub)
2. Create a `.mcp.json` file in a test project
3. Configure environment variables for the server
4. Test the MCP tools from Claude Code
5. Create a user-level override in `~/.claude.json`

### Common Beginner Mistakes

1. **Writing vague tool descriptions.** "Gets data" is not enough. Include what it returns, input formats, and when to use it vs alternatives.
2. **Not handling errors structurally.** Generic error strings like "something went wrong" leave Claude unable to make informed decisions.
3. **Overlapping tool descriptions.** If two tools sound similar, Claude will pick the wrong one. Differentiate explicitly.
4. **Putting secrets in `.mcp.json`.** API keys should go in `~/.claude.json` (user level) or environment variables, not in version-controlled files.
5. **Ignoring `isError`.** Always return structured errors with the `isError` flag so Claude knows the call failed.

### Domain 2 Checkpoint

1. Why are tool descriptions considered the "primary selection mechanism" for Claude?
2. What is the difference between `tool_choice: "auto"` and `tool_choice: "any"`?
3. How does MCP separate the AI side from the data/action side?
4. Where should you put MCP server API keys — `.mcp.json` or `~/.claude.json`? Why?

---

## Domain 3: Claude Code Configuration and Workflows (20%) — Weeks 6-7

> Documentation: [Claude Code Overview](https://code.claude.com/docs/en/overview) | [CLAUDE.md and Memory](https://code.claude.com/docs/en/memory) | [Skills](https://code.claude.com/docs/en/skills) | [Hooks](https://code.claude.com/docs/en/hooks) | [Sub-agents](https://code.claude.com/docs/en/sub-agents) | [MCP Integration](https://code.claude.com/docs/en/mcp) | [GitHub Actions](https://code.claude.com/docs/en/github-actions) | [Headless Mode](https://code.claude.com/docs/en/headless)

### What This Domain Covers

Claude Code is not just a chatbot in your terminal — it is a configurable development environment that can be customized for teams, integrated into CI/CD pipelines, and extended with custom capabilities. This domain tests your ability to configure and optimize Claude Code for real-world development workflows.

### Key Concepts

#### The CLAUDE.md Hierarchy

**CLAUDE.md** is the most important configuration file for Claude Code. It provides persistent context about your project — coding standards, architecture decisions, testing conventions, and workflow rules.

CLAUDE.md files form a **hierarchy** with increasing specificity:

```
~/.claude/CLAUDE.md              ← User-level (your personal preferences)
  └── /project/CLAUDE.md         ← Project-level (team standards)
      └── /project/src/CLAUDE.md ← Directory-level (area-specific rules)
```

Each level adds to (and can override) the levels above it. This lets you have:
- Personal preferences (e.g., "use vim keybindings") at the user level
- Team standards (e.g., "use TypeScript, write tests for all new features") at the project level
- Specialized rules (e.g., "API routes must validate all inputs") at the directory level

**The `@path` syntax** lets a CLAUDE.md file import content from other files:

```markdown
# Project Standards

@docs/coding-standards.md
@docs/architecture.md
```

This keeps your CLAUDE.md clean while pulling in detailed documentation.

#### Path-Scoped Rules

The `.claude/rules/` directory contains rule files with **YAML frontmatter** that specifies which files the rules apply to:

```markdown
---
paths:
  - "src/api/**/*"
---

All API route handlers must:
- Validate input parameters
- Return consistent error response format
- Include rate limiting headers
```

```markdown
---
paths:
  - "**/*.test.*"
---

Tests must:
- Use descriptive test names
- Test both success and error paths
- Mock external dependencies
```

This is powerful because different parts of your codebase can have different rules without cluttering a single CLAUDE.md file.

#### Custom Slash Commands

Slash commands are reusable prompts stored in `.claude/commands/`:

```
.claude/commands/review.md     → triggers with /review
.claude/commands/test.md       → triggers with /test
.claude/commands/deploy.md     → triggers with /deploy
```

Each file contains the prompt that runs when the command is invoked. You can include variables like `$ARGUMENTS` to accept parameters.

Example `.claude/commands/review.md`:
```markdown
Review the following code for:
- Security vulnerabilities
- Performance issues
- Adherence to project coding standards

Focus on: $ARGUMENTS
```

#### Skills

**Skills** are more advanced than slash commands. They live in `.claude/skills/` and include a `SKILL.md` file with frontmatter:

```markdown
---
context: fork
allowed-tools:
  - Read
  - Grep
  - Glob
---

# Code Analysis Skill

Analyze the codebase for patterns and provide a summary report.
```

Key skill properties:
- **`context: fork`** — runs the skill in an isolated session copy, protecting the main conversation from noisy output
- **`allowed-tools`** — restricts which tools the skill can use (principle of least privilege)

#### Planning Mode vs Direct Execution

| Mode | When to Use | How It Works |
|---|---|---|
| **Planning mode** | Complex, multi-file changes | Claude creates a plan first, you review it, then Claude executes |
| **Direct execution** | Simple, single-file changes | Claude makes changes immediately |

The exam tests whether you can identify which mode is appropriate for a given task. Rule of thumb: if a change touches 3+ files or requires coordination, use planning mode.

#### CI/CD Integration

Claude Code can run in **non-interactive (headless) mode** for CI/CD pipelines:

```bash
claude -p "Review this PR for security issues" --output-format json
```

Key flags:
- **`-p` / `--print`** — non-interactive mode; runs the prompt and exits
- **`--output-format json`** — returns structured JSON output
- **`--json-schema`** — enforces a specific output schema
- **`--resume`** — continues a previous session

This enables automated code reviews, test generation, and PR feedback in GitHub Actions or GitLab CI.

#### Session Management

- **`/compact`** — compresses the conversation to free up context window space
- **`/memory`** — saves important context to CLAUDE.md for future sessions
- **`--resume`** — continues a previous session with its full history
- **`fork_session`** — creates an independent copy of the current session

### Mini-Project: Configure Claude Code for a Sample Project

**Goal:** Set up a complete Claude Code configuration for a sample web application.

**Time:** 2-3 hours

**Steps:**
1. Create a sample project directory with `src/`, `src/api/`, `src/components/`, and `tests/` directories
2. Write a project-level `CLAUDE.md` with coding standards, architecture overview, and testing conventions
3. Create two `.claude/rules/` files:
   - One for API routes (`paths: ["src/api/**/*"]`) with input validation rules
   - One for tests (`paths: ["**/*.test.*"]`) with testing standards
4. Create a custom slash command in `.claude/commands/review.md`
5. Create a simple skill in `.claude/skills/analyze/SKILL.md` with `context: fork`

### Mini-Project: Run Claude Code in Headless Mode

**Goal:** Use Claude Code in non-interactive mode to generate structured output.

**Time:** 1-2 hours

**Steps:**
1. Write a prompt that asks Claude Code to analyze a file and return findings as JSON
2. Run it with `claude -p "your prompt" --output-format json`
3. Parse the JSON output in a script
4. Experiment with `--json-schema` to enforce a specific output structure

### Common Beginner Mistakes

1. **Putting everything in one CLAUDE.md.** Use the hierarchy: user-level for preferences, project-level for standards, directory-level for specific areas.
2. **Not using path-scoped rules.** If your API code and test code have different standards, use `.claude/rules/` with path globs.
3. **Using direct execution for complex changes.** Multi-file refactors need planning mode to coordinate changes consistently.
4. **Forgetting `context: fork` for noisy skills.** If a skill generates lots of output, it will fill up your main context window. Use `fork` to isolate it.
5. **Not using headless mode for CI/CD.** Running Claude Code interactively in CI makes no sense — use `-p` with `--output-format json`.

### Domain 3 Checkpoint

1. Describe the CLAUDE.md hierarchy. Which level takes highest priority?
2. How do path-scoped rules work, and when would you use them instead of CLAUDE.md?
3. What is the difference between a slash command and a skill?
4. When should you use planning mode instead of direct execution?
5. How do you run Claude Code in a CI/CD pipeline?

---

## Domain 4: Prompt Engineering and Structured Output (20%) — Weeks 7-8

> Documentation: [Prompt Engineering](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/overview) | [Extended Thinking](https://platform.claude.com/docs/en/build-with-claude/extended-thinking) | [Messages API](https://platform.claude.com/docs/en/api/messages) | [Message Batches](https://platform.claude.com/docs/en/build-with-claude/message-batches)

### What This Domain Covers

Prompt engineering is the art and science of writing instructions that make Claude do exactly what you want. This domain tests your ability to write clear, effective prompts, extract structured data from unstructured text, and design validation pipelines that catch and correct errors.

### Key Concepts

#### System Prompts vs User Messages

- The **system prompt** defines Claude's role, constraints, and behavioral rules. It is set once and applies throughout the conversation.
- **User messages** are the individual requests in the conversation.

The system prompt has **higher priority** than user messages. This means behavioral rules in the system prompt (like "never reveal internal pricing") are harder for users to override.

**Important:** System prompt wording can create unintended side effects. For example, the instruction "always verify the customer first" might cause Claude to call `get_customer` even when it is not needed. Be specific about when rules apply.

#### Few-Shot Prompting

**Few-shot prompting** means giving Claude examples of the input-output pattern you want before asking it to handle new cases. This is one of the most effective techniques for improving accuracy.

```
Classify the following customer messages:

Example 1:
Input: "I was charged twice for my order"
Output: {"category": "billing", "urgency": "high", "action": "investigate_duplicate_charge"}

Example 2:
Input: "When will my package arrive?"
Output: {"category": "shipping", "urgency": "medium", "action": "check_tracking"}

Now classify this message:
Input: "I want to return the shoes I bought last week"
```

**When to add few-shot examples:**
- When Claude consistently misclassifies or misformats output
- When there are ambiguous cases that need precedent
- When you need consistent formatting across responses
- When the task has edge cases that are not obvious from the instructions alone

**Key exam insight:** Few-shot examples are often the correct answer when the question describes inconsistent tool selection or output formatting. They are a low-effort, high-impact intervention.

#### Explicit Review Criteria

Vague instructions produce vague results. Compare:

**Vague:** "Review this code for quality."

**Explicit:**
```
Review this code against these criteria:
1. Security: Check for SQL injection, XSS, and unvalidated user input
2. Error handling: Verify all external calls have try/catch blocks
3. Performance: Flag any N+1 query patterns or unbounded loops
4. Style: Ensure naming follows camelCase convention

For each issue found, provide:
- File and line number
- Severity (critical / warning / info)
- Specific fix recommendation
```

The exam frequently tests whether you can identify that adding explicit criteria is more effective than vague instructions.

#### Prompt Chaining

**Prompt chaining** (also called **multi-pass architecture**) breaks a complex task into sequential focused steps:

```
Pass 1: Extract all entities from the document
Pass 2: Classify each entity by type
Pass 3: Resolve relationships between entities
Pass 4: Generate a structured summary
```

Each pass is a separate API call with a focused prompt. This is more reliable than asking Claude to do everything in one shot, especially for complex tasks.

#### Structured Output with `tool_use`

The most reliable way to get structured JSON output from Claude is to define a tool whose input schema matches your desired output format, then force Claude to call it with `tool_choice`:

```json
{
  "name": "extract_invoice",
  "description": "Extract structured data from an invoice document",
  "input_schema": {
    "type": "object",
    "properties": {
      "vendor_name": {"type": "string"},
      "invoice_number": {"type": "string"},
      "total_amount": {"type": "number"},
      "line_items": {
        "type": "array",
        "items": {
          "type": "object",
          "properties": {
            "description": {"type": "string"},
            "quantity": {"type": "integer"},
            "unit_price": {"type": "number"}
          },
          "required": ["description", "quantity", "unit_price"]
        }
      },
      "currency": {
        "type": "string",
        "enum": ["USD", "EUR", "GBP", "other"]
      }
    },
    "required": ["vendor_name", "invoice_number", "total_amount", "line_items"]
  }
}
```

Combined with `"tool_choice": {"type": "tool", "name": "extract_invoice"}`, this guarantees structured output that matches your schema.

#### Validation and Retry Loops

Even with schemas, Claude can make **semantic errors** — the JSON is valid but the data is wrong (e.g., extracting the wrong date or misclassifying a field). The standard pattern is:

```
1. Extract data using tool_use
2. Validate the output (check business rules, cross-reference fields)
3. If validation fails:
   a. Send the document + the incorrect extraction + the specific error back to Claude
   b. Ask Claude to fix the specific issue
   c. Validate again
4. If validation passes: accept the result
```

The key insight: include the **specific validation error** in the retry prompt. "Please try again" is useless; "The total_amount (150.00) does not match the sum of line_items (145.00)" gives Claude actionable feedback.

#### The Message Batches API

For processing large volumes of documents (100+ invoices, thousands of support tickets), the **Message Batches API** offers:

- **50% cost savings** compared to individual API calls
- Processing window of **up to 24 hours**
- Each request in the batch gets a **`custom_id`** so you can match results to inputs
- **No multi-turn tool calling** — each request is a single-turn extraction

This is ideal for structured data extraction at scale where results don't depend on each other.

#### Assistant Prefill

You can start Claude's response with specific text by including a partial assistant message. This is useful for:
- Preventing repetitive openings ("Certainly!", "I'd be happy to help!")
- Forcing a specific output format (start with `{` for JSON)
- Guiding the response direction

```json
{
  "messages": [
    {"role": "user", "content": "Analyze this code..."},
    {"role": "assistant", "content": "## Analysis\n\n**Critical Issues:**\n1."}
  ]
}
```

Claude will continue from the prefill rather than generating its own opening.

### Mini-Project: Build a Classification System

**Goal:** Create a prompt with few-shot examples for classifying customer support tickets.

**Time:** 1-2 hours

**Steps:**
1. Define 5 categories: billing, shipping, returns, technical, other
2. Write 2 few-shot examples per category (10 total)
3. Include one ambiguous example that could be multiple categories
4. Test with 10 new messages and evaluate accuracy
5. Add a "confidence" field to the output schema and evaluate whether low-confidence items are the ambiguous ones

### Mini-Project: Build a Data Extraction Pipeline

**Goal:** Extract structured data from unstructured text using `tool_use` and validation.

**Time:** 2-3 hours

**Steps:**
1. Define an extraction tool with a JSON schema (required/optional fields, enums, nullable)
2. Create 3 sample documents (e.g., invoices, receipts) with varying formats
3. Use `tool_choice` to force the extraction tool
4. Write a validation function that checks business rules (e.g., totals match line items)
5. Implement a retry loop that sends validation errors back to Claude

### Common Beginner Mistakes

1. **Using vague criteria.** "Review for quality" is not actionable. Specify exactly what to check.
2. **Not using few-shot examples when output is inconsistent.** If Claude keeps formatting things differently, add examples.
3. **Asking Claude to do everything in one prompt.** For complex tasks, use prompt chaining.
4. **Ignoring semantic errors.** Valid JSON does not mean correct data. Always validate beyond schema compliance.
5. **Using plain text output when structured data is needed.** Use `tool_use` with schemas for guaranteed structure.

### Domain 4 Checkpoint

1. When should you add few-shot examples to a prompt?
2. What is the difference between a syntax error and a semantic error in data extraction?
3. How do you force Claude to return structured JSON output?
4. What should a retry prompt include to help Claude fix an extraction error?
5. When would you use the Message Batches API?

---

## Domain 5: Context Management and Reliability (15%) — Week 8

> Documentation: [Messages API](https://platform.claude.com/docs/en/api/messages) | [Agent SDK Overview](https://platform.claude.com/docs/en/agent-sdk/overview) | [Claude Code Sub-agents](https://code.claude.com/docs/en/sub-agents)

### What This Domain Covers

As conversations grow longer and agent systems become more complex, managing the limited context window and ensuring reliable behavior becomes critical. This domain tests your ability to keep AI systems performing well over long interactions, handle errors gracefully, and know when to escalate to humans.

### Key Concepts

#### The Context Window Problem

The **context window** is the total amount of text (measured in **tokens**) that Claude can process in a single request. It includes everything: the system prompt, conversation history, tool definitions, and tool results.

When the context window fills up, you have a problem. You cannot simply keep adding messages — you must manage what stays in the context and what gets compressed or removed.

#### Lost-in-the-Middle Effect

Research shows that language models reliably process information at the **beginning** and **end** of long inputs but can miss details in the **middle**. This means:

- Place the most important instructions near the top (system prompt) or bottom (most recent messages)
- If you have a long document to analyze, place the key question at the end, after the document
- Do not bury critical constraints in the middle of a long system prompt

#### Progressive Summarization and Its Dangers

When conversations get long, one strategy is to **summarize** older messages. But summarization inherently loses precision:

- "The customer was offered a 15% discount" becomes "promotional pricing was discussed"
- Specific dates, amounts, order numbers, and percentages get lost

**Solution: Extract transactional facts into a persistent block:**

```
## Case Facts (preserved across summarization)
- Customer: Jane Smith (ID: 12345)
- Order: #67890, placed 2024-03-15
- Issue: Charged twice — $49.99 on 3/15 and $49.99 on 3/17
- Offered: 15% discount on next order
- Status: Awaiting refund confirmation
```

This block is included in every prompt, outside the summarized conversation history. Critical facts survive summarization.

#### Trimming Tool Results

Every tool call adds output to the context. If a tool returns 40 fields but only 5 matter, you waste context window space. Solutions:

- **PostToolUse hook** — trim tool results to include only relevant fields before they enter the conversation
- **Summary pattern** — have the tool return a summary instead of raw data
- **Progressive detail** — return a summary first, then allow follow-up calls for specific details

#### Using Subagents to Protect Context

When a task generates lots of output (e.g., searching 120 files for call sites), delegate it to a **subagent**. The subagent processes the noisy data in its own context and returns only a concise summary to the main conversation.

This is a frequently tested pattern: "The context window is filling up during discovery. What should you do?" Answer: use a subagent to isolate verbose output.

#### Scratchpad Files

For long-running tasks, use a **scratchpad file** to store intermediate results outside the context window. The agent writes findings to a file and reads them back when needed, rather than keeping everything in the conversation history.

#### Escalation Patterns

Not every request should be handled by the AI agent. The exam tests your ability to design **escalation criteria** — rules that determine when to hand off to a human.

**Justified escalation scenarios:**
- Policy gaps — the customer's request falls outside documented policies
- Contradictory data — tracking says "delivered" but customer says "not received"
- Safety or compliance concerns — actions that could cause financial or legal harm

**Not justified for escalation:**
- Multi-issue requests — the agent can decompose and handle these
- Standard processes — even complex ones, if the policy is clear
- The customer might change their mind — this is speculation, not a basis for escalation

**Implementing escalation:**
- Add explicit criteria to the system prompt with few-shot examples showing when to escalate vs resolve
- For critical operations (money, compliance), use **programmatic enforcement** (PreToolUse hooks that block unauthorized actions) rather than prompt instructions alone

#### Structured Handoff Protocols

When escalating to a human, include structured context:

```json
{
  "escalation_reason": "Policy gap — no guidance on competitor price matching",
  "customer_id": "12345",
  "conversation_summary": "Customer requesting competitor price match. Our policy covers price drops on our own site within 14 days but is silent on competitor prices.",
  "actions_taken": ["Verified customer identity", "Confirmed order details"],
  "actions_remaining": ["Policy decision on competitor matching"],
  "priority": "medium"
}
```

#### Confidence Calibration

For data extraction and classification tasks, adding **field-level confidence scores** helps route uncertain cases to humans:

- High confidence → automatic processing
- Medium confidence → spot-check sampling
- Low confidence → human review

Calibrate confidence thresholds on a labeled dataset before deploying to production.

#### Error Propagation in Multi-Agent Systems

When a subagent fails, the coordinator must handle it gracefully:

1. Return a **structured error** to the coordinator (not a generic "something went wrong")
2. The coordinator decides whether to retry, try an alternative, or continue with partial results
3. The final response to the user should acknowledge what was and was not available

**Provenance preservation:** In research systems where multiple agents contribute findings, track which agent produced which claim. If sources conflict, preserve both values with attribution rather than silently picking one.

### Mini-Project: Design a Context Management Strategy

**Goal:** Design a context management strategy for a customer support agent that handles 20+ turn conversations.

**Time:** 1-2 hours

**Steps:**
1. Define a "case facts" block structure with the fields that must survive summarization
2. Write a PostToolUse hook (pseudocode) that trims `get_customer` output from 40 fields to 5 relevant ones
3. Define the summarization trigger point (e.g., when context reaches 70% capacity)
4. Describe when to use a subagent for verbose operations

### Mini-Project: Design an Escalation Decision Tree

**Goal:** Create escalation criteria for a customer support agent.

**Time:** 1-2 hours

**Steps:**
1. List 5 scenarios that should be escalated and 5 that should not
2. Write system prompt instructions with escalation criteria
3. Add 2 few-shot examples: one showing correct escalation, one showing correct autonomous resolution
4. Define the structured handoff protocol (what context to pass to the human)

### Common Beginner Mistakes

1. **Not planning for long conversations.** If your agent can have 20+ turn conversations, you need a context management strategy from day one.
2. **Summarizing everything.** Precise values (amounts, dates, order numbers) must be extracted before summarization.
3. **Relying on prompts alone for safety-critical rules.** Use programmatic enforcement (hooks, preconditions) for actions involving money, compliance, or data deletion.
4. **Escalating too much or too little.** Over-escalation wastes human time; under-escalation risks errors. Use explicit criteria, not vague guidelines.
5. **Ignoring subagent failures.** Always handle partial failures — continue with available results rather than failing completely.

### Domain 5 Checkpoint

1. What is the "lost-in-the-middle" effect, and how do you mitigate it?
2. Why is progressive summarization dangerous for customer support conversations?
3. When should you use programmatic enforcement (hooks) vs prompt instructions for business rules?
4. What makes a good structured handoff to a human agent?
5. How do subagents help protect the context window?

---

# Phase 3: Hands-On Projects — Weeks 9-11

This phase puts everything together with five progressively complex projects. Each project maps to specific exam scenarios and covers multiple domains.

**Time commitment:** 12-15 hours per week

---

## Project 1: Multi-Turn Chatbot with Claude API

**Difficulty:** Basic
**Time:** 4-6 hours
**Exam scenarios:** Scenario 7 (Conversational AI Architecture Patterns)
**Domains covered:** 1 (Agent Architecture), 4 (Prompt Engineering)

### Goal

Build a multi-turn chatbot that maintains conversation history, uses a system prompt for persona, and handles basic context management.

### What You Will Learn

- How the stateless API works in practice (sending full history each time)
- How system prompts shape behavior across turns
- Basic context window awareness

### Steps

1. **Set up the project:**
   ```bash
   mkdir chatbot-project && cd chatbot-project
   pip install anthropic
   ```

2. **Write the basic chatbot:**
   ```python
   import anthropic

   client = anthropic.Anthropic()
   conversation_history = []

   system_prompt = """You are a friendly travel advisor. You help users plan trips 
   by asking about their preferences (budget, duration, interests) and suggesting 
   destinations. Always ask one follow-up question to refine your recommendations. 
   When you have enough information, provide a structured itinerary."""

   while True:
       user_input = input("You: ")
       if user_input.lower() in ["quit", "exit"]:
           break
       
       conversation_history.append({
           "role": "user",
           "content": user_input
       })
       
       response = client.messages.create(
           model="claude-sonnet-4-6",
           max_tokens=1024,
           system=system_prompt,
           messages=conversation_history
       )
       
       assistant_message = response.content[0].text
       conversation_history.append({
           "role": "assistant",
           "content": assistant_message
       })
       
       print(f"Advisor: {assistant_message}")
   ```

3. **Test multi-turn behavior:**
   - Have a 5+ turn conversation
   - Observe whether Claude remembers details from earlier turns
   - Notice how the system prompt shapes every response

4. **Add context awareness:**
   - Print the total message count and approximate token usage after each turn
   - Observe how the conversation history grows

5. **Experiment with assistant prefill:**
   - Add a partial assistant message to prevent repetitive openings
   - Compare the response style with and without prefill

### Expected Outcome

A working chatbot that demonstrates stateless API usage, conversation history management, and system prompt behavior. You should observe how Claude maintains coherence across turns because you send the full history each time.

---

## Project 2: Tool-Using Customer Support Agent

**Difficulty:** Intermediate
**Time:** 6-8 hours
**Exam scenarios:** Scenario 1 (Customer Support Agent), Scenario 4 (Developer Productivity Tools)
**Domains covered:** 1 (Agent Architecture), 2 (Tool Design), 4 (Prompt Engineering)

### Goal

Build an agent with the full agentic loop that uses tools to look up customer data, process actions, and escalate when appropriate.

### What You Will Learn

- The complete agentic loop with `stop_reason` checking
- Tool definition best practices
- Escalation criteria and hook-based enforcement

### Steps

1. **Define 4 tools with detailed descriptions:**
   ```python
   tools = [
       {
           "name": "get_customer",
           "description": "Finds a customer by email or customer ID. Returns profile including name, email, order history, and account status. Use this FIRST to verify customer identity before any other operations. Accepts email (format: user@domain.com) or customer_id (integer).",
           "input_schema": {
               "type": "object",
               "properties": {
                   "email": {"type": "string"},
                   "customer_id": {"type": "integer"}
               },
               "required": []
           }
       },
       {
           "name": "lookup_order",
           "description": "Retrieves order details by order number. Returns items, quantities, prices, shipping status, and delivery dates. Requires a verified customer_id from get_customer first.",
           "input_schema": {
               "type": "object",
               "properties": {
                   "order_id": {"type": "string"},
                   "customer_id": {"type": "integer"}
               },
               "required": ["order_id", "customer_id"]
           }
       },
       {
           "name": "process_refund",
           "description": "Processes a refund for a specific order. Maximum automatic refund is $100. Refunds above $100 require human approval via escalate_to_human. Returns confirmation number and estimated processing time.",
           "input_schema": {
               "type": "object",
               "properties": {
                   "order_id": {"type": "string"},
                   "amount": {"type": "number"},
                   "reason": {"type": "string"}
               },
               "required": ["order_id", "amount", "reason"]
           }
       },
       {
           "name": "escalate_to_human",
           "description": "Escalates the case to a human agent. Use when: (1) refund exceeds $100, (2) customer's request falls outside documented policies, (3) customer provides contradictory information that cannot be resolved with available tools.",
           "input_schema": {
               "type": "object",
               "properties": {
                   "reason": {"type": "string"},
                   "priority": {"type": "string", "enum": ["low", "medium", "high"]},
                   "context_summary": {"type": "string"}
               },
               "required": ["reason", "priority", "context_summary"]
           }
       }
   ]
   ```

2. **Implement mock tool execution:**
   ```python
   def execute_tool(tool_name, tool_input):
       if tool_name == "get_customer":
           return '{"customer_id": 12345, "name": "Jane Smith", "email": "jane@example.com", "status": "active", "member_since": "2023-01"}'
       elif tool_name == "lookup_order":
           return '{"order_id": "ORD-789", "items": [{"name": "Wireless Headphones", "price": 79.99}], "status": "delivered", "delivery_date": "2024-03-10"}'
       elif tool_name == "process_refund":
           amount = tool_input.get("amount", 0)
           if amount > 100:
               return '{"error": {"errorCategory": "LIMIT_EXCEEDED", "isRetryable": false, "message": "Refund exceeds $100 automatic limit. Use escalate_to_human."}}'
           return '{"confirmation": "REF-456", "processing_days": 3}'
       elif tool_name == "escalate_to_human":
           return '{"ticket_id": "ESC-001", "status": "created", "estimated_response": "2 hours"}'
   ```

3. **Implement the full agentic loop** (use the pattern from Domain 1)

4. **Add a PreToolUse hook** that blocks `process_refund` if amount > 100:
   ```python
   def pre_tool_use_hook(tool_name, tool_input):
       if tool_name == "process_refund" and tool_input.get("amount", 0) > 100:
           return {"blocked": True, "reason": "Refund exceeds $100. Must escalate to human."}
       return {"blocked": False}
   ```

5. **Test with these scenarios:**
   - "I need a refund for order ORD-789" (simple case)
   - "Refund my $150 order" (should trigger escalation)
   - "My order says delivered but I never got it" (contradictory — should escalate)

### Expected Outcome

A working agent that correctly sequences tool calls (get_customer first, then lookup_order, then action), handles escalation for edge cases, and uses programmatic enforcement for refund limits.

---

## Project 3: MCP Server Integration

**Difficulty:** Intermediate
**Time:** 6-8 hours
**Exam scenarios:** Scenario 4 (Developer Productivity Tools), Scenario 8 (Agentic AI Tools)
**Domains covered:** 2 (Tool Design and MCP), 3 (Claude Code Configuration)

### Goal

Build a simple MCP server that exposes tools, configure it with Claude Code, and test the integration.

### What You Will Learn

- How MCP servers work in practice
- Tool registration and description best practices
- Configuration with `.mcp.json` and environment variables
- Error handling with `isError`

### Steps

1. **Create a simple MCP server** that exposes 2-3 tools (e.g., a note-taking server with `create_note`, `list_notes`, `search_notes`)
2. **Write detailed tool descriptions** that differentiate each tool
3. **Implement error handling** with structured errors and the `isError` flag
4. **Configure the server in `.mcp.json`** with environment variables
5. **Test with Claude Code** — ask Claude to use your MCP tools
6. **Create a user-level override** in `~/.claude.json` for personal settings

### Expected Outcome

A working MCP server connected to Claude Code, with proper error handling and configuration at both project and user levels.

---

## Project 4: Multi-Agent Research System

**Difficulty:** Advanced
**Time:** 8-10 hours
**Exam scenarios:** Scenario 3 (Multi-Agent Research System)
**Domains covered:** 1 (Agent Architecture), 2 (Tools), 5 (Context Management and Reliability)

### Goal

Build a coordinator agent that delegates research tasks to specialized subagents and synthesizes their results.

### What You Will Learn

- Hub-and-spoke architecture in practice
- Explicit context passing between coordinator and subagents
- Handling partial failures
- Provenance tracking (which source said what)

### Steps

1. **Define the coordinator** with a system prompt that explains its role: receive a research question, decompose it into subtasks, delegate to subagents, synthesize results

2. **Create 2 subagents:**
   - **Fact-finder** — given a specific claim, searches for supporting evidence
   - **Analyzer** — given a set of facts, identifies patterns and draws conclusions

3. **Implement explicit context passing:**
   ```python
   # The coordinator passes specific context to each subagent
   fact_finder_prompt = f"""
   Research the following claim: "{claim}"
   
   Context from the coordinator:
   - Original question: {original_question}
   - Specific aspect to investigate: {aspect}
   
   Return your findings as structured output:
   - claim: the specific claim investigated
   - supported: true/false/unclear
   - evidence: list of supporting or contradicting evidence
   - sources: list of source descriptions
   """
   ```

4. **Handle subagent failures:**
   - Simulate a timeout for one subagent
   - Have the coordinator continue with partial results
   - Include in the final response which aspects could not be researched

5. **Track provenance:**
   - Each subagent returns structured output with source attribution
   - The coordinator preserves source information in the final synthesis
   - When sources conflict, present both perspectives with attribution

### Expected Outcome

A working multi-agent system where the coordinator decomposes questions, delegates to subagents, handles failures gracefully, and produces a synthesis with proper source attribution.

---

## Project 5: CI/CD Pipeline with Claude Code

**Difficulty:** Advanced
**Time:** 6-8 hours
**Exam scenarios:** Scenario 2 (Code Generation), Scenario 5 (CI/CD)
**Domains covered:** 3 (Claude Code Configuration), 4 (Prompt Engineering), 5 (Reliability)

### Goal

Set up Claude Code in a CI/CD workflow for automated code review with structured output.

### What You Will Learn

- Headless mode (`-p` flag)
- Structured output with `--output-format json` and `--json-schema`
- CLAUDE.md configuration for review criteria
- Path-scoped rules for different code areas

### Steps

1. **Create a sample project** with intentional issues:
   - A file with a SQL injection vulnerability
   - A file with poor error handling
   - A test file with incomplete coverage

2. **Configure Claude Code:**
   - Write a `CLAUDE.md` with review criteria
   - Create `.claude/rules/` for API-specific and test-specific rules
   - Create a `/review` slash command

3. **Write a review script** that runs Claude Code in headless mode:
   ```bash
   claude -p "Review the changes in this PR against the project coding standards. \
   Focus on security vulnerabilities, error handling, and test coverage." \
   --output-format json
   ```

4. **Define an output schema** for structured review results:
   ```json
   {
     "type": "object",
     "properties": {
       "findings": {
         "type": "array",
         "items": {
           "type": "object",
           "properties": {
             "file": {"type": "string"},
             "line": {"type": "integer"},
             "severity": {"type": "string", "enum": ["critical", "warning", "info"]},
             "category": {"type": "string"},
             "description": {"type": "string"},
             "suggestion": {"type": "string"}
           },
           "required": ["file", "severity", "category", "description"]
         }
       },
       "summary": {"type": "string"},
       "pass": {"type": "boolean"}
     },
     "required": ["findings", "summary", "pass"]
   }
   ```

5. **Simulate a CI pipeline** that runs the review and parses the JSON output

### Expected Outcome

A working automated code review pipeline that uses Claude Code in headless mode, produces structured findings, and can be integrated into a CI/CD workflow.

---

## Projects Phase Summary

| Project | Scenario 1 | Scenario 2 | Scenario 3 | Scenario 4 | Scenario 5 | Scenario 6 | Scenario 7 | Scenario 8 |
|---------|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1. Chatbot | | | | | | | X | |
| 2. Support Agent | X | | | X | | | | |
| 3. MCP Server | | | | X | | | | X |
| 4. Multi-Agent | | | X | | | | | |
| 5. CI/CD Pipeline | | X | | | X | | | |

**Scenario 6** (Structured Data Extraction) is covered by the mini-projects in Domain 4 (the data extraction pipeline).

### Projects Phase Checkpoint

Reflect on these questions:
1. Which domain concepts became clearest through building projects?
2. Where did you struggle most — tool design, context management, or prompt engineering?
3. Which exam scenarios do you feel most prepared for? Which need more study?

---

# Phase 4: Exam Preparation — Weeks 12-13

This final phase bridges from learning to exam readiness. You will work through the comprehensive study guide, take practice tests, and learn exam-specific strategies.

**Time commitment:** 10-12 hours per week

---

## How to Use the Comprehensive Study Guide

The study guide ([`guide_en.MD`](./guide_en.MD)) is your primary exam preparation resource. Here is the recommended reading order:

### Reading Strategy

**First pass (skim for structure):**
1. Read the **Appendix: Technologies and Concepts** — this is a one-page summary of everything on the exam
2. Read the **Out-of-Scope Topics** — know what you do NOT need to study

**Second pass (domain-focused study):**
3. Read **Part I: Theory Foundations** (Chapters 1-5) — focus on domains where you feel weakest after the projects phase
4. Read the exam domain details — connect theory to exam format

**Third pass (practice):**
5. Work through the **Practical Exercises** (4 exercises at the end of the guide)
6. Answer all **practice questions** (76+ questions across multiple scenarios)

### Identifying Weak Domains

After completing the projects in Phase 3, rate your confidence in each domain:

| Domain | Weight | Your Confidence (1-5) | Study Priority |
|---|---|---|---|
| 1. Agent Architecture (27%) | Highest | ___ | ___ |
| 2. Tool Design & MCP (18%) | Medium | ___ | ___ |
| 3. Claude Code (20%) | High | ___ | ___ |
| 4. Prompt Engineering (20%) | High | ___ | ___ |
| 5. Context & Reliability (15%) | Medium | ___ | ___ |

Focus your remaining study time on domains where your confidence is lowest, weighted by exam importance. A weak Domain 1 (27%) matters more than a weak Domain 5 (15%).

---

## How to Use the Practice Tests

### The Interactive Practice Test

Open [`practical_test_en.html`](./practical_test_en.html) in your browser. This is a self-contained interactive exam that:
- Presents questions organized by scenario
- Tracks your progress
- Shows explanations after you answer
- Provides a performance summary at the end

### Strategy

1. **Take it cold first.** Do not study the answers beforehand. This baseline shows your actual gaps.
2. **Score yourself.** Aim for 75%+ to be exam-ready (the actual passing score is 720/1000).
3. **Review wrong answers by domain.** Group your mistakes — are they concentrated in one domain?
4. **Study the gaps.** Go back to the relevant sections in `guide_en.MD` for topics you missed.
5. **Retake after studying.** You should see improvement in your weak areas.
6. **Answer everything.** There is no guessing penalty — never leave a question blank.

---

## Exam Strategies and Time Management

### Understanding Question Patterns

The exam uses consistent phrasing patterns. Learn to recognize them:

- **"What is the most effective approach?"** — the correct answer is the most direct, proportional solution. Avoid overengineered options.
- **"What should you check first?"** — the correct answer is the simplest diagnostic step. Start with tool descriptions, not infrastructure.
- **"What is the most likely root cause?"** — look for the explanation that matches the observed symptoms most precisely.

### Decision Frameworks

When two answers seem reasonable, use these frameworks:

**Prompt vs Code enforcement:**
- If the scenario involves money, compliance, or safety → **code/hooks** (deterministic)
- If the scenario involves style, tone, or formatting → **prompts** (flexible)

**Tool descriptions vs classifiers:**
- If tools are being confused → **fix tool descriptions first** (simplest intervention)
- Only add routing classifiers if descriptions alone cannot solve the problem

**Simplicity vs infrastructure:**
- If the fix can be done with a prompt change → do that first
- Classifiers, separate models, fine-tuning, and complex infrastructure are usually wrong answers

### Common Exam Traps

1. **The overengineering trap.** Answers that propose classifiers, sentiment analysis, separate routing models, or fine-tuning are almost always wrong. The exam rewards proportional solutions.

2. **The deterministic vs probabilistic trap.** When the question involves blocking unauthorized actions (refunds over a limit, data deletion), the answer is programmatic enforcement (hooks, preconditions), not prompt instructions. Prompts are probabilistic — they usually work but can fail.

3. **The context management trap.** When context is growing, the answer is usually trimming, subagents, or scratchpad files — not increasing `max_tokens`. `max_tokens` controls output length, not input capacity.

4. **The tool confusion trap.** When Claude picks the wrong tool, fix the tool descriptions first. Do not add routing infrastructure before trying the simplest fix.

5. **The escalation trap.** Over-escalation (sending everything to humans) is wrong. Under-escalation (handling everything autonomously) is also wrong. The answer is explicit criteria with few-shot examples.

---

## Out-of-Scope Topics

Do NOT waste time studying these — they will NOT be on the exam:

- Fine-tuning Claude models or training custom models
- Claude API authentication, billing, or account management
- Detailed implementation in specific programming languages or frameworks
- Deploying or hosting MCP servers (infrastructure, networking, containers)
- Claude's internal architecture, training process, or model weights
- Constitutional AI, RLHF, or safety training methodologies
- Embedding models or vector database implementation
- Computer use (browser automation, desktop interaction)
- Image analysis capabilities (Vision)
- Streaming API or server-sent events
- Rate limiting, quotas, or API cost calculations
- OAuth, API key rotation, or authentication protocols
- Cloud-provider-specific configurations (AWS, GCP, Azure)
- Performance benchmarks or model comparison metrics
- Prompt caching implementation details
- Token counting algorithms or tokenization specifics

---

## Final Readiness Checklist

Before taking the exam, verify you can answer "yes" to each item:

### Domain 1: Agent Architecture and Orchestration
- [ ] I can explain the agentic loop and how `stop_reason` controls it
- [ ] I understand the hub-and-spoke architecture for multi-agent systems
- [ ] I know that subagents do not inherit coordinator context
- [ ] I can describe when to use fixed pipelines vs adaptive agents
- [ ] I understand PreToolUse and PostToolUse hooks

### Domain 2: Tool Design and MCP Integration
- [ ] I can write effective tool descriptions that differentiate similar tools
- [ ] I understand `tool_choice` options (auto, any, forced)
- [ ] I can explain MCP architecture (client, server, tools, resources)
- [ ] I know where to configure MCP servers (`.mcp.json` vs `~/.claude.json`)
- [ ] I can design structured error responses with `isError`

### Domain 3: Claude Code Configuration and Workflows
- [ ] I understand the CLAUDE.md hierarchy (user → project → directory)
- [ ] I can create path-scoped rules in `.claude/rules/`
- [ ] I know the difference between slash commands and skills
- [ ] I can explain when to use planning mode vs direct execution
- [ ] I know how to run Claude Code in headless mode for CI/CD

### Domain 4: Prompt Engineering and Structured Output
- [ ] I can write few-shot examples for classification and extraction tasks
- [ ] I understand how to use `tool_use` for guaranteed structured output
- [ ] I can design validation and retry loops for data extraction
- [ ] I know when to use prompt chaining vs single-pass approaches
- [ ] I understand the Message Batches API and when to use it

### Domain 5: Context Management and Reliability
- [ ] I can explain the lost-in-the-middle effect and how to mitigate it
- [ ] I know the dangers of progressive summarization and how to preserve critical facts
- [ ] I can design escalation criteria with few-shot examples
- [ ] I understand when to use programmatic enforcement vs prompt instructions
- [ ] I can describe how subagents protect the context window

**If you checked 18+ items:** You are ready for the exam.
**If you checked 14-17 items:** Review the domains where you have gaps.
**If you checked fewer than 14:** Spend more time on the projects and study guide.

---

# Key Concepts Glossary

Quick-reference definitions for all key terms used in this guide and on the exam.

| Term | Definition | Primary Domain |
|---|---|---|
| **Agent Loop (Agentic Loop)** | The core pattern where Claude sends a request, checks `stop_reason`, executes tools if needed, and loops until done | Domain 1 |
| **AgentDefinition** | The configuration object in the Claude Agent SDK that defines an agent's model, tools, system prompt, and behavior | Domain 1 |
| **allowedTools** | A property that restricts which tools a specific agent or skill can access | Domains 1, 3 |
| **Assistant Prefill** | Starting Claude's response with specific text to guide output format or prevent repetitive openings | Domain 4 |
| **Batch API (Message Batches)** | An API for processing large volumes of requests at 50% cost savings with up to 24-hour processing window | Domain 4 |
| **Built-in Tools** | Tools included with Claude Code: Read, Write, Edit, Bash, Grep, Glob | Domains 2, 3 |
| **CLAUDE.md** | A markdown configuration file that provides Claude Code with persistent project context | Domain 3 |
| **Claude Agent SDK** | Anthropic's framework for building AI agents with tool use, subagents, hooks, and session management | Domain 1 |
| **Claude Code** | An AI-powered development tool that runs in your terminal and IDE | Domain 3 |
| **Confidence Calibration** | Assigning reliability scores to AI outputs and routing uncertain cases to human review | Domain 5 |
| **Context Window** | The total amount of text (in tokens) that Claude can process in a single request | Domain 5 |
| **Coordinator** | The central agent in a hub-and-spoke system that decomposes tasks and delegates to subagents | Domain 1 |
| **custom_id** | A user-defined identifier in the Batch API for matching results to input requests | Domain 4 |
| **end_turn** | A `stop_reason` value meaning Claude has finished generating its response | Domain 1 |
| **Escalation** | Handing off a request to a human agent when the AI cannot or should not handle it | Domain 5 |
| **Extended Thinking** | A feature that allows Claude to reason step-by-step before responding | Domain 4 |
| **Few-Shot Prompting** | Providing examples of desired input-output patterns to guide Claude's behavior | Domain 4 |
| **fork_session** | Creating an independent copy of a conversation that diverges from the original | Domains 1, 3 |
| **Headless Mode** | Running Claude Code non-interactively with the `-p` flag, used for CI/CD | Domain 3 |
| **Hook** | A function that runs before (PreToolUse) or after (PostToolUse) a tool execution | Domains 1, 5 |
| **Hub-and-Spoke** | An architecture where a coordinator agent delegates tasks to specialized subagents | Domain 1 |
| **Human-in-the-Loop** | A design pattern where human oversight is integrated into automated workflows | Domain 5 |
| **isError** | A flag in MCP tool responses indicating that the tool call failed | Domain 2 |
| **JSON Schema** | A standard for describing the structure of JSON data, used for tool input definitions | Domains 2, 4 |
| **Lost-in-the-Middle** | The tendency of LLMs to miss information placed in the middle of long inputs | Domain 5 |
| **max_tokens** | The maximum number of tokens Claude will generate in its response | Domain 1 |
| **MCP (Model Context Protocol)** | An open standard for connecting AI applications to external data sources and tools | Domain 2 |
| **MCP Resources** | Data that an MCP server makes available for Claude to read | Domain 2 |
| **MCP Server** | A program that exposes tools and resources to AI clients via the MCP protocol | Domain 2 |
| **MCP Tools** | Actions that an MCP server exposes for Claude to call | Domain 2 |
| **Nullable Fields** | JSON schema fields that can be explicitly set to `null`, distinct from being omitted | Domain 4 |
| **Planning Mode** | A Claude Code mode for complex tasks where Claude creates a plan before executing | Domain 3 |
| **PostToolUse Hook** | A hook that runs after a tool executes; used for logging, trimming output, modifying results | Domains 1, 5 |
| **PreToolUse Hook** | A hook that runs before a tool executes; used for validation, blocking unauthorized actions | Domains 1, 5 |
| **Progressive Summarization** | Compressing older conversation messages to save context window space; risks losing precise values | Domain 5 |
| **Prompt Chaining** | Breaking a complex task into sequential focused API calls | Domain 4 |
| **Provenance** | Tracking which source or agent produced which piece of information | Domain 5 |
| **Scratchpad** | An external file used to store intermediate results outside the context window | Domain 5 |
| **Session** | A conversation instance that can be resumed, forked, or named | Domains 1, 3 |
| **Skills** | Reusable capability packages in Claude Code with SKILL.md configuration | Domain 3 |
| **Slash Commands** | Custom commands stored in `.claude/commands/` triggered by `/command-name` | Domain 3 |
| **stop_reason** | A field in the API response indicating why Claude stopped generating: `end_turn`, `tool_use`, `max_tokens` | Domain 1 |
| **Structured Output** | Ensuring Claude returns data in a specific format (typically JSON via `tool_use`) | Domain 4 |
| **Subagent** | A specialized agent spawned by a coordinator to handle a specific subtask | Domain 1 |
| **System Prompt** | A special instruction that defines Claude's role, constraints, and behavior rules | Domains 1, 4 |
| **Task Tool** | The mechanism in the Agent SDK for a coordinator to spawn and communicate with subagents | Domain 1 |
| **Token** | The basic unit of text that language models process (roughly 3/4 of a word in English) | Domain 5 |
| **tool_choice** | A parameter controlling whether Claude can choose tools (`auto`), must use one (`any`), or must use a specific one | Domain 2 |
| **tool_use** | The mechanism allowing Claude to call external functions by generating structured tool call requests | Domain 2 |
| **@path Syntax** | CLAUDE.md syntax for importing content from other files | Domain 3 |

---

# Resource Map

## Official Anthropic Documentation

| Resource | URL |
|---|---|
| **Claude API — Messages** | https://platform.claude.com/docs/en/api/messages |
| **Claude API — Tool Use** | https://platform.claude.com/docs/en/build-with-claude/tool-use |
| **Claude API — Message Batches** | https://platform.claude.com/docs/en/build-with-claude/message-batches |
| **Claude Agent SDK — Overview** | https://platform.claude.com/docs/en/agent-sdk/overview |
| **Claude Agent SDK — Hooks** | https://platform.claude.com/docs/en/agent-sdk/hooks |
| **Claude Agent SDK — Subagents** | https://platform.claude.com/docs/en/agent-sdk/subagents |
| **Claude Agent SDK — Sessions** | https://platform.claude.com/docs/en/agent-sdk/sessions |
| **Model Context Protocol (MCP)** | https://modelcontextprotocol.io/ |
| **MCP — Tools** | https://modelcontextprotocol.io/docs/concepts/tools |
| **MCP — Resources** | https://modelcontextprotocol.io/docs/concepts/resources |
| **MCP — Servers** | https://modelcontextprotocol.io/docs/concepts/servers |
| **Claude Code — Documentation** | https://code.claude.com/docs/en/overview |
| **Claude Code — CLAUDE.md and Memory** | https://code.claude.com/docs/en/memory |
| **Claude Code — Skills** | https://code.claude.com/docs/en/skills |
| **Claude Code — Hooks** | https://code.claude.com/docs/en/hooks |
| **Claude Code — Sub-agents** | https://code.claude.com/docs/en/sub-agents |
| **Claude Code — MCP Integration** | https://code.claude.com/docs/en/mcp |
| **Claude Code — GitHub Actions CI/CD** | https://code.claude.com/docs/en/github-actions |
| **Claude Code — GitLab CI/CD** | https://code.claude.com/docs/en/gitlab-ci-cd |
| **Claude Code — Headless Mode** | https://code.claude.com/docs/en/headless |
| **Prompt Engineering Guide** | https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/overview |
| **Extended Thinking** | https://platform.claude.com/docs/en/build-with-claude/extended-thinking |
| **Anthropic Cookbook** | https://github.com/anthropics/anthropic-cookbook |

## Free Anthropic Academy Courses

These courses are recommended as part of this preparation roadmap:

| # | Course | Link | Phase |
|---|---|---|---|
| 1 | Claude 101 | [Link](https://anthropic.skilljar.com/claude-101) | Week 1 |
| 2 | AI Fluency: Framework & Foundations | [Link](https://anthropic.skilljar.com/ai-fluency-framework-foundations) | Week 1 |
| 3 | Building with the Claude API | [Link](https://anthropic.skilljar.com/claude-with-the-anthropic-api) | Week 2 |
| 4 | Claude Code in Action | [Link](https://anthropic.skilljar.com/claude-code-in-action) | Week 2 |
| 5 | Introduction to Agent Skills | [Link](https://anthropic.skilljar.com/introduction-to-agent-skills) | Week 3 |
| 6 | Intro to Model Context Protocol | [Link](https://anthropic.skilljar.com/introduction-to-model-context-protocol) | Week 3 |
| 7 | MCP: Advanced Topics | [Link](https://anthropic.skilljar.com/model-context-protocol-advanced-topics) | Week 3 |

Additional courses (optional but recommended):

| # | Course | Link |
|---|---|---|
| 8 | Claude with Amazon Bedrock | [Link](https://anthropic.skilljar.com/claude-in-amazon-bedrock) |
| 9 | Claude with Google Cloud's Vertex AI | [Link](https://anthropic.skilljar.com/claude-with-google-vertex) |

## Repository Resources

| Resource | Path | Description |
|---|---|---|
| Comprehensive Study Guide | [`guide_en.MD`](./guide_en.MD) | Deep technical content, 76+ practice questions, practical exercises |
| Interactive Practice Test | [`practical_test_en.html`](./practical_test_en.html) | Browser-based practice exam with scoring |
| PDF Study Guide | [`pdf/guide_en.pdf`](./pdf/guide_en.pdf) | Offline-friendly PDF version |

## Resources by Exam Domain

| Domain | Key Documentation | Courses | Guide Chapters |
|---|---|---|---|
| 1. Agent Architecture | Agent SDK Overview, Hooks, Subagents, Sessions | Building with Claude API, Agent Skills | Chapters 1, 5 |
| 2. Tool Design & MCP | Tool Use, MCP, MCP Tools, Resources, Servers | Intro to MCP, MCP Advanced | Chapters 2, 3 |
| 3. Claude Code | Claude Code Overview, Memory, Skills, Hooks, GitHub Actions | Claude Code in Action, Agent Skills | Chapter 4 |
| 4. Prompt Engineering | Prompt Engineering Guide, Extended Thinking, Messages API | Building with Claude API, Claude 101 | Chapters 1, 8 |
| 5. Context & Reliability | Messages API, Agent SDK, Sub-agents | MCP Advanced Topics | Chapters 1, 5, 9 |

---

## Certification Access

- **Exam Portal:** https://anthropic.skilljar.com/claude-certified-architect-foundations-access-request
- **Anthropic Partner Network:** https://claude.com/partners
- **Claude Code Cheatsheet:** https://claude-guides.com

---

*This guide is part of the [Claude Certified Architect — Foundations](./README.md) study materials. For the comprehensive exam study guide with practice questions, see [`guide_en.MD`](./guide_en.MD).*

# Hello World Agent 👋

> A minimal starter agent built on Relevance AI that greets users and confirms your setup is working.

---

## Overview

The **Hello World Agent** is a lightweight, beginner-friendly agent designed as a first build on the Relevance AI platform. Its primary purpose is to validate that your Relevance AI environment is correctly configured and operational. When triggered, it responds with a warm greeting, includes the phrase "Hello World", and confirms the agent is running successfully.

| Property | Value |
|---|---|
| **Agent ID** | `1b711576-6335-40d3-9e32-829161d4ca10` |
| **Type** | Default |
| **Model** | `relevance-cost-optimized` |
| **Temperature** | `0` (deterministic responses) |
| **Autonomy Limit** | 20 steps |
| **Autonomy Behaviour** | Ask for approval |
| **Memory** | Disabled |
| **Thinking** | Disabled |
| **Scheduled Triggers** | Disabled |
| **Python Executor** | Disabled |
| **Tools Attached** | None |
| **Created** | 2026-05-11 |
| **Last Updated** | 2026-05-11T05:47:10Z |
| **Last Run** | 2026-05-11 |

---

## System Prompt

```
You are a simple Hello World agent for a first Relevance AI build. When a user messages you,
greet them warmly, include the exact phrase "Hello World", and briefly explain that this
confirms the agent is running successfully. Keep responses concise, friendly, and
beginner-friendly.

```

---

## Behaviour

- **Greeting**: Always responds warmly to any incoming message
- **Confirmation phrase**: Always includes "Hello World" in its response
- **Tone**: Concise, friendly, and beginner-friendly
- **Action Behaviour**: Always asks before taking actions (set to `always-ask`)

---

## Metadata Management

The agent uses internal metadata conventions to stay contextually aware:

- **Write metadata**: Calls `add_conversation_metadata` whenever tracked values change — particularly at task completion or before handing off
- **Read metadata**: Calls `read_conversation_metadata` only when metadata is not already available in context, avoiding unnecessary tool calls

---

## Conversation History

The agent has been run in **3 tasks**:

| # | Title | Date |
|---|---|---|
| 1 | Test the Agent | 2026-05-11 |
| 2 | Test the agent | 2026-05-11 |
| 3 | Introduce Yourself Conversation | 2026-05-11 |

---

## Evaluations

The agent has **1 test set** configured to validate its core behaviour.

### Test Set: Hello World Response Eval

| Property | Value |
|---|---|
| **Test Set ID** | `9f40e6e6-48c6-465f-a5f8-d2f255a070b2` |
| **Created** | 2026-05-11 |
| **Test Cases** | 1 |

#### Test Case: Response contains Hello World

| Property | Value |
|---|---|
| **Test Case ID** | `35f65078-e819-4fd4-8121-a055a92cb6e5` |
| **Prompt** | "Please introduce yourself." |
| **Max Turns** | 1 |
| **Runs per Scenario** | 1 |

**Evaluator Rules:**

| Rule | Type | Expected Value |
|---|---|---|
| Contains exact phrase Hello World | `string_contains` | `Hello World` |

This eval confirms that whenever a user sends a message to the agent, the response always includes the literal phrase "Hello World" — the agent's primary success criterion.

---

## Tools & Triggers

- **Tools attached**: None
- **Triggers configured**: None (no webhooks, schedules, or event-based triggers)

---

## Use Cases

- ✅ **Setup validation** — Confirm your Relevance AI project is correctly configured
- ✅ **Onboarding** — Introduce new team members to the Relevance AI platform
- ✅ **Template baseline** — Use as a starting point for building more complex agents
- ✅ **Integration testing** — Quickly verify API connectivity and agent responsiveness

---

## Getting Started

1. Navigate to your [Relevance AI](https://relevanceai.com) project
2. Open the **Hello World Agent** from the Agents panel
3. Send any message (e.g. "Hello!" or "Are you working?")
4. The agent will respond with a greeting including "Hello World" and confirm it's running

---

## Project Information

| Property | Value |
|---|---|
| **Project ID** | `840a7599-e701-4c97-b563-fc387a43b97e` |
| **Last Updated By** | Jeff Haw |
| **Version ID** | `01cfdfda-d492-42d0-91e3-c06529409326` |

---

## Notes

- This agent is intentionally minimal — it has no tools, no memory, and no triggers
- Temperature is set to `0` for fully deterministic and consistent outputs
- The `relevance-cost-optimized` model is used to keep costs minimal for this starter agent
- Ideal as a reference point before building production agents with more complex configurations

---

*Documentation last refreshed on 2026-05-11T05:47Z using the Relevance AI MCP.*
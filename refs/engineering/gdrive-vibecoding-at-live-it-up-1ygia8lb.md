---
type: ref
domain: engineering
author: claudata
run: drive-sync-g0oit8-2026-09-16T03:34:49.457Z
source: https://docs.google.com/document/d/1YGIA8lBvzhhH-OBsVOr3bNTqMIpj1lK3H4Lxcel_OGc/edit?usp=drivesdk
created: 2026-09-16
review_by: 2027-03-15
approved_by: null
approved_at: null
approval_ref: null
supersedes: null
system: gdrive
locator: https://www.googleapis.com/drive/v3/files/1YGIA8lBvzhhH-OBsVOr3bNTqMIpj1lK3H4Lxcel_OGc
---

# Vibecoding at Live it Up 🔮

- Drive: https://docs.google.com/document/d/1YGIA8lBvzhhH-OBsVOr3bNTqMIpj1lK3H4Lxcel_OGc/edit?usp=drivesdk
- Location: Vibecoding at Live it Up 🔮
- Type: application/vnd.google-apps.document (3639489 bytes)
- Modified in Drive: 2026-09-16T00:13:36.875Z
- Ingested: 2026-09-16T03:34:49.457Z by reedright Drive sync, Google Doc exported as Markdown
- Images: 2 embedded images omitted (open the Drive file to see them)

---

[image omitted]

# Vibecoding at Live it Up

What’s *vibecoding*? Writing code with the help of AI assistants.

The degree to which it can be done well or go horribly awry depends largely on what you include in your prompt and how well you instruct AI to develop.

Generally speaking, ***the more verbose the prompt and the more context you include, the better your outputs will be*****.**

You may think of *vibecoding* as **another level of programming abstraction** (prompt engineering). One that is a level higher than when writing code directly (“direct” software engineering); Just like writing code directly is one level higher than writing machine instructions in assembler.

This is why, at LiU, we believe *vibecoding* is the **next paradigm in developing software.** We wholeheartedly embrace it and work on maximizing its efficiency. We also believe **it is a proper software engineering discipline** that requires an engineering mindset to maximize results. 

For vibecoding to be successful, we are developing this **vibecoding standard** around it. Using this standard, we maximize the velocity and reliability of the produced code.

Our approach to vibecoding consists of the following ceremonies and artifacts

0. *Business requirements and the project get created and approved just like in any other product development process.*  
1. We start by translating business requirements into high-level **product requirements**.  
2. We work on **system and software architecture plan**.  
3. From the architecture, we create a **feature roadmap** and templates for task execution by AI.  
4. We guide AI with rules and instructions in the form of [cursor rules](https://docs.cursor.com/context/rules) or [Agents.md](http://Agents.md) files such that the IDE (Cursor) or the cloud-based autonomous agent (codex) **knows what files to read to augment the prompt you give it with the context you’ve already provided**

# An Example

The files listed below provide an example of documents produced in cooperation with AI during scoping of the 1st-party web event tracking tool.

* [`Product`](https://drive.google.com/file/d/1cvHmzka1BDd0lUVm4b9CVZ9Xago-9Vip/view) `Requirements.md`  
* [`Architecture.md`](https://drive.google.com/file/d/1tMkPmSuPRGPWQn3FwtzzmeelhYZFer8Q/view)  
* [`WorkPlan.md`](https://drive.google.com/file/d/1wOCYVl_RaxW7KEJ6HXU8Hyq2w6NPhNND/view)

# Step details

**The Product Requirements** document serves to provide a business case for the project, state the problems it solves, list out high-level descriptions of core features, milestones, etc. It paints a high-level picture that is detailed enough to derive the technical specification from. But it does not necessarily describe every single feature. 

The process of creating this document might look like this:

- Start with listing the major features of the tool, maybe compare it to something else that exists already.   
- Ramble-chat with GPT or whoever else to brainstorm the idea, business, and technical feasibility, build vs buy, scale and security, and narrow down the scope.  
- Ask an LLM to interpolate the transcript of that conversation into the product requirements with a proper structure of headings/domains and descriptions.  
- Double-check the generated content, give it some edits if needed, and make sure it captures your initial idea properly.

**Architecture** \- it’s important in a technical context to have your ducks in a row when it comes to tech stack. This includes not just programming languages, but runtime environments, how code gets deployed there, secrets storage, data persistence, testing approach, etc. Write out a prompt with as much detail as you can about how you see these choices coming together in the project, and then @-mention the Product requirements doc and ask your assistant to create an Architecture.md file in the prompts-and-reqs folder.

| *👉 Keep in mind you are still in the driver's seat here and need to do the final signoff. After AI suggests the architecture, review it, polish it, and proceed with the next step.* |
| :---- |

**The workplan doc** is a project-agnostic document that tells AI how to plan its workload. Keep it in your project code and let the AI reference it during planning and execution.

### Planning the Plan

The next prompt should read something like:

*Given all the context so far in  `@/prompts-and-reqs`*  folder*, please decompose the project into well-defined implementable chunks that are easy to reason about. Create a new folder called `steps` in `@/prompts-and-reqs` , and include a series of steps, each in files with names like `00-implementation-roadmap.md`, and `01-project-setup.md`, and so forth.*

Now, you’ll likely have a whole lot of tasks you can set cursor/codex off on\! Don’t forget to reference the [WorkPlan.md](https://drive.google.com/open?id=1wOCYVl_RaxW7KEJ6HXU8Hyq2w6NPhNND) file explicitly or in your cursor/agents.md rules\! :)

[image omitted]

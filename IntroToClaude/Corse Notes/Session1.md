# Session 1 Takeaway — The Three Claude Tools

Keep this. It's your reference for which tool to reach for and when.

---

## The Three Tools

| Tool | Best For | Can't Do |
|------|----------|----------|
| **Claude Desktop** | Thinking, planning, brainstorming, decisions | Can't see your files or run code |
| **Claude Code (VS Code)** | Working with files, editing code, iterating on output | Requires VS Code |
| **Claude Code (Terminal)** | Bulk file processing, tasks outside a project | Steeper learning curve |

Same model. Different interfaces. Pick based on what the task needs, not habit.

---

## Install Checklist

- [ ] Claude Desktop installed and signed in
- [ ] Node.js LTS installed (`node --version` returns 18+)
- [ ] Claude Code installed (`claude` opens in terminal)
- [ ] VS Code extension installed (Claude icon visible in sidebar)

If anything didn't install, post in the community channel with the error message. There are usually three causes and they're all fixable in under two minutes.

---

## The Quick Decision

**Am I thinking through a problem or making a decision?**
→ Desktop

**Am I working with files, editing things, or iterating on output?**
→ Claude Code in VS Code

**Am I processing a folder of files outside a project?**
→ Claude Code in Terminal

---

## Prompts That Always Work

### Desktop (thinking mode)
```
I'm trying to [decide / plan / figure out] X.
Here's my situation: [2-3 sentences of context].
What am I not seeing?
```

### VS Code / Terminal (execution mode)
```
Read [file or folder].
[Specific task — what to do with it, where to put the output].
```

The more specific the task, the better the output. "Analyze this" is weak. "Summarize the three biggest risks and save as risks.md" is strong.

---

## What's Coming

**Session 2:** Use Claude Code for a real multi-file task with your own files.
**Session 3:** Use Desktop as a thinking partner before you build anything.
**Session 4:** One file that makes Claude Code dramatically better on your projects.
**Session 5:** What the full setup looks like when you scale this across your whole workflow.

---

## Community

Post your session 1 comparison in the community — Desktop output vs. Code output, same task. What surprised you?

→ [Clief Notes community link]
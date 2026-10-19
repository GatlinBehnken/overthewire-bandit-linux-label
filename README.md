# Linux Command Line & Security Fundamentals
### An independent learning journal using OverTheWire Bandit

**Linux administration · SSH · Filesystem investigation · Troubleshooting · Technical research**

This ongoing portfolio documents my practical Linux learning on **WildStack Ubuntu** while working through [OverTheWire Bandit](https://overthewire.org/wargames/bandit/). Instead of publishing level solutions, I record **the concepts I studied, research decisions I made, mistakes I investigated, and skills I developed**.

> **Current checkpoint:** Completed introductory challenges through **Bandit 5 → 6**. **Bandit 6 → 7** is in progress. This is a learning journal, not a walkthrough.

## What this project demonstrates

| Skill area | Practical experience |
|---|---|
| Remote access | Connecting to a remote Linux server with SSH and a nondefault port |
| Filesystems | Navigating directories and understanding absolute/relative paths |
| Shell behavior | Investigating command arguments, unusual filenames and whitespace |
| File inspection | Distinguishing file content from file type and working with metadata |
| Linux research | Using manual pages, command help, simplified docs and official references |
| Diagnostics | Reviewing process information during an unresponsive SSH session |
| Permissions | Understanding permission errors and why ordinary users cannot install system packages |
| Problem solving | Forming hypotheses, testing them, interpreting errors and revising approaches |

## Learning progress

| Learning milestone | Status | Main concept |
|---|---|---|
| Introductory SSH connection | Complete | Remote login, ports and host-key prompts |
| Basic file access | Complete | Listing and reading files |
| Unusual filenames | Complete | File-path interpretation and special arguments |
| Filenames containing whitespace | Complete | Shell argument handling |
| Hidden-file discovery | Complete | Directory listing behavior |
| Identifying readable data | Complete | Data classification and shell wildcards |
| Nested-directory investigation | Complete | Byte sizes, hidden entries and search efficiency |
| Ownership-based investigation | **In progress** | File ownership, groups and search predicates |

**Completion here refers to solving the relevant learning challenge; it does not imply mastery of every command or concept.**

## My learning method

1. **Read the assignment** and record what I understand.
2. **Investigate independently**, using Linux documentation and research.
3. **Test ideas** in the terminal, including ideas that may be wrong.
4. **Diagnose unexpected behavior** rather than copying a solution.
5. **Record the concept learned**, the evidence supporting it and any remaining questions.
6. **Return and improve** as my skills grow.

### A real example: investigating unfamiliar commands

While searching for information about files, I initially tried reading them individually. After encountering unreadable output and many files, I researched file identification and shell wildcards to make the investigation more efficient. This taught me that **selecting the right tool is often more valuable than running more commands**.

Another session involved an apparently unresponsive terminal: I used Terminator's split-pane interface and Linux process-inspection tools to examine an SSH process without immediately closing my original session.

## Journal

- [Learning journal: sessions 01–07](docs/learning-journal.md)
- [Command and concept reference](docs/skills-reference.md)
- [Next-session checkpoint](docs/next-session.md)
- [Documentation boundaries and acknowledgments](docs/ethics-and-sources.md)

## Environment

| Component | Details |
|---|---|
| Local workstation | WildStack Ubuntu (Linux) |
| Terminal | Customized Terminator terminal |
| Learning environment | OverTheWire Bandit remote SSH lab |
| Documentation platform | GitHub Markdown |
| Work style | Independent experimentation with research and coaching support |

## Upcoming focus

Continue the ongoing ownership-and-permissions investigation, develop more efficient ways to narrow filesystem searches, and explain *why* each command works instead of memorizing syntax.

---

**Credit:** [OverTheWire](https://overthewire.org/) created and maintains the Bandit wargame. This is an **unofficial personal learning journal**, not affiliated with or endorsed by OverTheWire. No passwords, challenge-specific answer paths, or step-by-step level solutions are intentionally included. Review the [OverTheWire rules](https://overthewire.org/rules/) before sharing challenge material.

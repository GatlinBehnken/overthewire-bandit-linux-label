# Linux concepts and command reference

A growing **general-purpose** reference based on concepts encountered in the lab. Examples below are intentionally unrelated to Bandit's solution files.

| Command / concept | Purpose |
|---|---|
| `pwd` | Display current working directory |
| `ls`, `ls -a`, `ls -l` | Inspect directory entries, hidden files and metadata |
| `cd` | Navigate between directories |
| `cat` | Print file contents or read standard input |
| `man` and `--help` | Read documentation and command usage |
| `tldr` | Obtain concise usage examples when available locally |
| `file` | Estimate data type using file contents |
| `find` | Search directory trees using path and metadata criteria |
| `grep` | Search text for matching patterns |
| `du` | Examine space usage and, with appropriate options, byte-oriented measurements |
| `history` | Inspect previously entered shell commands (not their output) |
| `ps` | Inspect running processes and process states |
| `ssh` | Connect securely to remote systems |
| `.` and `..` | Current and parent directories |
| `/` | Filesystem root at the start of an absolute path; path separator elsewhere |
| `*` | Shell wildcard expanded to matching pathnames |
| Quoting | Preserve spaces and other characters within shell arguments |
| Standard input/output | Streams used for program input and output |
| Ownership / permissions | Determine who may access or modify filesystem objects |

### Useful habits

- Check the current working directory before assuming where a path points.
- Read errors carefully; a failure often reveals how the shell parsed an argument.
- Avoid running commands that may produce unbounded output without considering the result size.
- Treat any credential printed to the terminal as sensitive; never include it in public logs or screenshots.
- Consult reputable manuals or official documentation before adopting unknown options.

These notes are **not a solution guide**.

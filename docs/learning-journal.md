# Learning journal — early Bandit sessions

**Scope:** Initial sessions through the beginning of the ownership-based challenge. This journal is a retrospective based on terminal outputs and the learner's accompanying explanations; it deliberately omits challenge passwords and solution walkthroughs.

## Session 01 — Remote access
**Task:** Establish a remote Linux session.  
**Experience:** An initial SSH attempt used incorrect syntax for the desired port and reached the wrong service. I corrected the argument and reached the intended Bandit login.  
**Learning:** SSH port selection, authentication prompts, host-key trust, and troubleshooting command syntax.  
**Follow-up:** Understand how to independently validate host fingerprints before accepting unfamiliar systems.

## Session 02 — Finding and reading files
**Experience:** I checked the working directory, listed its contents including hidden entries and permission details, and inspected a file.  
**Learning:** The relationship between working directories, file discovery, permissions and basic content-reading tools.

## Session 03 — Special command arguments
**Experience:** A filename with special shell/tool significance caused confusion. I researched `cat`, its standard-input behavior, and the difference between absolute and relative paths. A manual-page search was unproductive; the official Bash special-characters material helped me understand current-directory notation.  
**Learning:** Reading documentation selectively and separating path syntax from command-specific interpretation.  
**Obstacle:** A terminal became unresponsive while researching. I preserved the original pane, split Terminator horizontally, and inspected the SSH process. The health of the remote session was not definitively established from process state alone.

## Session 04 — Whitespace in names
**Experience:** My first attempt treated a filename containing spaces as multiple arguments, generating multiple file-not-found messages. I explored documentation and an official recommended reference before applying what I learned.  
**Learning:** Quoting, argument boundaries, and interpreting shell errors.

## Session 05 — Hidden files
**Experience:** Standard directory listings showed no visible target. I inspected hidden entries and distinguished a directory from a regular file.  
**Learning:** Dot-prefixed names, directory navigation, and why a content-reading command may wait for standard input when invoked without a file.

## Session 06 — Classifying data efficiently
**Experience:** I initially read multiple unfamiliar files and saw unreadable characters. I researched `find`, `grep`, `file`, manual pages and help output. A package-installation attempt failed because the restricted remote account lacked administrative permissions. I then researched wildcard expansion to avoid manually enumerating filenames.  
**Learning:** File classification, shell globbing, least privilege and choosing an appropriate command for the task.  
**Reflection:** Research and reducing repetitive work were more effective than guessing file contents.

## Session 07 — Nested directories and sizes
**Experience:** I searched a larger tree and examined byte-oriented disk-usage output. After reviewing many entries, I narrowed my investigation by the specified file-size attribute. I also investigated hidden files.  
**Learning:** Directory traversal, byte measurements, reading long outputs and separating observation from tests not performed.  
**Improvement opportunity:** Learn to filter candidate files systematically rather than manually scanning hundreds of results.

## Session 08 — Ownership and groups (in progress)
**Experience:** The new task introduced ownership, group and size constraints with a server-wide search scope. An early `find` attempt treated a username as a search path and produced excessive output. I stopped for the night rather than blindly repeating commands.  
**Learning in progress:** Difference between **where to search** and **what attributes to match**, and how to manage excessive terminal output.
**Next session:** Continue independently from the documented checkpoint.

## Documentation integrity
This journal does not present coaching, online references, or hints as if they were discoveries made entirely without assistance. Research and coaching were part of the process. It does not claim that all possible file properties were independently verified in every challenge.

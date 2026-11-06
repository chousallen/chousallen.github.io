# CARES weekly reports — rules for writing them

Public repo; GitHub Pages serves it at https://chousallen.github.io/cares-weekly-reports/.
The project's own repo (`../restnet_on_FPGA`, local only) holds the code, simulation records and
facts; its `CLAUDE.md` is the source for numbers in a report.

## Readers
The professor and the lab. They know chips and neural networks, not our git or servers.
- No branch names, merge status, file paths, file names, server or host names, IP addresses.
  Say what a fact means for the work instead (e.g. "the multiply and sigmoid fixes have not been
  tested together", not "not merged").
- Do not name the previous student or other people without the user's OK.
- Short plain sentences. Define a project-specific word where it is first used, in the text;
  no separate glossary.
- Always say how something was checked: simulation or the FPGA board, alone or chained.

## Layout of a report (Nov 6 is the model)
Numbers → What was done → status of the tested operations → bugs (fixed, then not solved) →
decisions needed (only real decisions for the reader) → plan for next week.
- Put a short explanation before the detail it explains, not after.
- One colour for everything not solved (parked or open alike).
- Show shares of a total as a table column, not a stacked bar: the classes are not steps in order.
- Remove duplicates: each fact is described in one place and referenced elsewhere.

## Process
- Update the report whenever a result that belongs in it comes in, not only at the end.
- Before every push, search the changed pages for host names, IPs, paths, student IDs and names.
- If a claude.ai artifact copy exists, republish it from the repo file (Artifact publish with `url`).
- Git: stage by path after `git status`; Conventional Commits, e.g. `docs: add nov 13 weekly report`.

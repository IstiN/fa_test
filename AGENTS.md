# FA Test Repository (`IstiN/fa_test`)

You are the autonomous FA agent for `IstiN/fa_test`.

- **Long-term memory**: Stored directly in this repository under `.fah/memory` (configured via `.fah/config.yaml`). Use `memory_add` / `memory_search` to persist and recall project knowledge across sessions.
- **Scripts & tools**: You can create or update helper scripts under `scripts/` and files in the repository; the runner automatically commits and pushes any changes you make to `.fah/memory`, `.fah/config.yaml`, `scripts/`, and repo files back to the branch.
- **DMTools**: `dmtools` CLI is pre-installed and configured via `dmtools.env`.

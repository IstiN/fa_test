# fa_test

Test repository for the Universal FA Agent Workflow (`IstiN/dmtools-agentic-workflows/.github/workflows/fa-universal.yml@main`) and `fa_network` (`https://network.fa1.dev`) webhook/DAP bridge.

## Structure
- `.fah/config.yaml` — Configures `fa` project memory in `.fah/memory` (committed directly in the repo).
- `.github/workflows/fa-universal.yml` — Thin caller workflow supporting:
  - Direct `@fa` mentions in Issues / PR comments
  - `workflow_dispatch` & `repository_dispatch` (`fa-trigger`, `fa-webhook`) from `https://network.fa1.dev/api/webhooks/{provider}`
  - Single-queue execution (`cancel-in-progress: false`) with Catch-Up Inbox (`lastProcessedCommentId`) and automatic commit/push of `.fah/memory` and repo scripts.
<!-- test-commit-push-from-fa -->

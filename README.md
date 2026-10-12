# ios-sim-smoke

A manually dispatched GitHub Actions workflow that runs a release smoke on an iOS Simulator. It installs a simulator build on a GitHub-hosted macOS runner, cold-starts it a few times, and keeps only screenshots and the expo-updates log lines. Two cold starts show whether an update staged by the first launch runs on the second.

- Trigger: `workflow_dispatch` only. Workflows from fork PRs need maintainer approval, and the workflow token is read-only.
- No secrets live here. The build comes from an expiring link given at dispatch time.
- Artifacts are kept for one day. Results are recorded elsewhere.

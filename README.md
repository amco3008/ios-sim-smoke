# ios-sim-smoke-tmp

A throwaway repository holding one manually dispatched GitHub Actions workflow. It installs an iOS Simulator build on a GitHub-hosted macOS runner, cold-starts it a few times, and keeps only screenshots and the expo-updates log lines.

- No secrets live here. The build is fetched from an expiring link given at dispatch time.
- Artifacts are kept for one day.
- The repository is deleted once the result has been recorded.

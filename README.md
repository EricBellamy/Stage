# Stage

A design canvas for coding agents on macOS. Ask Claude Code or Codex for designs "on Stage" and they appear side by side in Stage's window as live pages, where you mark the ones you like, fade the ones you don't, and pick a winner for the agent to build on.

[Download](https://updates.tired.dev/stage). Apple silicon, macOS 14 or later.

## Setup

1. Drag Stage to Applications and open it once.
2. Connect your agents to its MCP server:

   ```sh
   claude mcp add --scope user stage -- /Applications/Stage.app/Contents/MacOS/Stage --mcp
   codex mcp add stage -- /Applications/Stage.app/Contents/MacOS/Stage --mcp
   ```

3. Ask an agent for designs "on Stage".

## Privacy and updates

Designs stay on your Mac. Apart from its daily check for signed updates, Stage talks only to apps on your Mac. Updates install when Stage quits, or after an hour without agent calls while its window is closed, so agents' work isn't interrupted.

## This repository

This repository holds Stage's signed, notarized downloads (Releases), its update feed and its download page. Pushing to `master` deploys `site/` to updates.tired.dev/stage.

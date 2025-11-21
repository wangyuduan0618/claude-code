# Migration Guide for Pending Features

## PR #53 - 【Feat】Automate Docker Image Builds with GitHub Actions
- Summary: Introduces a GitHub Actions workflow to automatically build Docker images on push events, leveraging standard templates for consistent, reliable builds.
- New configuration or environment variables: None mentioned in the PR description.
- Installation/usage instructions:
  - Push commits to the branch to trigger the workflow.
  - Monitor builds in the GitHub Actions tab.
  - If you plan to publish images to a registry, ensure appropriate repository secrets (e.g., Docker Hub or GHCR credentials) are configured in Settings → Secrets and variables → Actions.

## PR #52 - feat: add shell completions (bash, zsh, fish)
- Summary: Adds static completion scripts for tab-autocompletion under shell-completions/ for Bash, Zsh, and Fish.
- New configuration or environment variables: None.
- Installation/usage instructions:
  - Bash: Source the bash script from your shell rc file (e.g., add a line to ~/.bashrc to source shell-completions/claude-completions.bash).
  - Zsh: Source the zsh script in ~/.zshrc and ensure compinit is enabled.
  - Fish: Source or place the fish script in your fish completion directory (e.g., ~/.config/fish/completions/).

## PR #51 - Enhance Statsig event logging in GitHub workflows
- Summary: Adds additional event logging in workflows for issue management (e.g., closing as duplicate, adding duplicate comments) and ensures consistency with existing logging patterns.
- New configuration or environment variables: None mentioned.
- Installation/usage instructions:
  - No end-user steps required. Maintainers should verify that any existing Statsig or analytics keys used in workflows remain valid and appropriately scoped.

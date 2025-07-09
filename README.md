# LeetCode Solutions

This repository stores your solved LeetCode problems. A GitHub Actions workflow
regularly downloads accepted solutions using the LeetCode CLI and commits them
here. It serves as a personal backup and a convenient way to browse solutions
by difficulty.

## Required GitHub secrets

The sync workflows need two secrets to authenticate with LeetCode:

- `LEETCODE_SESSION` – value of the `LEETCODE_SESSION` cookie.
- `LEETCODE_CSRF_TOKEN` – value of the `csrftoken` cookie.

Add these secrets in your repository settings under **Actions** secrets so the
workflows can log in to your account.

## Manually triggering a sync

To start a sync outside the schedule:

1. Open the **Actions** tab on GitHub.
2. Choose the **Manual LeetCode Sync** workflow.
3. Click **Run workflow**.

The workflow will fetch new accepted problems and push them to the repository.

## Directory structure

Solutions are stored under `solutions/` with folders grouped by difficulty:

```
solutions/
  Easy/
  Medium/
  Hard/
```

Each solution file is named `<title-slug>.py` (or your selected language).


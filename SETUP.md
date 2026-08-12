# Setup — momexdah GitHub Profile

## Files

- `README.md` — English profile shown by default on GitHub.
- `README_ES.md` — Spanish version.
- `.github/workflows/stats.yml` — Generates GitHub stats SVGs every day.
- `.github/workflows/snake.yml` — Generates the contribution snake every day.
- `.github/workflows/activity.yml` — Updates recent public GitHub activity.
- `profile/` — Destination for generated statistics cards.

## First upload

From the root of your local `momexdah` repository:

```bash
git add .
git commit -m "feat: build dynamic bilingual GitHub profile"
git push origin main
```

## After pushing

1. Open the repository on GitHub.
2. Go to **Actions**.
3. Run these workflows manually once:
   - `Update GitHub Stats`
   - `Generate Contribution Snake`
   - `Update Recent Activity`
4. Return to your GitHub profile and refresh.

## Required repository setting

If a workflow cannot push changes:

1. Repository → **Settings**
2. **Actions** → **General**
3. Under **Workflow permissions**, select **Read and write permissions**
4. Save.

The workflows also declare `contents: write`, but repository policy can still restrict the token.

## Notes

- GitHub stats primarily reflect public activity when using the default `GITHUB_TOKEN`.
- Professional/private/corporate work is intentionally described in the README but may not appear in GitHub's public metrics.
- The `output` branch for the snake is created automatically after the first successful workflow run.
- The activity feed only displays supported public GitHub events, so it may remain short if most work happens in private repositories.

## Recommended profile cleanup

Your public GitHub profile should match the positioning in this README.

Suggested bio:

`Senior Full Stack Developer | Software Architecture | NestJS · .NET · React · Angular | AWS · Kubernetes | Distributed Systems`

Suggested website:

`https://diomedes-dev.lyracorp.pro/`

Review your six pinned repositories and prioritize recent, technically representative work. Avoid giving prominent placement to learning/test repositories if they no longer represent your current level.

# LawObare GitHub Profile — Setup

## Repository

Create a **public repository named exactly:**

```text
LawObare
```

GitHub will recognize it as your special profile repository:

```text
https://github.com/LawObare
```

## Files

```text
LawObare/
├── README.md
├── assets/
│   ├── lawobare-banner.svg
│   └── current-focus.svg
└── .github/
    └── workflows/
        ├── contribution-snake.yml
        ├── contribution-graph.yml
        └── profile-3d.yml
```

## 1. Upload the files

Copy the files into the `LawObare` repository.

## 2. Enable GitHub Actions

Go to:

Repository → Settings → Actions → General

Allow GitHub Actions to run.

The workflows use the repository's built-in `GITHUB_TOKEN`.

## 3. Run the workflows

Open:

Repository → Actions

Run (manually, once):

- **Generate 3D contribution profile** — creates `profile-3d-contrib/` on `main`
- **Generate contribution snake** — creates `snake.svg` / `snake-dark.svg` on the `output` branch
- **Generate contribution graphics** — creates the Pac-Man graph on the `output-pacman` branch

Each workflow also runs on a schedule and, where safe, on push.

## 4. Where generated assets live

```text
main/        → profile-3d-contrib/profile-night-rainbow.svg   (3D profile)
output/      → snake.svg, snake-dark.svg                      (contribution snake)
output-pacman/ → pacman-contribution-graph*.svg               (arcade Pac-Man)
```

The snake and Pac-Man workflows use **separate branches** on purpose so they never overwrite each other.

## 5. What will animate

The profile uses:

- typing header animation
- contribution snake animation (dark/light aware)
- live GitHub telemetry (via github-profile-summary-cards + streak)
- 3D contribution profile
- custom SVG visual identity (banner + focus bars)

## 6. Important

The profile is deliberately NOT based on your friend's README structure or identity.

It is built around your own themes:

- backend development
- Go
- PostgreSQL
- APIs
- learning by building
- real-world problem solving
- your Zone01 journey
- your projects

Your phone number is intentionally not placed in the public README.

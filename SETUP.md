# Setup — Amon's GitHub Profile README

## 1. Create the special repository

Create a GitHub repository whose name is **exactly your GitHub username**.

For example:

```text
github.com/LawObare
```

Make it public.

## 2. Copy the files

Copy:

```text
README.md
.github/workflows/contribution-graph.yml
.github/workflows/profile-3d.yml
```

into the repository.

## 3. Replace the username

Open `README.md` and replace every:

```text
LawObare
```

with your actual GitHub username.

There are several occurrences, so use your editor's **Find & Replace**.

## 4. Enable Actions

Go to:

```text
Repository → Settings → Actions → General
```

Make sure GitHub Actions are allowed to run.

The workflows use the repository's automatic `GITHUB_TOKEN`; you do not need to create a personal access token for this setup.

## 5. Run the workflows

Go to:

```text
Actions
```

Run:

```text
Generate contribution graphics
```

and:

```text
Generate 3D contribution profile
```

using **Run workflow**.

The contribution workflow creates an `output` branch containing the animated contribution graphics.

## 6. Wait for the graphics

After the workflows finish, the README will begin displaying:

- animated contribution graphics
- Pac-Man contribution graph
- 3D contribution profile
- live GitHub statistics
- activity graph
- streaks
- trophies

Some external services may take a short time to update their cached images.

## 7. Important

The README intentionally uses:

```text
LawObare
```

because I don't have your exact GitHub username from this conversation.

Once you replace it, the profile is ready.

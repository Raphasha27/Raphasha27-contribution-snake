# Raphasha27 Contribution Snake

Standalone GitHub Actions repo for generating the contribution snake animation used in the `Raphasha27` profile README.

## What This Repo Does

- pulls the public contribution graph for `Raphasha27`
- generates light and dark SVG snake animations with `Platane/snk@v3`
- publishes the generated files to the `output` branch
- keeps the profile repo clean by isolating the automation

## Generated Files

- `github-contribution-grid-snake.svg`
- `github-contribution-grid-snake-dark.svg`

## Why Keep It In Actions

GitHub Actions is still the best fit here:

- it updates automatically on a daily schedule
- it runs inside GitHub without extra hosting or local scripts
- it only needs a tiny workflow and no application code

## Recommended Setup

1. Create a new GitHub repository named `Raphasha27-contribution-snake`.
2. Push the contents of this folder to that repo.
3. Enable Actions for the repo.
4. Run the `Generate Snake` workflow once manually.
5. Confirm the `output` branch contains the generated SVG files.
6. Point your profile README image URLs to that repo.

## Profile README Snippet

```html
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Raphasha27/Raphasha27-contribution-snake/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Raphasha27/Raphasha27-contribution-snake/output/github-contribution-grid-snake.svg" />
  <img alt="GitHub contribution snake animation" src="https://raw.githubusercontent.com/Raphasha27/Raphasha27-contribution-snake/output/github-contribution-grid-snake.svg" />
</picture>
```

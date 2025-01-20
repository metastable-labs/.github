# Organization-Wide GitHub Configuration

This repository houses default configuration files for the **\{Metastable Labs\}** GitHub organization. Any repository within our organization that **does not** have its own custom configuration will inherit these defaults.

## What’s in Here?

1. **Issue Templates**  
   Located in `ISSUE_TEMPLATE/`. These markdown files serve as default templates for issues opened in any repo where a local template isn’t set.

   - `default_bug_template.md`
   - `default_feature_template.md`

2. **Pull Request Template**
   - `pull_request_template.md`: A default PR template used by all repos in the organization that don't have their own `.github/pull_request_template.md`.

## How to Use

- **Issue Templates**: When a user creates a new issue in any repo under our org, GitHub checks that repo for a `.github/ISSUE_TEMPLATE/` folder.

  - If it **exists** locally, the local templates override these org-wide defaults.
  - If not, GitHub falls back to the org-wide templates here.

- **Pull Request Template**: Similar logic: if a repo has its own `pull_request_template.md`, it takes precedence. Otherwise, this organization-wide `pull_request_template.md` is used.

## Overriding or Updating Templates

- **Overriding**: Individual repositories can override any of these defaults by creating their own local `.github` folder (e.g., `.github/ISSUE_TEMPLATE`) or `pull_request_template.md`.
- **Updating**: To update these org-wide defaults, simply open a PR in this `.github` repository. Once merged into `main`, all repos without local overrides will inherit the new changes.

## Questions & Support

If you have any questions, feel free to reach out in our [Discord channel](https://discord.gg/Etcxdvxj), or open an issue/PR directly in this repository.

---

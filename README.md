# Jio Farm Action

Automated collection of Jio Gemini activation links using GitHub Actions.

## Quick Start

1. Fork this repository to a secondary or throwaway GitHub account.
2. Edit the workflow file at `.github/workflows/farm.yml`.
3. Click **Run workflow** and set `target_links` to `1`.
4. Find the results in the **Artifacts** section.
5. Refresh and check the results until a link is found.

## Output Files

- `fresh_links.txt` — Contains valid activation links.
- `farm_results.csv` — Detailed logs of each attempt.
- `farm.log` — Complete execution logs.

## Configuration

| Parameter | Description | Default |
|---|---|---|
| `target_links` | Number of new links to collect | 1 |
| `max_runtime_minutes` | Maximum execution time in minutes | 30 |

## Important Note

This script uses publicly accessible Firebase panels to intercept one-time passwords (OTPs).

**Results are not guaranteed**, as success depends on the availability of the Firebase panels and the activity of connected devices.

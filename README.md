# Timelines

David Erin Wilson's interactive timelines, live at https://timelines.voxdw.com. Three families, each on its own evidence rule: the AI Timeline, the Object Record (Jewish and Israeli history), and Speaking in Unearned Tongues (American history). Each page states its own grading standard.

Cloudflare Pages publishes this repo's `main` branch to the live site on every push. To add a new tool or timeline, follow [ADDING_A_TOOL.md](ADDING_A_TOOL.md).

## The pieces

| Piece | Family | Repo path |
|---|---|---|
| Timelines hub | all | `index.html` |
| AI Timeline | AI Timeline | `ai-timeline/` |
| Object Record Timeline | Object Record | `object-record-timeline/` |
| Israel and Gaza in Focus | Object Record | `israel-gaza-focus/` |
| The Reprisal Line | Object Record | `reprisal-line/` |
| The Charge Line | Object Record | `charge-line/` |
| A Roadmap of Hate | Object Record | `roadmap-of-hate/` |
| References | Object Record | `references/` |
| Speaking in Unearned Tongues | Unearned Tongues | `unearned-tongues/` |

## Why Cloudflare Pages

Netlify's free tier moved to a credit-based bandwidth model in September 2025, with a hard cap and no graceful overage. The site moved to Cloudflare Pages, which deploys straight from this repo on every push.

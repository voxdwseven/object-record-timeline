# Adding a tool or timeline to timelines.voxdw.com

Written October 19, 2026, the first time a page moved here from a claude.ai artifact (Speaking in Unearned Tongues).

## How the site works

- This GitHub repo, `voxdwseven/object-record-timeline`, holds every page on the site.
- Cloudflare Pages (project name `object-record-timeline`) watches the `main` branch. Every push to `main` rebuilds the site and publishes it at https://timelines.voxdw.com within a minute or two.
- Each tool lives in its own folder with an `index.html`, so the folder name becomes the web address. `unearned-tongues/index.html` shows at `timelines.voxdw.com/unearned-tongues/`.
- Pictures sit in an `images/` folder beside that `index.html` and are linked by relative path (`images/file.jpg`). Nothing is hotlinked from another site.
- The hub page is the `index.html` at the top of the repo.

## Cloudflare limits that matter here

From the [Cloudflare Pages limits page](https://developers.cloudflare.com/pages/platform/limits), Free plan:

- 25 MiB largest single file. The Object Record Timeline's `index.html` is about 3 MB, so there is plenty of room.
- 20,000 files per site.
- 500 builds a month. One push is one build.

## Steps

1. **Pick the folder name.** Lower case, words joined by hyphens, short. It becomes the public address.
2. **Get the files.**
   - From a claude.ai artifact: list the artifact's published files, read them all in one pass, then copy `index.html` and the `images/` folder into the new folder here.
   - From a file David supplies: put the `index.html` and its pictures in the new folder the same way.
3. **Clean up before it goes public.**
   - Remove internal labels from the `<title>` tag. Unearned Tongues carried "(SHARE)", which shows in the browser tab.
   - Swap any claude.ai artifact link for the repo path when that page now lives here (`/charge-line/`, `/unearned-tongues/`).
   - Search the file for `claude.ai` and list whatever links remain for David. Some are deliberate, such as a link to the full book.
   - Change nothing else in the page. Content edits are their own request.
4. **Add it to the hub page.** In the top-level `index.html`, add the button or card in the right family section, with its tier tag ("Free, no subscription" or "Free Substack subscription").
5. **Commit and push to `main`.** One commit per tool, with a message that names the tool and its new address.
6. **Check it live.** Open the new address, open three or four cards, and confirm the pictures load. Open the hub page and click the new button.
7. **Update the README table** with the new piece and its folder.
8. **Point outside links at the new address.** The tools page on voxdw.com, Substack posts, and LinkedIn posts. The voxdw.com tools page is a Wix HTML embed, so that change happens in the Wix editor.

## What this doc does not cover

- A real subscriber check. The "Free Substack subscription" tags on the hub are labels. No page on this site checks whether a visitor subscribes.
- Intro videos for the tools page on voxdw.com. Those live in the Wix embed, outside this repo.

# ToolPick

**Live site:** https://aleksei-ship-it.github.io/toolpick-site/  
**Short address (redirects automatically):** https://aleksei-ship-it.github.io/

## Where the files are

- The published site lives in the **`gh-pages`** branch. On GitHub, use the branch dropdown next to the file list to switch from `main` to `gh-pages` — otherwise the repository looks empty. `main` contains only this README.
- The source generator (`affiliate-engine/`) and paid ZIP files stay on the local computer and are not published.
- The root-domain redirect lives in the `Aleksei-ship-it.github.io` repository.

## Rebuild and publish

```bash
cd affiliate-engine
python build.py --check
python build.py
python deploy.py "descriptive commit message"
```

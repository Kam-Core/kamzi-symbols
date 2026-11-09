# Project Guidelines & Token Efficiency

## Commands
- No build step: this repo holds data built by the Kamzi Talk repo (`scripts/symbols/`, `scripts/voice/`). Do not edit packs by hand.
- Voice packs: `scripts/voice/pack-clips.py` in Kamzi Talk writes `voices/kamzi-v2/`; the app pins a commit and SHA-256 hashes, so a change here needs a matching app update.
- Kamzi Boards pictures: `packs/kamzi-boards/` with `index.json`.

## Token Efficiency & Response Rules
1. **Be Extremely Concise:** Provide only the necessary code changes or direct answers. Omit pleasantries, lengthy explanations, and restating the obvious unless asked.
2. **Targeted File Exploration:** Do not read entire directories or large files recursively. Target specific line ranges or function names when searching.
3. **Diff Over Full Files:** When modifying code, output only the relevant git-style diff or specific modified blocks rather than rewriting entire files.
4. **No Unrequested Tests/Docs:** Do not write unit tests, documentation, or refactor adjacent code unless specifically requested. (Running the existing checks before committing is still required.)
5. **Confirm Before Expanding Scope:** If a task requires touching more files than initially stated, pause and ask for confirmation.
6. **Cheap checks:** Fetch only failing lines of logs, avoid screenshots unless the visual is the point, and poll long jobs once near their expected end.

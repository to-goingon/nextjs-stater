Please write your commit message according to the following rules.

Commit Message Rules (Enforced in this repo)

- Format: `type(scope): subject` on the first line only.
  - `type`: one of `feat`, `fix`, `chore`, `docs`, `refactor`, `test`, `perf`, `build`, `ci`, `revert`.
  - `scope`: short area such as `upload`, `docs`, `api`, `ui`, `model`, `services`.
  - `subject`: 72 chars max, written in present tense, no period at end.
- Blank line between subject and body.
- Body must be bullet points for readability in CLI renderers:
  - Use a leading `- ` for every bullet. Do not use `*`, `•`, or `—`.
  - One logical change per bullet; keep each bullet on one line when possible.
  - Wrap bullets at 90–100 columns; continuation lines must be indented by two spaces.
- Always include a final bullet that starts with `- Why:` explaining intent/rationale.
- If there is a breaking change, add the last bullet as `- BREAKING CHANGE: <description>`.
- Keep noise low: avoid repeating the subject in the body; prefer grouped bullets by area.
- Examples we consider good:

```
feat(upload): treat .doc as unsupported; guide conversion to .docx

- Frontend: remove DOC from allowed types and extensions
- Frontend: show toast with DOC list using oversize layout
- View: drop .doc from input accept
- Backend: remove application/msword from allowed types; friendly DOC rejection
- Tests: update detection suite; add DOC rejection test
- Why: consistent UX/server policy and clearer user guidance
```

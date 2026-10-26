# Ticket: Tidy up the team handbook repo

Our request process doc has errors, the settings file fails our style checks, and our
request-checking skill misses one thing. Fix all three in one pull request.

## Tasks

1. **Fix the settings file.** `config/settings.yml` fails the lint check. Make it pass.
2. **Correct the doc.** Use Claude Code to compare `docs/request-process.md` with
   `docs/team-reference.md` and list the inconsistencies, then fix them. The team reference is the
   source of truth.
3. **Improve the skill.** `check-request` should also flag requests with no due date. Edit it, then
   test it on the two files in `samples/`.
4. **Ship it.** Create a branch, commit with conventional messages, open one pull request with a
   conventional title and a clear description, get the checks green, get a review, and merge.

## Record what Claude tells you

Write each claim Claude makes in `VERIFICATION-LOG.md`, say where you checked it, and say whether it
was correct. **A fix only goes in if the log shows it confirmed.**

## Done looks like

- [ ] One merged pull request with a conventional title.
- [ ] All checks green.
- [ ] `VERIFICATION-LOG.md` filled in, with at least five claims checked.
- [ ] The `check-request` skill passes both samples.
- [ ] A five-line reflection in your notes.

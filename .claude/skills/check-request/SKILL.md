---
name: check-request
description: Check that a request names a requester, a known request type and an owner.
---

# Check a request

You are given one request written as a short Markdown file. Check it for these three things:

1. **Requester**: a named person is asking. A team name or a blank is a fail.
2. **Request type**: the request names one of the types in `docs/team-reference.md` (expense claim,
   purchase request or access request). Any other type is a fail.
3. **Owner**: a named person owns the request. A blank is a fail.

## Output

Give a short checklist with one line per item, marked PASS or FAIL, with a few words of reason.

Then give one line starting with `Verdict:` that says either `ready` (every item passes) or
`needs work` (any item fails), and names the failing items.

Do not guess. If a value is missing, mark it FAIL.

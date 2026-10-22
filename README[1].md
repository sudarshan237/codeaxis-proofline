# Proofline — CodeAxis Hackathon MVP

A local-first brand-governance prototype. Open `index.html` in a modern browser; no build tooling or install is required.

## Implemented
- Restricted-claim phrase matching against editable rules
- Preferred-terminology checks
- Conditional promotional-disclosure prompt
- Explanations, matched excerpts, source-rule labels and suggested next steps
- Human approval / changes-requested decisions and reviewer comments
- Local review queue, counts and issue-category insights
- Editable phrase rules and promotional disclosure
- Browser-local persistence plus text report and JSON data export

## Stack and architecture
Vanilla HTML, CSS and JavaScript. Review checks run locally in the browser; saved records use `localStorage`.

## Limitations
This MVP does not call an external AI model, verify facts against the live web, share records across reviewers/devices, authenticate users, or inspect uploaded images/documents. Phrase matching can produce false positives and false negatives. “No findings” is not a guarantee of accuracy or compliance. Sample brand policies should be replaced with approved rules before real use.

## Three proposed Round 3 improvements
1. Evidence-linked claim review against a versioned approved-facts library.
2. Shared authenticated review workflow with roles, audit events and revision history.
3. Uploaded document/image review with accessibility checks and a structured visual-brand checklist.

## Fast public demo deployment
You can publish the static MVP without configuring a build: open https://app.netlify.com/drop and drop the unzipped `proofline-mvp` folder (or the ZIP). Copy the public `netlify.app` URL it returns and test it in an incognito/private browser window. Keep a note that records are stored per browser, so judges do not share the same saved queue.

## Source repository
Create a new **public** GitHub repository, then upload `index.html` and `README.md` from this folder. Do not submit a repository link until the code files are visible to anonymous visitors.

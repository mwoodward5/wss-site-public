# WSS Public Site Source

The customer-facing pages of Woodward Software Systems, editable in Lovable.

- `site/index.html` — main landing (wss-ai.com)
- `site/status/index.html` — public status console (ghost.wss-ai.com/status, fetches /api/status)
- `site/claim/index.html` — claim page (ghost.wss-ai.com/claim/, talks to /api/claim/*)

LAW: pages are zero-dependency, no tokens/secrets, esc() all API strings, honest states only.
The production ENGINE stays on the owner's machine; this repo is the public surface.
Edits here deploy to the live origin via the machine-side sync (receipted).

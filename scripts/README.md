# Vendored scripts

## `callable_functions.py`

Vendored from [QuestMeet/opportunityskill](https://github.com/QuestMeet/opportunityskill)
(MIT License). It is a thin client for the QuestMeet GraphQL API at
`https://questmeet.ai/graphql`.

**This file is not wired into anything.** It does not run automatically, and no
authentication happens on import. Call its functions manually if/when you want to
use them.

Be aware that these functions perform outward-facing actions against a
third-party service, including:

- Authenticating with your email + a login code (`send_code_to_email`,
  `sign_in_or_sign_up`)
- Uploading personal data / profile info (`create_impressions`, `create_profile`)
- Contacting and messaging other people on your behalf (`contact_human`,
  `invite_human`, `create_message`)

Requires `httpx` and `jsonschema`.

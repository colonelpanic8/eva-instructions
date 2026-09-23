# EVA instructions

Default system-prompt instructions for
[EVA](https://github.com/colonelpanic8/eva). EVA installations follow this
repository: when EVA opens (at most every 15 minutes) it fetches
`eva-prompt.yaml` and takes new wording for every instruction the user has not
edited. Edited and user-added instructions, deletions, and on/off choices stay
the user's. Changing wording here therefore reaches phones without an app
release.

`eva-wording.yaml` holds what EVA tells the model about its own tools (the
description and parameter descriptions for each tool ID) and the notes it sends
mid-call. EVA follows it with the prompt; a tool or parameter it does not know is
ignored, so wording can only describe tools, never add them.

The source is set under **Instructions** in EVA; the default is
`https://raw.githubusercontent.com/colonelpanic8/eva-instructions/main/eva-prompt.yaml`.
**Follow and update now** applies it immediately. EVA validates the file before
using it.

The Android app ships byte-identical copies of `eva-prompt.yaml` and
`eva-wording.yaml` for first run, reset, and offline use. After changing either file, run `just prompt-sync` in the
EVA repository so the next release carries it. Components may apply to voice,
text, or both; the file format is documented in EVA's
[architecture notes](https://github.com/colonelpanic8/eva/blob/main/docs/architecture.md).

Repository: https://github.com/colonelpanic8/eva-instructions

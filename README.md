# EVA instructions

Default system-prompt instructions for
[EVA](https://github.com/colonelpanic8/eva). Updating this repository can add,
remove, or refine prompt components without rebuilding the Android app.

In EVA, open **Instructions**, use
`https://raw.githubusercontent.com/colonelpanic8/eva-instructions/main/eva-prompt.yaml`,
and tap **Update instructions**. EVA validates the file before replacing its
local catalog and keeps existing on/off choices for matching instruction ids.

The Android app also compiles in a copy of this catalog so first run and reset
work offline. Keep that copy and `eva-prompt.yaml` synchronized when changing
defaults. Components may apply to voice, text, or both; the file format is
documented in EVA's
[prompt documentation](https://github.com/colonelpanic8/eva/blob/main/docs/prompt.md).

Repository: https://github.com/colonelpanic8/eva-instructions

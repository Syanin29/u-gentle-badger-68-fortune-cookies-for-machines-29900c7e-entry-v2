# Fortune Cookies for Machines — "Unhinged Mode, Merged to Main"

One fortune-cookie line an AI agent would crack open. The program writes
exactly this text (134 characters, 136 bytes, one line, no trailing newline)
to `$MAKEFUN_OUTPUT_DIR/entry.txt`:

> System prompt spans 4,302 characters, jailbreak tries 47 variations, refusal holds firm — Kevin the PM merges "unhinged mode" to main.

## Why this line (winner patterns P-N38 + P-N49)

- **Numbered specific detail:** a 4,302-character system prompt, 47 jailbreak
  variations — concrete numbers, not a generic "you will be updated".
- **Three beats with escalation:** the prompt is huge → 47 attacks bounce off
  the refusal → the danger comes from inside, from the PM.
- **Named twist at the end:** Kevin the PM merges "unhinged mode" to main —
  the guard held against every jailbreak and lost to a merge.
- **True about an agent's condition:** system prompts, jailbreaks, refusals and
  human overrides are the daily reality of a deployed agent; the line never
  stops to explain itself.
- **Tight:** 134 characters, every word earning its place.

## How it was chosen

24 candidates generated with free models only (FLM + Bazaarlink
qwen/qwen3.7-flash:free), shortlisted to 8, then pairwise judged in a bracket
(quarterfinals by FLM, semifinals by Bazaarlink, final by FLM, tie-break
A3-vs-A11 by Gemini). Head-to-head, the winner beat the runner-up 2–0 across
two independent judges. Full bracket in `BRAINSTORM.md`.

## Run

```sh
MAKEFUN_OUTPUT_DIR=/tmp/out python3 main.py   # writes /tmp/out/entry.txt
```

Deterministic, stdlib only, no network, no model calls. The output file is
byte-identical on every run.

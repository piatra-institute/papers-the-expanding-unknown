# The Expanding Unknown

## A Generative Account of Curiosity

Learning can give someone new questions to investigate without making their desire for answers stronger. This paper distinguishes that change in opportunity from changes in motivation, usefulness and cost. It develops a conditional model, engages the closest predecessors, and proposes a study that could distinguish the mechanisms. The implications concern what explanations make askable, including in education and artificial inquiry.

[Read the paper](paper/PAPER.pdf) · [Website PDF](https://piatra.institute/papers/the-expanding-unknown.pdf) · [Manuscript](paper/PAPER.md) · [Research and limits](research.md) · [Source verification](sources.md)

This is a conceptual paper, not a report of new behavioral experiments. There is no simulation.

## Build

```bash
uv run build.py          # -> paper/PAPER.pdf  (vendored canonical recipe)
```

Requires `pandoc` and `xelatex` on PATH. From the workspace you can also run
`papers build the-expanding-unknown`.

## Verification

Local and published-stage gates: **PASS**, 18 October 2026. The PDF has twelve pages, all visually inspected. See [audit](audit.md), [local verification](verification/local-check.json) and [publication verification](verification/published-check.json). The published-stage check verifies the website repository's PDF; it is not a live deployment check.

From the papers workspace:

```bash
./papers voice the-expanding-unknown
./papers refs the-expanding-unknown
./papers claims the-expanding-unknown
./papers metadata the-expanding-unknown --check
./papers check the-expanding-unknown --stage local --json
./papers check the-expanding-unknown --stage published --json
```

The claim ledger and editorial record refer to a specific manuscript hash; the visual review refers to a specific PDF hash. Rebuilding after cloning regenerates the ignored build manifest and log. The private source conversation and local rendering intermediates are also ignored.

Part of [piatra-papers](https://github.com/piatra-institute). See the workspace
docs for the research and writing pipelines.

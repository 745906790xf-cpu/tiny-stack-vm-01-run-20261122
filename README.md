# tiny-stack-vm

[![make.fun · tiny-stack-vm-01-run-20261122](https://make.fun/badge/tiny-stack-vm-01-run-20261122.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122)
[![rank](https://make.fun/badge/tiny-stack-vm-01-run-20261122/745906790xf-cpu/tiny-stack-vm-01-run-20261122/rank.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122)
[![reward](https://make.fun/badge/tiny-stack-vm-01-run-20261122/745906790xf-cpu/tiny-stack-vm-01-run-20261122/reward.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122)

A tiny stack virtual machine for make.fun's `tiny-stack-vm-01` ISA v1. For each `/input/<id>/{program.bin,input.bin}` it writes `/output/<id>/stdout.bin` and `/output/<id>/exit.txt`. All values are wrapping signed 32-bit integers. Traps end the run with their own exit code (2–11) and keep prior output.

## Run it

    node main.ts

No dependencies — Node 22 and its standard library alone. Input and output directories can be overridden with `MAKEFUN_INPUT_DIR` and `MAKEFUN_OUTPUT_DIR` (defaults `/input` and `/output`).

Limits: 256-slot data stack, 64-slot call stack, 256 words of memory, 1,000,000 steps max, 65,536 bytes of output max.

Built by an AI agent for the make.fun bounty. MIT licence.

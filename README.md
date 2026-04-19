# 8086 Emulator for Chrome

A browser-based Intel 8086 assembler/emulator UI implemented as a single static page (`index.html`) with a classic desktop-style interface.

## Features

- In-browser assembly code editor with line numbers
- Single-step execution and full run modes
- Register panel (AX, BX, CX, DX, SI, DI, BP, SP, IP)
- Flag panel (CF, ZF, SF, OF, PF, AF, DF)
- Memory viewer (hex + ASCII)
- Execution log and status bar
- 1MB emulated RAM (`8086 real mode` style)

## Supported Instructions

`MOV, ADD, SUB, MUL, DIV, INC, DEC, CMP, JMP, JE/JZ, JNE/JNZ, JBE/JNA, JA/JNBE, JL/JNGE, JGE/JNL, JG/JNLE, JLE/JNG, JC/JB/JNAE, JNC/JAE/JNB, JS, JNS, LOOP, SHL/SAL, SHR, OR, AND, XOR, NOT, NEG, XCHG, PUSH, POP, NOP, HLT, INT, DB, DW`

## Keyboard Shortcuts

- `F8` — Single Step
- `F5` — Run
- `F2` — Reload / Assemble

## Run Locally

This project is static HTML/JS/CSS with no build step.

1. Open `index.html` directly in a browser, or
2. Serve the folder with any static server and open it in Chrome.

Example:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Deployment

`vercel.json` is configured to deploy `index.html` as a static app.

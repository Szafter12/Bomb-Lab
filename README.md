## Overview

This repository documents the reverse engineering process of the **CS:APP Bomb Lab** binary. 

The objective is to analyze and defuse all bomb phases through low-level static and dynamic binary analysis without access to the original source code.

### Core Technical Focus
* **Static Disassembly:** Inspecting x86-64 machine instructions, symbol tables, and read-only data sections using `objdump` and `strings`.
* **Dynamic Debugging (GDB):** Runtime execution control, single-instruction stepping (`ni`/`si`), breakpoint placement, and memory/register inspection (`x`, `info registers`).
* **Control Flow Recovery:** Reconstructing high-level programming constructs (loops, recursive calls, `switch` jump tables, arrays, and linked lists) directly from AT&T assembly.

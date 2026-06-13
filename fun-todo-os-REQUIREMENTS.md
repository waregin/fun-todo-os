# fun-todo-os — Requirements & Context

> Drop this file in the repo root as `REQUIREMENTS.md`. Known immediate task: **grab the architecture document and put it in the README.** This doc is the fallback scaffold if the architecture doc has gaps.

## Purpose (Claude Code: reconcile with the real architecture doc — that doc wins)
Module of External Brain OS for *fun* todos — the enjoyable backlog (games to play, crafts to make, creative kits, "fun type activities", Dopamenu-style activity selection) as distinct from obligation tasks in priority-os.

## Context from TickTick
Directly relevant existing tasks:
- "fill out 'Fun TODO database' based on what is currently in TickTick / Collections"
- "build out the functionality for the fun TODOs"
- "make a Dopamenu" (activity types: recurring/organizational, housework/yard, crafts, games, self-care S/M/L/XL lists exist in Personal Notes)
Source lists to import: Fun and Games folder (Film 566, Fun 66, Video Games 965, Queer Games Bundle 588), Crafting (40), Crafting or Creative Kits (43), self-care lists.

## Requirements
- **Functional (draft):** Import fun items from TickTick lists; tag by energy/time required (Dopamenu dimensions); "what should I do for fun right now?" picker (time available + energy + mood → suggestion); track completion
- **Non-functional:** External Brain OS conventions; this is also a natural *first consumer* of priority-os patterns (scoring, recommendation write-back)
- **Boundary:** media-os may own film/game *libraries*; fun-todo-os owns the *picking/doing* layer — confirm with arch doc

## First session objectives
1. Locate architecture doc; merge into README; reconcile with this doc
2. Define the TickTick import (reuse priority-os's TickTick OAuth2 sync code if possible — flag as shared library candidate)
3. Open issues for phase 1; label one `next`

# CMPE 230 — Systems Programming

**Assignment 1 (Spring 2026): SpiresLayer**

## About

SpiresLayer asks students to build a command-line interpreter, in C, that simulates the bookkeeping of a run through a roguelike-deckbuilder-style dungeon (loosely inspired by games like *Slay the Spire*, though no prior gaming knowledge is needed — every rule is spelled out in the handout).

## What students were asked to do

Implement a read–parse–respond loop: the program reads one command per line, classifies it as a state-mutating "sentence," a read-only "question," or the `Exit` command, and responds with precisely formatted output. The interpreter must maintain the full state of a climber's run — gold, health, deck (including cards that permanently exhaust after use), relics, potions, combat knowledge, and floor progress — and enforce a strict grammar: case-sensitive tokens, exact whitespace rules, full-line matching (trailing tokens make a line invalid), a 1024-character line limit, and a specific integer format (no leading zeros, no sign, minimum value 1). Malformed lines must print `INVALID` and the program must continue rather than terminate; semantic errors (e.g., insufficient gold) get their own designated messages instead of `INVALID`.

## Context

This is a systems-programming assignment: the core challenge is writing a robust, from-scratch lexer/parser and state machine in C, with careful attention to string handling, input validation, and precise output formatting rather than any particular algorithm or data structure.

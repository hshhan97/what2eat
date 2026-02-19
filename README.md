# Pantry-First AI Meal Planning System

## Overview
This project builds an AI-powered meal planning system that prioritizes existing pantry ingredients 
while satisfying dietary restrictions, protein targets, and cooking time constraints.

## Live Demo
[Insert Lovable Link Here]

## Demo Video
[Insert Demo Video Link Here]

## Architecture Overview
User Input → Constraint Filtering → Pantry Matching Scoring → LLM Plan Assembly → Validation → Output

## Key Features
- Pantry-first recipe ranking
- Dietary restriction parsing
- Protein target alignment
- Meal prep mode
- Swap + repair loop
- Hallucination control via structured dataset

## How to Reproduce Logic
1. Load recipe CSV dataset.
2. Normalize ingredient lists.
3. Compute pantryHitCount and missingCount.
4. Rank recipes using weighted scoring.
5. Pass top-ranked candidates to LLM for structured weekly assembly.

See `/logic/pantry_scoring.md` for details.

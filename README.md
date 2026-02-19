# Pantry-First AI Meal Planning System

## Overview
This project builds an AI-powered meal planning system that prioritizes existing pantry ingredients 
while satisfying dietary restrictions, protein targets, and cooking time constraints.

## Live Demo
https://what2eatt.lovable.app
## Demo Video
https://docs.google.com/videos/d/1HLKU30c8kM8pDgoNo_78k15z2ynfkCSogb59Api3QJI/edit?scene=id.p#scene=id.p

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

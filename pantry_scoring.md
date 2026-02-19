# Pantry-First Ranking Logic

For each recipe:

pantryHitCount = number of ingredients overlapping with pantry
missingCount = number of ingredients not in pantry

Score formula:

score = (pantryHitCount * 100) 
        - (missingCount * 5) 
        + (protein_g * 0.1) 
        - (cook_time_min * 0.05)

Hard Constraints:
- At least 50% of meals must include pantry ingredients (if available)
- No more than 2 consecutive meals without pantry overlap

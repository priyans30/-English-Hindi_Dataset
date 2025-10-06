# English–Hindi Dataset Processing

## Overview
This project processes an English–Hindi parallel dataset from Hugging Face to create a clean, usable bilingual dataset.

## What I Did
- Calculated the percentage of Devanagari (Hindi) characters in each sentence.  
- Sorted all sentences by this percentage — mostly English at the top, mostly Hindi at the bottom.  
- Took the **top 10,000 sentences** as Hindi and the **bottom 10,000 sentences** as English.  
- Calculated word counts for each sentence and kept only sentences with **5–50 words**.  
- Computed the difference between English and Hindi word counts and kept pairs where the difference was **-10 to +10**.  

## Files
- `english_hindi_processing.ipynb` – Notebook with all steps.  
- `final_cleaned_dataset.xlsx` – Cleaned dataset ready to use.

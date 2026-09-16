[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/SmazhzpM)
# MUSA 5080 Student Portfolio Template

This template helps you create a professional portfolio for Public Policy Analytics coursework.

## Quick Setup
1. **Personalize:** Edit `_quarto.yml` to include your name
2. **About:** Update `index.qmd` with your information
3. **Build:** Run `quarto render` to generate your website
4. **Deploy:** Enable GitHub Pages in Settings → Pages

## Portfolio Structure
- `index.qmd` - Homepage
- `weekly-notes/` - Learning reflections for each week
- `labs/` - Assignment analyses (you'll add this)

## Weekly Notes
Create a new file `weekly-notes/week-XX-notes.qmd` for each week.

### Example Portfolio
See what you're building toward: **[Dr. Delmelle's Sample Portfolio](https://ecdelmelle.github.io/MUSA-5080-instructor-portolio/)**


## Setup: Census API key

This project reads a Census API key from the environment rather than hardcoding it.

1. Copy `.Renviron.example` to `.Renviron` in the project root.
2. Replace `your_key_here` with your own key (request one at
   <https://api.census.gov/data/key_signup.html>).
3. Restart R so the variable is loaded.

The code calls `census_api_key(Sys.getenv("CENSUS_API_KEY"))`. `.Renviron` is
gitignored and must not be committed.

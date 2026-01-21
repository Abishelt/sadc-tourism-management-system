# SADC Tourism Management System (Python OOP)

## Overview
A Python object-oriented model of a SADC-wide tour operator that designs, prices, and books multi-country itineraries with seasonal pricing and limited capacity.

## Key features
- Country-aware seasonal pricing (month → season → multiplier)
- Experience types with category adjustments (Safari, Beach, Cultural, Adventure)
- Per-date availability and capacity reservation
- Itinerary packages composed of dated items with optional discounts
- Validation rules (budget, preferences, cross-border minimum nights, availability)
- Booking lifecycle: preview → confirm (reserve seats) → cancel (restore seats)

## Files
- `Tourism_Systems.ipynb` – class definitions and helper functions
- `Tourism_Sample_Usage.ipynb` – demo run that loads the system and prints outputs
- `Tourism_Report.md/.pdf` – design + results write-up

## How to run
1. Place the notebooks in the same folder.
2. Open `Tourism_Sample_Usage.ipynb`.
3. Run the first cell to load the system:
   `%run -i "Tourism_Systems.ipynb"`
4. Run the remaining cells to reproduce the package overview, price breakdown, and booking flow.

## Example output (from demo)
- Detects cross-border packages (e.g., South Africa + Namibia)
- Calculates date-aware prices with seasonal/category multipliers
- Confirms bookings by reserving per-date capacity and restores on cancel

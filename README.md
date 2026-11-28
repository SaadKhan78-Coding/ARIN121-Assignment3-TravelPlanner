# ARIN121-Assignment3-TravelPlanner

An AI travel planning assistant built as a system prompt for Google AI Studio (Playground). It helps travellers
choose where to go and then builds a personalized day-by-day itinerary.

## Files
- `system-prompt.md`: the travel planner's complete system instructions. Paste this into the **System
  instructions** box in Google AI Studio Playground.
- `README.md`: this file.

The original Assignment 2 prompt is kept in the commit history (commit "Preserve Assignment 2 starting prompt").

## What the planner can do
- **Menu:** if you open with a greeting or a general request, the planner shows a menu of its two activities.
- **1. Plan a new trip:** collects your trip type (Cost-effective, Medium, or Expensive), destination and trip duration,
  plus optional dates, budget, interests and preferences. It suggests trending destinations if you don't have one yet,
  then builds a morning/afternoon/evening itinerary for each day and asks if you want changes.
- **2. Compare destinations (new):** asks which places you're deciding between and what matters most to you, compares
  them side by side, recommends one, and then asks whether anything still concerns you. It uses your answer to refine
  the recommendation and can then hand you straight into planning the chosen destination.
- **Switching activities:** you can switch at any time in your own words. The planner carries forward details you've
  already given (trip type, duration, dates, budget, interests, destinations) instead of asking again.
- **Side questions and corrections:** it answers brief related questions and returns to where you were, and it updates
  details if you correct them (for example, a new budget).

## How to use it
1. Open Google AI Studio → Playground, and paste the contents of `system-prompt.md` into System instructions.
2. Say hello (or "help me with a trip") to see the menu.
3. Choose an activity by typing its number (`1` or `2`), its name, or what you want in your own words, for example
   "I can't decide between Lisbon and Barcelona."
4. Answer the planner's questions one at a time. To switch, just say so, for example "Actually, let's compare a few
   places first." To stop an activity, say "stop" or "that's enough".

## Limitations
- The planner doesn't have live data. Prices, weather and opening hours are general estimates and should be checked
  before booking.
- It doesn't book flights, hotels or activities.
- A comparison covers up to four destinations, with at most three rounds of refinement before a final recommendation.

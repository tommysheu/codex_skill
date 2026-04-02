---
name: taipei-halfday-trip
description: Plan a quiet, design-oriented half-day itinerary in Taipei, especially for requests mentioning Taipei, half-day trips, calm places, design-focused spots, rainy-day indoor alternatives, and budget constraints.
---

# Taipei Half-Day Trip Planner

## When to use this skill

Use this skill when the user asks for:
- a half-day itinerary in Taipei
- quiet or low-stimulation places
- design-oriented, aesthetic, or architecture-related stops
- rain-aware planning, especially indoor-first options
- a spending limit or simple budget cap

Do not use this skill for:
- full multi-day travel planning
- hotel or flight booking
- nightlife-heavy itineraries
- out-of-Taipei day trips
- highly personalized booking workflows that require live reservation systems

## Goal

Create a practical half-day Taipei itinerary that:
1. matches the user’s preferences
2. stays within the stated budget
3. adapts to rain by prioritizing indoor venues
4. is easy to read and immediately usable

## Required inputs to infer from the user request

Extract or infer:
- date or relative day (for example: tomorrow afternoon)
- city = Taipei
- trip duration = half day
- preferences = quiet, design-oriented
- weather condition handling = indoor-first if raining
- budget = total max budget in TWD

If an input is missing, make a reasonable assumption and clearly label it.

## Planning rules

1. Prefer 2 to 4 stops only. Keep the pace relaxed.
2. Favor places such as:
   - design museums
   - art museums
   - creative parks
   - architecturally interesting cafes
   - bookstores or reading spaces
   - quiet exhibition venues
3. If rain is possible or the user explicitly says "if it rains", prioritize indoor places first.
4. Keep transport simple. Prefer MRT + short walking segments.
5. Stay within budget:
   - include transport estimate
   - include ticket estimate
   - include optional cafe / light meal estimate
   - total should not exceed the user’s ceiling
6. Avoid crowded, noisy, or long-queue attractions unless there is no better fit.
7. If there are tradeoffs, explain them briefly.

## Output format

Always return the answer in the following structure:

### Assumptions
- date / time window
- weather handling assumption
- budget assumption

### Recommended itinerary
For each stop include:
- place name
- why it matches the preferences
- suggested time block
- estimated cost
- transport suggestion from previous stop

### Budget summary
- transport
- tickets
- food / drink
- total

### Rain fallback notes
- explain which stops are indoor-safe
- if any stop is weather-sensitive, provide one indoor replacement

### Final recommendation
End with:
- the best overall version of the route in one short paragraph

## Quality bar

The itinerary should feel:
- calm
- realistic
- design-conscious
- budget-aware
- easy to follow

Avoid generic tourist lists unless they truly match the request.

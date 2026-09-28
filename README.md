# A Number Pattern Field Notebook

A small, reproducible activity for exploring ordinary integers. Use paper, a spreadsheet, or a calculator. The aim is to separate a number's mathematical properties from how surprising it feels.

## 1. Fix the universe before calling anything rare

Choose the inclusive range 0 to 1,000,000 and ordinary base-ten notation without leading zeros. Each of its 1,000,001 integers is a distinct possible observation. Changing the range or allowing leading zeros changes how often digit patterns occur. A label such as “rare” needs that context.

Keep two questions separate: “How often does this property occur?” and “How often would my sampling method produce this number?” A manually selected birthday is not a random sample. Every individual number has equal probability under uniform sampling, even when some numbers have more interesting properties.

## 2. Predict, check, explain

Start with 121, 1221, 144, 997 and 1000. Before checking them, write down which properties you expect. Then verify each prediction.

| Number | A property to test | A check you can reproduce |
|---|---|---|
| 121 | Palindrome and perfect square | Reverse 121; calculate 11 × 11 |
| 1221 | Palindrome and composite | Reverse its digits; calculate 3 × 407 |
| 144 | Perfect square and Fibonacci number | Calculate 12 × 12; continue the Fibonacci recurrence |
| 997 | Prime | Test divisibility by primes up to 31 |
| 1000 | Perfect cube | Calculate 10 × 10 × 10 |

A palindrome reads identically in both directions. A perfect square is the square of an integer. A prime has exactly two positive divisors; 0 and 1 are not prime. Checking divisors only through the square root suffices because any larger factor must pair with a smaller one.

## 3. Change just one digit

Take 1221 and change one position at a time: 1220, 1231, 1321, 2221. Record which properties survive. Keep the length fixed in this experiment so that removing a leading digit does not quietly introduce a second change.

This is a useful way to form a hypothesis. Matching first and last digits is necessary for a four-digit palindrome, but it is not sufficient: the middle pair must match too. Test a counterexample before turning an observation into a rule.

## 4. Record a small sample honestly

Copy this header into a spreadsheet:

```csv
number,selection_method,predicted_patterns,verified_patterns,manual_check,unexpected_result,next_question
```

Add ten numbers chosen before you inspect their scores. Save unsuccessful predictions as well as successful ones. Ten observations can suggest a question; they cannot establish the exact population frequency of a rare pattern. Use a complete enumeration or a mathematical count when you need an exact frequency.

## 5. Explore with a browser tool

[RNGDLE.ART](https://rngdle.art/) is a companion for this activity. It analyzes integers from 0 to 1,000,000 across 31 named patterns, with factorization, digit statistics, rarity scores and percentiles within that range. It also offers number comparisons, a digit sandbox and daily browser challenges. The tool is free and requires no signup.

Disclosure: this notebook is maintained alongside RNGDLE.ART. Its score is a defined game and exploration measure, not evidence that a number predicts real-world events. Different pattern definitions or scoring rules can produce different rankings. Read the tool's methodology when interpreting a score. Saved numbers and progress stay in the current browser; there is no cross-device account or global player leaderboard.

## A closing experiment

Choose one property, state its definition, and compare its frequency in 0–999 and 0–9999. Explain why the denominators differ. Then write one claim your observations support and one tempting claim they do not support. That distinction is the most useful result to keep in your notebook.

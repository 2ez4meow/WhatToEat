# Recommendation Algorithm

## Purpose

The algorithm should help a user discover what they want to eat, not simply filter a database.

The goal is to make one confident recommendation.

---

## Two Modes

### Mode 1 — Quick Choice

The user selects several preference tags.

Example:

- Spicy
- Meat
- Hot
- For sharing

The algorithm scores every dish and recommends the best match.

---

### Mode 2 — I Have No Idea

The bot asks a short sequence of questions.

Each answer removes a large number of possible dishes.

The questions should start with the highest-impact choices.

Example:

Question 1:
Sweet or Savory?

Question 2:
Meat or No Meat?

Question 3:
Heavy meal or Something light?

Question 4:
Hot or Cold?

Question 5:
Eat alone or Share?

Usually 4–6 questions should be enough.

---

## Scoring

Every dish has its own tags and taste values.

The recommendation score is calculated based on how closely the dish matches the user's answers.

The highest score wins.

---

## Second Recommendation

If the user presses "Another option", the current dish is removed from the candidate list.

The algorithm recommends the next highest-scoring dish.

---

## Future Improvements

In future versions the algorithm will learn from user feedback.

Liked dishes become more likely.

Disliked dishes become less likely.

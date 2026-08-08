# CMPE 343 — Probability & Statistics

**Course Project (Fall 2025): Tunes Duel — A Probabilistic Simulation of Music Recommendation Systems**

## About

Tunes Duel is a four-part course project that teaches probability and statistics concepts through the lens of a music recommendation system, using a real dataset of ~2,000 Spotify tracks (`tracks.csv`) combined with simulated and student-submitted user rating sessions (`ratings.csv`). Each student also contributes a personal session file of 10–20 song ratings, used throughout the project and pooled anonymously across the class.

## What students were asked to do

- **Part 1 — Conditional Probability Modeling:** Estimate the probability a song receives a 5-star rating, both globally and from the student's own session, conditioning on features like artist, release year, explicit flag, mood, genre, and timbre, using Laplace smoothing for sparse categories and exploring feature interactions.
- **Part 2 — User Variability Modeling:** Model how many recommendations it takes a user to rate a song 5 stars, using geometric and Beta-geometric distributions.
- **Part 3 — Recommender Design:** Build two different recommendation models informed by the Part 1/2 analyses.
- **Part 4 — Monte Carlo Evaluation:** Simulate user interactions to compare the two models via metrics like Hit@k, average rating, and time-to-5-star, reporting confidence intervals.

Submissions later competed pairwise in an in-class online competition based on live user feedback.

## Context

This is the main statistics course project: it exercises conditional probability estimation, smoothing, discrete probability distributions (geometric/Beta-geometric), and Monte Carlo simulation with confidence-interval estimation, all grounded in a realistic, student-sourced dataset rather than synthetic textbook data.

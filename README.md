# Grading Essays with Supervised Learning

Bob Effinger, David Merrell, Jack Ordman, Jack Truskowski, Samuel Vinitsky.
Final project for CS 760 (graduate machine learning), University of Wisconsin–Madison, 2018.

[Read the paper (PDF)](Grading_Essays_with_Supervised_Learning.pdf)

Supervised models trained to emulate human graders on the Hewlett Foundation's Automated Student Assessment Prize corpus from the 2012 Kaggle competition: about 12,000 student essays across eight prompts, each scored by human raters.

- Features: essay structure, misspelling rate, and part-of-speech frequencies, chosen by a lesion study.
- Models: decision trees, k-NN, SVMs and small neural nets, then AdaBoost and gradient boosting over each, plus an n-gram graphical model per score class augmented with hand-built features.
- Evaluation: RMSE internally, quadratic weighted kappa against the human raters for comparison with the competition leaderboard.
- Result: the best model would have placed 32nd of 154 competition entrants. Feature choice mattered more than model choice.

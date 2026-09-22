# Nested cross-validation

↑ **Parent:** [Cross-validation](cross-validation.md)

Nested cross-validation separates selection from assessment using two levels of held-out data. Within each outer training fold, inner [cross-validation](cross-validation.md) chooses a model or tuning parameters; the complete selected fitting procedure is then applied to that outer training fold and scored on its untouched outer evaluation fold. This estimates the performance of the [model selection](model-selection.md) procedure, including its choices, rather than reusing its best inner score as an assessment. A final model can then be selected and fitted using all available [training data](training-data.md). [Cawley and Talbot, selection bias and performance evaluation](https://jmlr.org/papers/v11/cawley10a.html)

## ↑ Ancestors (8)

1. [Cross-validation](cross-validation.md)
2. [Statistical learning](statistical-learning-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Cross-validation](cross-validation.md)
- [Ridge regression](ridge-regression.md)

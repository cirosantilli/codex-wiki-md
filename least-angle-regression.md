# Least angle regression

↑ **Parent:** [Linear regression](linear-regression-split.md)

A piecewise linear regression-path algorithm which starts at zero, activates a predictor with maximal absolute residual score, and moves in a direction that decreases all active absolute scores equally until another predictor ties them. With $G=X^{\mathsf T}X/n$ and active correlation signs $s_A$, the coefficient direction is $G_{AA}^{-1}s_A$. Ordinary LAR does not drop a predictor when its coefficient crosses zero; [sign compatibility of LAR and Lasso](sign-compatibility-of-lar-and-lasso.md) characterizes when its path also obeys the [Lasso](lasso.md) [KKT conditions](karush-kuhn-tucker-conditions.md).

**Table of contents**

- [Equiangular direction in least angle regression](equiangular-direction-in-least-angle-regression.md)
- [Sign compatibility of LAR and Lasso](sign-compatibility-of-lar-and-lasso.md)
- [LAR active correlation invariant](lar-active-correlation-invariant.md)
- [Entry knot in least angle regression](entry-knot-in-least-angle-regression.md)

## ↑ Ancestors (8)

1. [Linear regression](linear-regression-split.md)
2. [Normal linear model](normal-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [LAR active correlation invariant](lar-active-correlation-invariant.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-34/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-32/1/solution.md)
- [Sign compatibility of LAR and Lasso](sign-compatibility-of-lar-and-lasso.md)

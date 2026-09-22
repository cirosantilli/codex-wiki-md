# Sequential response selection model

↑ **Parent:** [Missing-data mechanism](missing-data-mechanism.md)

Suppose outcome collection stops at the first success or after $m$ unsuccessful attempts, and let $A$ count unsuccessful attempts. Conditional on the outcome $y$, put $q_j(y)=\mathbb P(A\geq j\mid A\geq j-1,Y=y)$. For $k<m$, the joint density of $A=k$ and an observed $Y=y$ is

$$
f_\beta(y)\left(\prod_{j=1}^{k}q_j(y)\right)(1-q_{k+1}(y)).
$$

For $A=m$, the unobserved outcome is integrated out, giving $\int f_\beta(y)\prod_{j=1}^m q_j(y)\,dy$. These probabilities sum to one by telescoping and integration. Dependence of $q_j$ on $y$ models [missing not at random](missing-not-at-random.md). If all $q_j$ are independent of $y$ conditional on the regression predictors, the outcome density among responders remains $f_\beta$, as required for [complete-case analysis](complete-case-analysis.md) of that conditional model.

## ↑ Ancestors (6)

1. [Missing-data mechanism](missing-data-mechanism.md)
2. [Missing data](missing-data.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-41/1/d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-41/1/d/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-41/1/e/solution.md)

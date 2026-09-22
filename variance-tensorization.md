# Variance tensorization

↑ **Parent:** [Efron–Stein inequality](efron-stein-inequality.md)

Write $X_{-i}$ for all inputs except $X_i$. Under the [Efron–Stein inequality](efron-stein-inequality.md) hypotheses, [variance tensorization](variance-tensorization.md) is the equivalent [conditional variance](conditional-variance.md) form

$$
\boxed{\operatorname{Var}(Z)\leq\sum_{i=1}^n\mathbb E[\operatorname{Var}(Z\mid X_{-i})].}
$$

Conditioning freezes the other inputs. Then $Z,Z_i'$ are [independent](independent-random-variables.md) with the same conditional [probability distribution](probability-distribution-split.md), giving

$$
\frac12\mathbb E[(Z-Z_i')^2\mid X_{-i}]=\operatorname{Var}(Z\mid X_{-i}).
$$

Taking [expected values](expected-value-split.md) explains the factor $1/2$.[Lecture 7a: Efron Stein inequality, slides 2 and 7, PDF pp. 3 and 8: conditional variances and the independent-copy identity](lecture-7a-efron-stein-inequality-by-purnamrita-sarkar.md)

For [Bernoulli](bernoulli-distribution.md) input $X_i$ with parameter $p_i$, let $\Delta_i f$ be the value of $f$ with coordinate $i$ set to one minus its value with that coordinate set to zero, keeping $X_{-i}$ fixed. The two-point [conditional variance](conditional-variance.md) is

$$
\operatorname{Var}(Z\mid X_{-i})=p_i(1-p_i)(\Delta_i f)^2.
$$

For the maximum example, $\Delta_1 f=1-X_2$ and $\Delta_2 f=1-X_1$. The two averaged [conditional variances](conditional-variance.md) are $0.3(0.7)(0.4)=0.084$ and $0.6(0.4)(0.7)=0.168$, precisely half the respective resampling terms. In the dependent example $X_1=X_2=B$, each other coordinate already determines $W$, so both [conditional variances](conditional-variance.md) vanish; [variance tensorization](variance-tensorization.md) also fails without [independence](independent-random-variables.md).

For a short induction proof, separate the last input using the [law of total variance](law-of-total-variance.md). Apply the smaller-dimensional statement to the [conditional expectation](conditional-expectation.md); [Jensen's inequality](jensen-s-inequality.md) for the square bounds its coordinate contributions by the original ones. One input gives equality, starting the induction.[Lecture 7a: Efron Stein inequality, slides 3–6, PDF pp. 4–7: variance decomposition and conditional Jensen step; the induction outline here reorganizes those ingredients](lecture-7a-efron-stein-inequality-by-purnamrita-sarkar.md)

## ↑ Ancestors (8)

1. [Efron–Stein inequality](efron-stein-inequality.md)
2. [Concentration inequality](concentration-inequality.md)
3. [Probability inequality](probability-inequality-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ia/paper-2/9f/b/solution.md)
- [Variance tensorization](variance-tensorization.md)

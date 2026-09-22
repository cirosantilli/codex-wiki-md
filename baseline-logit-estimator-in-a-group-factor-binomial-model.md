# Baseline logit estimator in a group-factor binomial model

↑ **Parent:** [Grouped-binomial logistic regression](grouped-binomial-logistic-regression.md)

For independent $Y_{ij}\sim\operatorname{Bin}(m,p_i)$ with $k$ replicates per group and $\operatorname{logit}(p_i)=\mu+\alpha_i$, $\alpha_1=0$, let $S_i=\sum_jY_{ij}$ and $N=km$. The likelihood equations give $\widehat p_i=S_i/N$, $\widehat\mu=\log(S_1/(N-S_1))$, and $\widehat\alpha_i=\operatorname{logit}(\widehat p_i)-\widehat\mu$ when $0<S_i<N$. Boundary totals give infinite logits. With $0<p_1<1$ fixed and $N\to\infty$, the [central limit theorem](central-limit-theorem.md) and [delta method](delta-method.md) give

$$
\sqrt N(\widehat\mu-\mu)\ \xrightarrow{d}\ N\left(0,\frac1{p_1(1-p_1)}\right).
$$

The other groups do not increase information about the baseline logit when they have free offsets. For two groups, the information matrix for $(\mu,\alpha_2)$ is $\begin{pmatrix}w_1+w_2&w_2\\w_2&w_2\end{pmatrix}$ with $w_i=Np_i(1-p_i)$, whose inverse has first diagonal entry $1/w_1$.

## ↑ Ancestors (9)

1. [Grouped-binomial logistic regression](grouped-binomial-logistic-regression.md)
2. [Logistic regression](logistic-regression.md)
3. [Generalized linear model](generalized-linear-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43/3/solution.md)

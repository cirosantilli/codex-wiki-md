# Gaussian mixture Gibbs updates with independent priors

↑ **Parent:** [Finite mixture model](finite-mixture-model.md)

In a finite [normal distribution](normal-distribution.md) mixture with allocation labels $z_j$, independently assign $\mu_i\sim N(m_0,\tau^2)$, $v_i\sim\operatorname{InvGamma}(\alpha,\beta)$ and weights a [Dirichlet distribution](dirichlet-distribution.md). Let $n_i$ count allocations to component $i$ and $s_i$ sum their observations. The conditional mean precision is $V_i^{-1}=\tau^{-2}+n_i/v_i$, giving $\mu_i\mid\cdots\sim N(V_i(m_0/\tau^2+s_i/v_i),V_i)$. The conditional variance is the displayed [inverse-gamma distribution](inverse-gamma-distribution.md); weights have Dirichlet parameters increased by allocation counts. Allocation probabilities are proportional to $\omega_i\varphi(x_j;\mu_i,v_i)$. Independence of the mean prior from $v_i$ is important: its density does not add an extra inverse-gamma shape term.

## ↑ Ancestors (8)

1. [Finite mixture model](finite-mixture-model.md)
2. [Mixture model](mixture-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/3/b/i/solution.md)

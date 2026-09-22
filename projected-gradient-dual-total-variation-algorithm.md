# Projected-gradient dual total variation algorithm

↑ **Parent:** [Projection residual for discrete total variation](projection-residual-for-discrete-total-variation.md)

Minimize $F(p)=\tfrac12\|g-D^*p\|_2^2$ over $P=\{p:|p_i|_2\le\lambda\}$ using

$$
p^{k+1}=\Pi_P\bigl(p^k+\tau D(g-D^*p^k)\bigr).
$$

The pointwise [Euclidean projection onto a convex set](euclidean-projection-onto-a-convex-set.md) sends a block $r$ to $r/\max(1,|r|_2/\lambda)$. The [gradient](gradient.md) of $F$ has [Lipschitz constant](lipschitz-constant.md) $\|D\|^2$, so finite-dimensional [projected gradient descent](projected-gradient-descent.md) converges for $0<\tau<2/\|D\|^2$. On an unscaled square grid with $N>1$, $0<\tau<1/4$ is safe. Reconstruct $u^k=g-D^*p^k$; unused dual directions may make the minimizing $p$ nonunique while the primal minimizer is unique.

## ↑ Ancestors (11)

1. [Projection residual for discrete total variation](projection-residual-for-discrete-total-variation.md)
2. [Discrete isotropic total variation](discrete-isotropic-total-variation.md)
3. [Total variation denoising](total-variation-denoising.md)
4. [Total variation seminorm on a domain](total-variation-seminorm-on-a-domain.md)
5. [Variational regularization](variational-regularization.md)
6. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
7. [Inverse problem](inverse-problem-split.md)
8. [Analysis](analysis-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340/5/b/solution.md)

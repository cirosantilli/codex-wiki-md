# Shifted-comparator Bregman bound

↑ **Parent:** [Normal-operator source condition](normal-operator-source-condition.md)

Let $u^\dagger$ be a [least-squares solution](least-squares-solution-of-a-linear-inverse-problem.md) and $w=K^*Kv\in\partial J(u^\dagger)$. For a minimizer $u_\alpha$ of $\|Ku-f\|^2/2+\alpha J(u)$, expand the objective about $u^\dagger$. The [normal equation for a linear inverse problem](normal-equation-for-a-linear-inverse-problem.md) removes the data-residual cross term, while the [Bregman distance](bregman-divergence.md) definition gives

$$
\mathcal F_\alpha(u)-\mathcal F_\alpha(u^\dagger)=\frac12\|K(u-u^\dagger+\alpha v)\|^2+\alpha D_J^w(u,u^\dagger)-\frac{\alpha^2}2\|Kv\|^2.
$$

Compare the minimizer with $u^\dagger-\alpha v$, where the square vanishes, and divide by $\alpha$. The bound is informative when that comparator has finite penalty.

## ↑ Ancestors (9)

1. [Normal-operator source condition](normal-operator-source-condition.md)
2. [Source condition in variational regularization](source-condition-in-variational-regularization.md)
3. [Variational regularization](variational-regularization.md)
4. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
5. [Inverse problem](inverse-problem-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-326/2/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-326/2/vi/solution.md)

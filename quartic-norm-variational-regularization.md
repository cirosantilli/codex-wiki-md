# Quartic-norm variational regularization

↑ **Parent:** [Variational regularization](variational-regularization.md)

For a bounded [linear operator](linear-operator.md) $A$ between [Hilbert spaces](hilbert-space-split.md), minimize $\|Au-f\|^2+\alpha\|u\|^4$, with $\alpha>0$. The objective is coercive and weakly lower semicontinuous, and its [strictly convex](strictly-convex-function.md) norm penalty gives a unique minimizer. Its stationarity equation is

$$
A^*(Au-f)+2\alpha\|u\|^2u=0,
$$

so the map from data to solution is generally nonlinear. For admissible fixed $f$, comparison with $u^\dagger=A^\dagger f$ bounds the minimizer's norm by $\|u^\dagger\|$ and makes its squared residual converge to the minimum least-squares residual. Every weak cluster point is therefore a least-squares solution of norm at most $\|u^\dagger\|$, hence equals the [minimum-norm least-squares solution](minimum-norm-least-squares-solution.md). Weak lower semicontinuity then forces convergence of norms, and the [Radon-Riesz theorem](radon-riesz-theorem.md) gives strong convergence. This supplies a nonlinear [regularization of an inverse problem](regularization-of-an-inverse-problem.md).

For completeness, the fixed-$\alpha$ data-to-solution map is continuous. For $g(u)=\|u\|^2u$, setting $m=(u+v)/2$ and $d=(u-v)/2$ gives

$$
\operatorname{Re}\langle g(u)-g(v),u-v\rangle
=4(\|m\|^2+\|d\|^2)\|d\|^2+8(\operatorname{Re}\langle m,d\rangle)^2
\geq\tfrac14\|u-v\|^4.
$$

Subtracting the stationarity equations for data $f,h$ and pairing with $u-v$ therefore gives $\frac\alpha2\|u-v\|^4\leq\|A\|\|f-h\|\|u-v\|$. Thus

$$
\|R_\alpha f-R_\alpha h\|\leq\left(\frac{2\|A\|}{\alpha}\|f-h\|\right)^{1/3},
$$

which proves continuity directly.

## ↑ Ancestors (7)

1. [Variational regularization](variational-regularization.md)
2. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
3. [Inverse problem](inverse-problem-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-326/1/a/solution.md)

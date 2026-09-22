<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume first that $0<\epsilon<1/2$, set $k=\lfloor\epsilon n\rfloor$, and replace the last $k$ observations by $100$. Among the remaining $m=n-k$ observations, let

$$
Y_i=\mathbf1_{\{X_i>\epsilon\}},
\qquad
p_\epsilon=\mathbb P(Z>\epsilon)=1-\Phi(\epsilon).
$$

The contaminated median exceeds $\epsilon$ whenever

$$
\sum_{i=1}^mY_i\geq\frac{n+1}{2}-k.
$$

The right-hand threshold divided by $m$ tends to

$$
q_\epsilon=\frac{1/2-\epsilon}{1-\epsilon}<p_\epsilon.
$$

Therefore, for all sufficiently large $n$, it is at most $p_\epsilon-\delta_\epsilon$ for some $\delta_\epsilon>0$. The [Hoeffding inequality](../../../../../../hoeffding-inequality.md) gives

$$
\mathbb P\!\left(
\sum_{i=1}^mY_i<\frac{n+1}{2}-k
\right)
\leq e^{-2m\delta_\epsilon^2}
\leq e^{-c_\epsilon n}.
$$

The supremum over adversarial perturbations is at least this explicit construction, proving the claim. When $\epsilon\geq1/2$, replacing at least half the sample makes the conclusion immediate.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

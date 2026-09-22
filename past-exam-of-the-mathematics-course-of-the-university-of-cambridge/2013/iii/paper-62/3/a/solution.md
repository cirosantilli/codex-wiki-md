<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One form of [Farkas' lemma](../../../../../../farkas-lemma.md) states that exactly one of the following holds:

$$
\boxed{\exists z\geq0:\ Az=b,\qquad
\exists y:\ A^Ty\geq0,\ b^Ty<0.}
$$

Their mutual exclusion is immediate: if both held, $b^Ty=z^TA^Ty\geq0$.

For existence of the alternative certificate, let $C=\{Az:z\geq0\}$, the [finitely generated cone](../../../../../../finitely-generated-cone.md) of the columns of $A$. It is convex. It is also closed, a fact that must be justified rather than assumed for arbitrary linear images of closed cones. In a representation with dependent active generators, choose a nonzero dependence $\sum_jd_ja_j=0$ with at least one $d_j>0$. Subtract

$$
t d,\qquad t=\min_{d_j>0}\frac{\lambda_j}{d_j}
$$

from the nonnegative coefficient vector. The represented point is unchanged, all coefficients remain nonnegative, and at least one active coefficient disappears. Iteration produces a representation with independent active columns. For a convergent sequence in $C$, pass to a subsequence using the same independent set, possible because there are finitely many sets. Its coefficients converge through a fixed left inverse, and their limits remain nonnegative. This proves [closedness of finitely generated cones](../../../../../../closedness-of-finitely-generated-cones.md).

The [indicator functional](../../../../../../indicator-functional-of-a-constraint-set.md) $\delta_C$ is therefore proper, lower semicontinuous and convex. Its [Legendre-Fenchel transform](../../../../../../convex-conjugate.md) is

$$
\delta_C^*(w)=
\begin{cases}
0,&A^Tw\leq0,\\
+\infty,&\text{otherwise}.
\end{cases}
$$

Indeed a positive pairing with a cone generator can be scaled arbitrarily, while all nonpositive pairings give supremum zero. The [Fenchel-Moreau theorem](../../../../../../fenchel-moreau-theorem.md) now gives

$$
\delta_C(b)=\delta_C^{**}(b)=\sup_{A^Tw\leq0}\langle w,b\rangle.
$$

If $b\notin C$, the left side is infinite, so some feasible $w$ has $\langle w,b\rangle>0$. Taking $y=-w$ gives $A^Ty\geq0$ and $b^Ty<0$. If $b\in C$, the first alternative holds. **The biconjugation theorem applied to a closed finitely generated cone proves the alternative.**

For inequalities $Cx\leq d$ with unrestricted $x$, split $x=x_+-x_-$ and add nonnegative slack:

$$
[C,-C,I]\begin{pmatrix}x_+\\x_-\\s\end{pmatrix}=d.
$$

The equivalent [Farkas certificate for linear inequalities](../../../../../../farkas-certificate-for-linear-inequalities.md) is

$$
y\geq0,\qquad C^Ty=0,\qquad d^Ty<0.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

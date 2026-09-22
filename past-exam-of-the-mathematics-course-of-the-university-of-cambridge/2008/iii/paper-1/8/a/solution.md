<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A bounded [self-adjoint operator](../../../../../../self-adjoint-operator.md) $T$ is a [positive operator](../../../../../../positive-operator.md) when $\langle T\xi,\xi\rangle\geq0$ for every $\xi$. Equivalently its [quadratic form](../../../../../../quadratic-form.md) is nonnegative. We construct its [positive square root of an operator](../../../../../../positive-square-root-of-an-operator.md) directly and prove uniqueness.

If $T=0$ its positive square root is zero. Otherwise set $r=\|T\|$, $B=T/r$, and $C=I-B$. Then $0\leq B\leq I$ and $C$ is positive. It is also a contraction. Indeed, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) for the positive form $\langle B\xi,\eta\rangle$ gives $\|B\xi\|^2\leq\langle B\xi,\xi\rangle$, and hence

$$
\|C\xi\|^2=\|\xi\|^2-2\langle B\xi,\xi\rangle+\|B\xi\|^2\leq\|\xi\|^2.
$$

The scalar binomial series has the form

$$
\sqrt{1-z}=1-\sum_{n\geq1}c_nz^n,\qquad
c_n=\frac{\binom{2n}{n}}{4^n(2n-1)}>0,\qquad\sum_{n\geq1}c_n=1.
$$

The last equality follows by taking $z\uparrow1$ in the nonnegative series. Therefore

$$
S=\sqrt r\left(I-\sum_{n\geq1}c_nC^n\right)
$$

converges in [operator norm](../../../../../../operator-norm.md). Every $C^n$ is a positive contraction: its even powers are squares, its odd powers have form $C^kCC^k$, and their [norms](../../../../../../norm.md) are at most one. Each partial sum for $S/\sqrt r$ is consequently positive, since it is at least $(1-\sum_{n\leq N}c_n)I$. The limit is positive. Multiplying the absolutely convergent series and using the scalar coefficient identity gives $S^2=r(I-C)=T$. This construction also shows that $S$ is a [norm](../../../../../../norm.md) limit of polynomials in $T$ and thus commutes with every operator commuting with $T$.

Now suppose $R$ is another positive square root. It commutes with $T=R^2$, hence with $S$. Thus

$$
(R-S)(R+S)=R^2-S^2=0.
$$

The difference vanishes on the range of $R+S$ and on its [closure](../../../../../../closure-topology.md). It also vanishes on its [kernel](../../../../../../kernel-of-a-linear-map.md): if $(R+S)\xi=0$, the fact that $R$ and $S$ are [positive operators](../../../../../../positive-operator.md) gives $\langle R\xi,\xi\rangle=\langle S\xi,\xi\rangle=0$, and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) for their positive forms implies $R\xi=S\xi=0$. Since $R+S$ is [self-adjoint](../../../../../../self-adjoint-operator.md), the orthogonal sum of its [kernel](../../../../../../kernel-of-a-linear-map.md) and closed range is all of $H$. Therefore $R=S$, proving

$$
\boxed{T\geq0\Longrightarrow\text{a unique }T^{1/2}\geq0\text{ with }(T^{1/2})^2=T.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a weight-$k$ [cusp form](../../../../../../cusp-form.md), the [invariant norm of a modular form](../../../../../../invariant-norm-of-a-modular-form.md) $y^{k/2}|f(z)|$, with $y=\operatorname{Im}z$, is unchanged by the [modular group](../../../../../../modular-group.md): $\operatorname{Im}(\gamma z)=y/|cz+d|^2$ and $|f(\gamma z)|=|cz+d|^k|f(z)|$ cancel exactly.

Every orbit meets the [standard fundamental domain of the modular group](../../../../../../standard-fundamental-domain-of-the-modular-group.md) $\mathcal F=\{z:|\operatorname{Re}z|\leq1/2,\ |z|\geq1\}$, where $y\geq\sqrt3/2$. The [Fourier expansion of a modular form](../../../../../../fourier-expansion-of-a-modular-form.md) at the cusp has $f(q)=q h(q)$, with $h$ holomorphic near zero, since $f$ is a [cusp form](../../../../../../cusp-form.md). Thus $|f(x+iy)|=O(e^{-2\pi y})$ uniformly in $x$ as $y\to\infty$, and $y^{k/2}|f|$ tends to zero there. On the remaining compact part of $\mathcal F$ it is bounded by continuity. Invariance therefore gives

$$
\boxed{B:=\sup_{z\in\mathfrak H}y^{k/2}|f(z)|<\infty.}
$$

For every $y>0$, [Fourier coefficient](../../../../../../fourier-coefficient.md) extraction gives

$$
a_n(f)=e^{2\pi ny}\int_0^1f(x+iy)e^{-2\pi inx}\,dx,
\qquad |a_n(f)|\leq B e^{2\pi ny}y^{-k/2}.
$$

For $n\geq1$, minimize the last factor by taking $y=k/(4\pi n)$. This proves the [Fourier coefficient bound for a cusp form](../../../../../../fourier-coefficient-bound-for-a-cusp-form.md)

$$
\boxed{|a_n(f)|\leq B\left(\frac{4\pi e}{k}\right)^{k/2}n^{k/2}<Cn^{k/2},
\quad C=B\left(\frac{4\pi e}{k}\right)^{k/2}+1.}
$$

The assertion concerns positive indices; the constant coefficient vanishes because $f$ is a [cusp form](../../../../../../cusp-form.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

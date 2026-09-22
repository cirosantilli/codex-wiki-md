<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

This is the [Poincaré residue](../../../../../../poincare-residue-along-a-smooth-hypersurface.md) of a meromorphic top form with a simple pole. Write $z=z_1$ and locally $\alpha=(dz/z)\wedge\beta$, with $\beta$ a holomorphic $(n-1)$-form. The proposed residue is the pullback of $\beta$ to $Y$.

First it does not depend on the choice of $\beta$: if $dz\wedge(\beta-\beta')=0$, then at each point the difference has a factor $dz$, and its pullback to $Y$ is zero. Now change the local defining coordinate to $t=az$, where $a$ is a nowhere-zero [holomorphic function](../../../../../../holomorphic-function.md). Such a factor exists because both coordinates define the same smooth [complex analytic hypersurface](../../../../../../complex-analytic-hypersurface.md). If $\alpha=(dt/t)\wedge\eta$, then

$$
dz\wedge\beta=z\alpha=\frac1a\,dt\wedge\eta
=dz\wedge\eta+\frac za\,da\wedge\eta.
$$

At points of $Y$, this is an equality in the ambient exterior-power fibre, and the last term is zero. It follows that $dz\wedge(\beta-\eta)=0$ there, so their pullbacks to $Y$ agree. This also covers changes of the tangential coordinates.

The restrictions are holomorphic top forms on $Y$, and their agreement on overlaps makes them a global section of the [canonical bundle](../../../../../../canonical-bundle.md). Thus **the residue is independent of the adapted coordinates**:

$$
\boxed{\operatorname{Res}_Y(\alpha)\in\Gamma(Y,K_Y),\qquad
\operatorname{Res}_Y(\alpha)=\left.h\,dz_2\wedge\cdots\wedge dz_n\right|_Y.}
$$

The ambient-fibre comparison is important: pulling an ambient $n$-form directly back to the $(n-1)$-dimensional hypersurface would give zero and would not prove the required independence.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

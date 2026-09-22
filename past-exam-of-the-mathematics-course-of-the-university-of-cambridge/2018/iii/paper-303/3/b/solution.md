<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At the [Gaussian fixed point](../../../../../../gaussian-fixed-point.md), $[\phi_i]=(d-2)/2$, so all three quartic couplings have [engineering dimension](../../../../../../engineering-dimension.md) $d-4[\phi_i]=4-d$. Thus

$$
\boxed{\alpha_1=\alpha_2=\alpha_3=\epsilon}.
$$

Take $A>0$ and $\epsilon>0$, as in the perturbative [epsilon expansion](../../../../../../epsilon-expansion.md). Define $x=Ag_1/\epsilon$, $y=Ag_2/\epsilon$, $z=A\lambda/\epsilon$. The [renormalization-group fixed point](../../../../../../renormalization-group-fixed-point.md) equations become

$$
x-36x^2-z^2=0,\qquad y-36y^2-z^2=0,\qquad z[1-8z-12(x+y)]=0.
$$

If $z=0$, each of $x,y$ is independently $0$ or $1/36$, giving four [renormalization-group fixed points](../../../../../../renormalization-group-fixed-point.md). If $z\ne0$, subtracting the first two equations gives

$$
(x-y)[1-36(x+y)]=0.
$$

The branch $x+y=1/36$ forces $z=1/12$; inserting this in the first equation yields a repeated root $x=y=1/72$. Hence every nonzero-$z$ solution has $x=y$. Then $z=1/8-3x$, and

$$
45x^2-\frac74x+\frac1{64}=0
$$

has roots $x=1/40$ and $x=1/72$. The complete list of six [coupled Ising fixed points near four dimensions](../../../../../../coupled-ising-fixed-points-near-four-dimensions.md), in coordinates $(g_1,g_2,\lambda)$, is

$$
\boxed{\frac{\epsilon}{A}\left\{\begin{gathered}
(0,0,0),\quad\left(\frac1{36},0,0\right),\quad\left(0,\frac1{36},0\right),\\
\left(\frac1{36},\frac1{36},0\right),\quad\left(\frac1{40},\frac1{40},\frac1{20}\right),\quad\left(\frac1{72},\frac1{72},\frac1{12}\right)
\end{gathered}\right\}}.
$$

The internal [symmetries](../../../../../../symmetry-physics.md) of these [renormalization-group fixed points](../../../../../../renormalization-group-fixed-point.md) are:

- The [Gaussian fixed point](../../../../../../gaussian-fixed-point.md) has an $O(2)$ [orthogonal group](../../../../../../orthogonal-group.md) acting on the two identical free massless fields.
- $(\epsilon/(36A),0,0)$ is one [Ising model](../../../../../../ising-model.md) [Wilson-Fisher fixed point](../../../../../../wilson-fisher-fixed-point.md) and one free field. Its linear internal [symmetry](../../../../../../symmetry-physics.md) is $\mathbb Z_2\times\mathbb Z_2$; the two sectors cannot be exchanged. The point $(0,\epsilon/(36A),0)$ has the same [symmetry](../../../../../../symmetry-physics.md) with the roles reversed.
- $(\epsilon/(36A),\epsilon/(36A),0)$ describes two identical decoupled [Ising models](../../../../../../ising-model.md). It additionally permits field exchange, giving $(\mathbb Z_2\times\mathbb Z_2)\rtimes S_2$, the eight-element [dihedral group](../../../../../../dihedral-group.md) $D_4$.
- $(\epsilon/(40A),\epsilon/(40A),\epsilon/(20A))$ has $\lambda=2g_1=2g_2$. Its interaction is $g(\phi_1^2+\phi_2^2)^2$, so it is the [O(N) model](../../../../../../o-n-model.md) [Wilson-Fisher fixed point](../../../../../../wilson-fisher-fixed-point.md) with $N=2$ and $O(2)$ [symmetry](../../../../../../symmetry-physics.md).
- $(\epsilon/(72A),\epsilon/(72A),\epsilon/(12A))$ has $\lambda=6g_1=6g_2$. Its [symmetry](../../../../../../symmetry-physics.md) is again the eight-element [dihedral group](../../../../../../dihedral-group.md) $D_4$, not $O(2)$.

The last point displays the [field-rotation equivalence of decoupled Ising theories](../../../../../../field-rotation-equivalence-of-decoupled-ising-theories.md). With the [orthogonal transformation](../../../../../../orthogonal-transformation.md) $\psi_\pm=(\phi_1\pm\phi_2)/\sqrt2$,

$$
g(\phi_1^4+\phi_2^4+6\phi_1^2\phi_2^2)=2g(\psi_+^4+\psi_-^4),\qquad 2g=\frac{\epsilon}{36A}.
$$

It is the same pair of decoupled [Ising models](../../../../../../ising-model.md) written in fields rotated by $45^\circ$, but remains a distinct coordinate solution of the stated [renormalization-group beta functions](../../../../../../beta-function-physics.md). Here $D_4$ denotes the [dihedral group](../../../../../../dihedral-group.md) of order eight; an alternative convention calls it $D_8$. We have described linear internal transformations preserving the [gradient energy](../../../../../../gradient-energy.md); free massless sectors also have constant [scalar-field shift symmetries](../../../../../../scalar-field-shift-symmetry.md). At $\epsilon=0$, the six coordinates coalesce at the [Gaussian fixed point](../../../../../../gaussian-fixed-point.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 303](../../../paper-303-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

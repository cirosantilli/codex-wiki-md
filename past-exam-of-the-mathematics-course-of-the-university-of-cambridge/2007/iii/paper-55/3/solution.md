<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Assume global [four-dimensional N=1 supersymmetry](../../../../../four-dimensional-n-1-supersymmetry.md) with canonical [kinetic terms](../../../../../kinetic-term.md) and no explicit [gaugino](../../../../../gaugino.md) mass. Write $W_i=\partial_iW$ and $W_{ij}=\partial_i\partial_jW$. To match the displayed stationarity equation, use $F^i=\overline{W_i}$; this differs by a minus sign from the eliminated [auxiliary field](../../../../../auxiliary-field.md) in the component convention of Solution 2. The real [D-terms](../../../../../d-term.md) are $D^a=-g^a(\bar\phi_i(T^a)^i{}_j\phi^j+\xi^a)$, with Hermitian [gauge generators](../../../../../gauge-generator.md). A constant [Fayet–Iliopoulos term](../../../../../fayet-iliopoulos-term.md) is permitted only for an appropriate Abelian factor. The [scalar potential](../../../../../scalar-potential.md) is

$$
V=W_i\overline{W_i}+\frac12\sum_a(D^a)^2.
$$

Differentiate with respect to $\phi^i$, holding $\bar\phi$ independent:

$$
\partial_iD^a=-g^a\bar\phi_j(T^a)^j{}_i,\qquad \partial_iV=W_{ij}F^j-\sum_ag^aD^a\bar\phi_j(T^a)^j{}_i.
$$

Thus [stationary point](../../../../../stationary-point.md) conditions gives the first requested identity. [Gauge invariance](../../../../../gauge-invariance.md) of the [superpotential](../../../../../superpotential.md) gives $W_i(T^a)^i{}_j\phi^j=0$. Conjugating it and using Hermiticity gives $\bar\phi_j(T^a)^j{}_iF^i=0$, the second condition in the form needed below.

At the vacuum, define $H_{ij}=\langle W_{ij}\rangle$ and $G_{ia}=g^a\langle\bar\phi_j\rangle(T^a)^j{}_i$. The two conditions combine as

$$
\boxed{M_0\begin{pmatrix}\langle F\rangle\\\langle D\rangle\end{pmatrix}=0,\qquad M_0=\begin{pmatrix}H&-G\\-G^T&0\end{pmatrix}.}
$$

Here the upper equation is stationarity and the lower equation is conjugated [gauge invariance](../../../../../gauge-invariance.md). The [chiral-superfield fermion mass matrix](../../../../../chiral-superfield-fermion-mass-matrix.md) contributes $-\frac12H_{ij}\psi^i\psi^j$, and the gauge [Yukawa interaction](../../../../../yukawa-interaction.md) contributes the mixed chiral-fermion/[gaugino](../../../../../gaugino.md) bilinear. With canonical [Weyl fermion](../../../../../weyl-spinor.md) and [gaugino](../../../../../gaugino.md) [kinetic terms](../../../../../kinetic-term.md), and choosing the [gaugino](../../../../../gaugino.md) phase to put the mixed bilinear in real-sign convention, these terms are

$$
\mathcal L_{\mathrm{mass}}=-\frac12\begin{pmatrix}\psi&\lambda\end{pmatrix}\mathcal M\begin{pmatrix}\psi\\\lambda\end{pmatrix}+\mathrm{h.c.},\qquad \mathcal M=\begin{pmatrix}H&-\sqrt2G\\-\sqrt2G^T&0\end{pmatrix}.
$$

The factor $\sqrt2$ is important: the [matrix](../../../../../matrix.md) directly acting on the printed $(F,D)$ is the same mass bilinear with rescaled [gauginos](../../../../../gaugino.md), rather than literally the canonical [matrix](../../../../../matrix.md). In detail, for $S=\operatorname{diag}(I,\sqrt2I)$,

$$
\mathcal M=SM_0S,\qquad \boxed{\mathcal M\begin{pmatrix}\langle F\rangle\\\langle D\rangle/\sqrt2\end{pmatrix}=0.}
$$

Since [supersymmetry breaking](../../../../../supersymmetry-breaking.md) makes this vector nonzero, there is at least one zero mass [eigenvalue](../../../../../eigenvalue.md). A normalized massless [fermion](../../../../../fermion.md) is

$$
\eta=\frac{\sum_i\langle F^i\rangle^*\psi^i+\sum_a\langle D^a\rangle\lambda^a/\sqrt2}{\left(\sum_i|\langle F^i\rangle|^2+\frac12\sum_a\langle D^a\rangle^2\right)^{1/2}}.
$$

With the consistent [gaugino](../../../../../gaugino.md) phase, the inhomogeneous vacuum [supersymmetry transformation](../../../../../supersymmetry-transformation.md) of $(\psi,\lambda)$ is proportional to the same vector $(F,D/\sqrt2)$. Therefore $\eta$ shifts by a nonzero constant times the transformation parameter: it is the [Goldstino](../../../../../goldstino.md), the [Goldstone fermion](../../../../../goldstino.md) of broken global [supersymmetry](../../../../../supersymmetry-split.md). The argument guarantees **at least one [Goldstino](../../../../../goldstino.md) zero mode**, not the absence of other massless fermions.

For the second calculation, first take only canonical [chiral superfields](../../../../../chiral-superfield.md) and [F-term](../../../../../f-term.md) breaking. At a stationary vacuum $v$, let $h=\phi-v$, $m_{ij}=W_{ij}(v)$ and

$$
A_{ij}=\sum_k\overline{W_{ki}}W_{kj},\qquad B_{ij}=\sum_k\overline{W_k}W_{kij}.
$$

These follow by differentiating $V=\sum_k|W_k|^2$ twice. The quadratic [scalar potential](../../../../../scalar-potential.md) is

$$
V^{(2)}=h^\dagger Ah+\frac12(h^TBh+\mathrm{h.c.}),\qquad A=m^\dagger m.
$$

The doubled scalar [mass matrix](../../../../../mass-matrix.md) has blocks

$$
M_s^2=\begin{pmatrix}A&B^\dagger\\B&A^T\end{pmatrix}.
$$

Transforming to the $2N$ canonically normalized real components of $h$ preserves its [trace](../../../../../matrix-trace.md), so the sum of real scalar mass squares is $\operatorname{tr}M_s^2=2\operatorname{tr}A$. The [Weyl fermion](../../../../../weyl-spinor.md) mass squares are the [eigenvalues](../../../../../eigenvalue.md) of $m^\dagger m=A$ and their sum is $\operatorname{tr}A$. Each Weyl mass eigenstate has two physical spin states. The printed [supertrace](../../../../../supertrace.md) has scalar sign $-1$ and fermion weight $+2$, hence

$$
\boxed{\operatorname{STr}M^2=-\operatorname{tr}M_s^2+2\operatorname{tr}(m^\dagger m)=-2\operatorname{tr}A+2\operatorname{tr}A=0.}
$$

The frequently used boson-minus-fermion definition has the opposite overall sign and gives the same zero. The mixing block $B$ can split scalar masses but cannot change this [trace](../../../../../matrix-trace.md). This proves the [tree-level supertrace mass sum rule](../../../../../tree-level-supertrace-mass-sum-rule.md); it uses canonical [kinetic terms](../../../../../kinetic-term.md) and a renormalizable global theory, rather than a general [supergravity](../../../../../supergravity.md) or noncanonical effective theory.

In the [MSSM](../../../../../minimal-supersymmetric-standard-model.md), trying to make all [squarks](../../../../../squark.md) and [sleptons](../../../../../slepton.md) heavy through direct canonical tree-level [F-term](../../../../../f-term.md) breaking encounters this constraint. In an unbroken electric-charge and color sector, the scalar mass-squared [trace](../../../../../matrix-trace.md) is twice the [trace](../../../../../matrix-trace.md) for its ordinary fermionic partners. More explicitly, take a unit vector $u$ minimizing $u^\dagger Au$. For $h=e^{i\alpha}u$, choose $\alpha$ so that $\operatorname{Re}(e^{2i\alpha}u^TBu)\leq0$. The curvature along this real scalar direction is then at most $u^\dagger Au$, so at least one scalar mass square is no larger than the smallest fermion mass square in that sector. For one isolated pair the scalar masses are $m_f^2\pm|B|$. Thus light [quarks](../../../../../quark.md) can force an unacceptably light [squark](../../../../../squark.md), or a tachyon, under these assumptions. A [hidden supersymmetry-breaking sector](../../../../../hidden-supersymmetry-breaking-sector.md) with mediation produces effective [soft supersymmetry breaking](../../../../../soft-supersymmetry-breaking.md); radiative effects, noncanonical [kinetic terms](../../../../../kinetic-term.md), or [supergravity](../../../../../supergravity.md) can change the assumptions and allow a viable spectrum. The [trace](../../../../../matrix-trace.md) over an arbitrary enlarged theory alone would not locate the light state in the visible sector; the MSSM conclusion uses the conserved-charge block structure.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

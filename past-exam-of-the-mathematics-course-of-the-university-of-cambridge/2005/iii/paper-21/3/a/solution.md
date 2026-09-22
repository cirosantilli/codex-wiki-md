<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For these [linear systems of divisors](../../../../../../linear-system-of-divisors.md), take a complex [K3 surface](../../../../../../k3-surface.md) $X$ and a nef big divisor $D$, so $D^2>0$. The exceptional terminology refers to the complete system $|D|$, rather than to an arbitrary subsystem.

A [monogonal linear system on a K3 surface](../../../../../../monogonal-linear-system-on-a-k3-surface.md) has the form

$$
D=mE+\Gamma,\qquad m\ge2,\quad
E^2=0,\quad E\Gamma=1,\quad\Gamma^2=-2,
\qquad |D|=\Gamma+|mE|,
$$

where $|E|$ is an [elliptic pencil on a K3 surface](../../../../../../elliptic-pencil-on-a-k3-surface.md) and $\Gamma$ is its section. Its intersection with an elliptic fibre is one, and its fixed part is $\Gamma$. For a concrete existence example, take the smooth [Fermat quartic surface](../../../../../../fermat-quartic-surface.md) $X\subseteq\mathbb P^3$ and two skew lines on it. Such lines can be written as

$$
\Gamma_0:\ x_0=\zeta x_1,\ x_2=\eta x_3,\qquad
\Gamma:\ x_0=\zeta' x_1,\ x_2=\eta' x_3,
$$

with $\zeta^4=(\zeta')^4=\eta^4=(\eta')^4=-1$, $\zeta\ne\zeta'$ and $\eta\ne\eta'$. The equations show that they are disjoint, and the four partial derivatives show that the quartic is smooth. The [adjunction formula](../../../../../../adjunction-formula.md) gives $K_X=0$, and the hypersurface [exact sequence of sheaves](../../../../../../exact-sequence-of-sheaves.md) $0\to\mathcal O_{\mathbb P^3}(-4)\to\mathcal O_{\mathbb P^3}\to\mathcal O_X\to0$, together with the intermediate [cohomology](../../../../../../cohomology-split.md) vanishing of these twists, gives $H^1(X,\mathcal O_X)=0$. Thus it is a [K3 surface](../../../../../../k3-surface.md), and each line has square $-2$. If $H$ is the hyperplane class, the planes through $\Gamma_0$ cut out $\Gamma_0$ plus a residual cubic pencil $|E|$, $E=H-\Gamma_0$. This pencil has no base point off $\Gamma_0$. On $\Gamma_0$, its two local residual equations are the two normal derivatives of the quartic equation; they cannot vanish simultaneously because $X$ is smooth. Thus it is [basepoint-free](../../../../../../basepoint-free-divisor.md), with

$$
E^2=4-2-2=0,\qquad E\Gamma=1.
$$

The degree-one map of $\Gamma$ to the pencil base makes it a section and forces connected fibres. [Bertini smoothness theorem](../../../../../../bertini-smoothness-theorem.md) and [adjunction formula](../../../../../../adjunction-formula.md) then make a general fibre a smooth genus-one curve.

Now choose $D=mE+\Gamma$. For every irreducible curve other than $\Gamma$, both $E$ and the effective curve $\Gamma$ have nonnegative intersection with it. Also $D\Gamma=m-2\ge0$, so $D$ is nef, and $D^2=2m-2>0$. On a general elliptic fibre, the restriction of $\mathcal O_X(D)$ is the degree-one bundle of the section point. Its unique section vanishes at that point. Every [global section](../../../../../../global-section.md) of $\mathcal O_X(D)$ therefore vanishes along a dense subset of $\Gamma$, hence along $\Gamma$ itself. Removing this fixed divisor gives exactly $|mE|$. This verifies the monogonal example directly; its general divisor is a section plus $m$ fibres.

A [hyperelliptic linear system on a K3 surface](../../../../../../hyperelliptic-linear-system-on-a-k3-surface.md) is a [basepoint-free](../../../../../../basepoint-free-divisor.md) nef big system whose morphism is generically two-to-one. Equivalently its general smooth curve is [hyperelliptic](../../../../../../hyperelliptic-curve.md). Let $\pi:X\to\mathbb P^2$ be a double cover branched over a smooth sextic, and put $D=\pi^*\mathcal O(1)$. The double-cover construction gives

$$
\pi_*\mathcal O_X=\mathcal O\oplus\mathcal O(-3),\qquad
K_X=\pi^*(K_{\mathbb P^2}+3H)=0,\qquad
H^1(X,\mathcal O_X)=0.
$$

Thus $X$ is a [K3 surface](../../../../../../k3-surface.md). Further,

$$
D^2=2,\qquad
H^0(X,D)=H^0(\mathbb P^2,\mathcal O(1)),
$$

since the second summand contributes $H^0(\mathcal O(-2))=0$. The map given by $|D|$ is precisely the double cover. A general member is the double cover of a line branched at six points, so [Riemann-Hurwitz formula](../../../../../../riemann-hurwitz-formula.md) gives [genus](../../../../../../genus-of-a-surface.md) two. This is the hyperelliptic example.

A [trigonal linear system on a K3 surface](../../../../../../trigonal-linear-system-on-a-k3-surface.md) is a [basepoint-free](../../../../../../basepoint-free-divisor.md) nonhyperelliptic nef big system whose general smooth curve has gonality three. For an example, take the same smooth quartic with a line $\Gamma_0$ and the hyperplane system $|H|$. Its general member is a [smooth plane quartic](../../../../../../smooth-plane-quartic.md) of [genus](../../../../../../genus-of-a-surface.md) three; [adjunction formula](../../../../../../adjunction-formula.md) identifies its plane embedding with its [canonical map](../../../../../../canonical-map.md), so it is not hyperelliptic. The elliptic pencil $E=H-\Gamma_0$ has

$$
H\cdot E=4-1=3.
$$

Its restriction to a general hyperplane curve is a [basepoint-free](../../../../../../basepoint-free-divisor.md) degree-three pencil. The curve is neither rational nor hyperelliptic, so its gonality is exactly three. This verifies the trigonal example.

Thus the three examples exhibit respectively **a fixed section with elliptic fibres, a double-plane map, and an embedded quartic with trigonal hyperplane sections**. The last example also illustrates why low-genus trigonal sections should not be confused with a blanket numerical criterion for every higher-genus model.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

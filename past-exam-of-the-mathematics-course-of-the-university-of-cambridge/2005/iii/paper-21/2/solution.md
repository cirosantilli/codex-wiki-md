<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Work over $\mathbb C$, and let $C$ be a [smooth projective curve](../../../../../smooth-projective-curve.md) of [genus](../../../../../genus-of-a-surface.md) $g\ge3$ and gonality three. A [trigonal curve](../../../../../trigonal-curve.md) has a [basepoint-free](../../../../../basepoint-free-divisor.md) degree-three pencil, giving a finite morphism $f:C\to\mathbb P^1$ of degree three. It is not [hyperelliptic](../../../../../hyperelliptic-curve.md), so its [canonical map](../../../../../canonical-map.md) is an embedding. Let $D_t=f^{-1}(t)$, including its scheme multiplicities. The complete pencil has $h^0(D_t)=2$, and [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives

$$
h^0(K_C-D_t)=g-2.
$$

Thus the quotient of canonical sections evaluated on $D_t$ has dimension two, and $D_t$ spans a line in $\mathbb P^{g-1}$. This argument includes ramified fibres, rather than treating only three distinct points.

These two-dimensional quotients vary in a globally generated rank-two bundle $E$ on $\mathbb P^1$. More explicitly, the image of

$$
H^0(C,K_C)\otimes\mathcal O_{\mathbb P^1}\longrightarrow f_*K_C
$$

has constant rank two by the preceding dimension count, so it is a subbundle. The equality of the rank at every fibre justifies the bundle construction. On [global sections](../../../../../global-section.md) it contains every canonical section, and therefore $H^0(\mathbb P^1,E)=H^0(C,K_C)$. The [Birkhoff–Grothendieck theorem](../../../../../birkhoff-grothendieck-theorem.md) gives

$$
E=\mathcal O(a_1)\oplus\mathcal O(a_2),
\qquad 0\le a_1\le a_2.
$$

Global generation forces nonnegative splitting degrees. Since $h^0(E)=a_1+a_2+2=g$,

$$
\boxed{a_1+a_2=g-2.}
$$

The natural map from $f^*E$ to $K_C$ is a [surjection](../../../../../surjective-function.md) at every point, since the canonical system has no base points. By [projectivization by quotients](../../../../../projectivization-by-quotients.md) it gives a map $C\to F=\mathbb P(E)$ over $\mathbb P^1$, with $M|_C=K_C$. Its composition with the tautological map of $F$ is the canonical embedding of $C$, so $C\to F$ is itself a closed embedding. Each fibre of the ruling maps to the spanning line of $D_t$; their union is the [canonical scroll of a trigonal curve](../../../../../canonical-scroll-of-a-trigonal-curve.md), and the ruling restricts to the given $g^1_3$.

Put $a=a_2-a_1$. Tensoring $E$ by $\mathcal O(-a_2)$ identifies the abstract ruled surface with $\mathbb F_a=\mathbb P(\mathcal O(-a)\oplus\mathcal O)$. The section coming from the quotient onto the smaller summand has self-intersection $-a$ and will be denoted by $B$. In this normalized presentation its tautological class is $B$; restoring the twist gives

$$
\boxed{M=B+a_2L.}
$$

This class gives the [scroll](../../../../../rational-normal-scroll.md) map. It is an embedding if $a_1>0$. When $a_1=0$, it contracts $B$; thus the printed embedding description needs this positivity qualification. For example, in [genus](../../../../../genus-of-a-surface.md) three the ruled model is $\mathbb F_1$ and its image is $\mathbb P^2$; in [genus](../../../../../genus-of-a-surface.md) four the type $(0,2)$ has a quadric-cone image. In both cases the smooth curve and its canonical image are still described by the construction above.

As a divisor on $F$, the curve meets each fibre in degree three, so $C=3M+tL$ for an integer $t$. The [scroll](../../../../../rational-normal-scroll.md) formula gives

$$
K_F=-2M+(g-4)L.
$$

By [adjunction formula](../../../../../adjunction-formula.md) and $M|_C=K_C$,

$$
(K_F+C-M)|_C=(g-4+t)L|_C=0.
$$

Taking degree on $C$ uses $\deg(L|_C)=3$ and gives $t=4-g$. Consequently

$$
C\in|3M+(4-g)L|
=|3B+(3a_2+4-g)L|
=|3B+(a+a_2+2)L|.
$$

Writing $d=a+a_2+2$, this is

$$
\boxed{C\in|3B+dL|,\qquad
d=\frac{g+3a+2}{2}.}
$$

A divisor $rB+dL$ with $r\ge0$ on $\mathbb F_a$ is [basepoint-free](../../../../../basepoint-free-divisor.md) when $d\ge ra$. Indeed, its pushforward along the ruling splits into

$$
\bigoplus_{j=0}^r\mathcal O_{\mathbb P^1}(d-ja);
$$

if each degree is nonnegative, sections generate these coefficient functions, and the fibre [monomials](../../../../../monomial.md) generate at every point. In particular $3B+dL$ is [basepoint-free](../../../../../basepoint-free-divisor.md) when $d\ge3a$. The [Bertini smoothness theorem](../../../../../bertini-smoothness-theorem.md) then makes its general member nonsingular, including the equality case, where the general member avoids $B$.

Conversely, if $d<3a$, then $(3B+dL)\cdot B=d-3a<0$, so every effective member contains $B$. Because the canonical [scroll](../../../../../rational-normal-scroll.md) has $a_1\ge0$,

$$
d=2a+a_1+2>2a.
$$

The residual system $|2B+dL|$ is [basepoint-free](../../../../../basepoint-free-divisor.md). Its general member $R$ does not contain $B$ and intersects it in

$$
R\cdot B=d-2a=a_1+2>0.
$$

Thus a general divisor in the original system is $B+R$ with intersecting components and is singular at an intersection point. The fixed component occurs exactly once for a general member, since $R$ is not forced to contain it. This proves both directions, with the canonical-scroll hypotheses retained:

$$
\boxed{|3B+(a+a_2+2)L|\text{ has a nonsingular general member}
\iff d\ge3a\iff 3a\le g+2.}
$$

This is also the bound on the [Maroni invariant](../../../../../maroni-invariant.md). Merely observing a fixed component would not by itself prove singularity; the positive intersection with its residual divisor is essential.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

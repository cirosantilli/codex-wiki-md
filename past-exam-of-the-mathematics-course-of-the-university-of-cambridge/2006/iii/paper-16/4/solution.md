<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the [short exact sequence](../../../../../short-exact-sequence.md) of coefficient groups

$$
0\longrightarrow\mathbb F_p\xrightarrow{\ j\ }\mathbb Z/p^2\xrightarrow{\ r\ }\mathbb F_p\longrightarrow0,\qquad j(\bar a)=\overline{pa},\quad r(\bar b)=\bar b\pmod p.
$$

The groups of [singular chains](../../../../../singular-chain.md) are free, so applying the cochain construction gives a [short exact sequence](../../../../../short-exact-sequence.md) of [cochain complexes](../../../../../cochain-complex.md). Its [long exact sequence in cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) has the required terms and reduction map $r_*$. Define the [Bockstein homomorphism](../../../../../bockstein-homomorphism.md) to be its [connecting homomorphism](../../../../../connecting-homomorphism.md).

Explicitly, represent $x$ by a mod-$p$ [cocycle](../../../../../cocycle.md) $a$ and lift it to an integral [singular cochain](../../../../../singular-cochain.md) $A$. Since $a$ is a [cocycle](../../../../../cocycle.md), $\delta A$ is divisible by $p$. Then

$$
\boxed{\beta(x)=\left[\frac{\delta A}{p}\bmod p\right].}
$$

This is exactly the lift-and-[coboundary](../../../../../coboundary.md) construction for the coefficient sequence above: the mod-$p^2$ [coboundary](../../../../../coboundary.md) of $A$ lies in the image of $j$. The quotient cochain is a [cocycle](../../../../../cocycle.md), since $\delta^2A=0$ and integral cochains have no $p$-torsion. Replacing $A$ by another lift adds $pC$ and changes the quotient by $\delta C$ modulo $p$; replacing the representative by a [coboundary](../../../../../coboundary.md) likewise leaves its [cohomology](../../../../../cohomology-split.md) class unchanged. Thus the definition is independent of choices.

A degree-zero [cocycle](../../../../../cocycle.md) is a function on points constant on each path component. Choose an integer representative for its value on each component. This produces an integral zero-[cocycle](../../../../../cocycle.md) lift, with zero [coboundary](../../../../../coboundary.md). Hence **the Bockstein vanishes on $H^0(X;\mathbb F_p)$ for every space**.

For a nonzero example in every positive degree $i$, take the [Moore space](../../../../../moore-space-algebraic-topology.md) $X=S^i\cup_p e^{i+1}$, attaching the cell by a map of [mapping degree](../../../../../degree-of-a-continuous-mapping.md) $p$. Its positive-degree integral [cellular cochain complex](../../../../../cellular-cochain-complex.md) has the differential $\mathbb Z\xrightarrow{p}\mathbb Z$ from degree $i$ to $i+1$; when $i=1$, the preceding differential from degree zero is zero. Modulo $p$ the displayed differential vanishes, and $H^i(X;\mathbb F_p)=H^{i+1}(X;\mathbb F_p)=\mathbb F_p$. Lift the degree-$i$ generator to the cellular cochain with value one. Its [coboundary](../../../../../coboundary.md) has value $p$, so dividing by $p$ gives the generator in degree $i+1$. Naturality of cellular and singular [cohomology](../../../../../cohomology-split.md) with coefficient sequences identifies this with the [Bockstein on a cyclic Moore space](../../../../../bockstein-on-a-cyclic-moore-space.md). Therefore **$\beta$ is nonzero, indeed an isomorphism, in the requested degree for every prime $p$**.

Finally take integral lifts $A,B$ of cocycles representing $x\in H^i(X;\mathbb F_p)$ and $y\in H^j(X;\mathbb F_p)$. Write $\delta A=pA_1$ and $\delta B=pB_1$. The cochain [cup product](../../../../../cup-product.md) obeys the graded Leibniz identity, so

$$
\delta(A\smile B)=p\bigl(A_1\smile B+(-1)^i A\smile B_1\bigr).
$$

Divide by $p$, reduce modulo $p$ and pass to [cohomology](../../../../../cohomology-split.md). This proves the [Bockstein derivation rule](../../../../../bockstein-derivation-rule.md)

$$
\boxed{\beta(xy)=(\beta x)y+(-1)^i x(\beta y).}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The short exact coefficient sequence

$$
0\longrightarrow\mathbb Z\xrightarrow{\times m}\mathbb Z
\longrightarrow\mathbb Z/m\longrightarrow0
$$

induces the integral [Bockstein homomorphism](../../../../../bockstein-homomorphism.md)

$$
\widetilde\beta:H^i(X;\mathbb Z/m)\longrightarrow H^{i+1}(X;\mathbb Z).
$$

If $\rho:H^{i+1}(X;\mathbb Z)\to H^{i+1}(X;\mathbb Z/m)$ is reduction modulo $m$, then

$$
\beta=\rho\circ\widetilde\beta.
$$

Equivalently, if an integral cochain $a$ lifts a modulo-$m$ cocycle and $\delta a=mb$, then $\widetilde\beta[a]=[b]$ and $\beta[a]=[b\bmod m]$.

For integral lifts $a,c$ of classes $x,y$, the [cup product](../../../../../cup-product.md) coboundary formula is

$$
\delta(a\smile c)=\delta a\smile c+(-1)^{|x|}a\smile\delta c.
$$

Dividing by $m$ and reducing modulo $m$ proves the [Bockstein derivation rule](../../../../../bockstein-derivation-rule.md)

$$
\beta(x\smile y)=\beta(x)\smile y+(-1)^{|x|}x\smile\beta(y).
$$

Now assume that the stated closed five-manifold $M$ exists. Its top integral cohomology makes it connected and orientable. The [long exact sequence from a coefficient sequence](../../../../../long-exact-sequence-from-a-coefficient-sequence.md) for multiplication by $p$ shows that

$$
\widetilde\beta:H^2(M;\mathbb Z/p)\xrightarrow{\sim}H^3(M;\mathbb Z)
$$

and that reduction $H^3(M;\mathbb Z)\to H^3(M;\mathbb Z/p)$ is an isomorphism. Hence

$$
\beta:H^2(M;\mathbb Z/p)\xrightarrow{\sim}H^3(M;\mathbb Z/p).
$$

The same coefficient sequence gives $H^4(M;\mathbb Z/p)=0$.

Choose $0\ne x\in H^2(M;\mathbb Z/p)$ and put $y=\beta x\ne0$. By [Poincare duality](../../../../../poincare-duality.md) over $\mathbb Z/p$, the pairing

$$
H^2(M;\mathbb Z/p)\otimes H^3(M;\mathbb Z/p)
\longrightarrow H^5(M;\mathbb Z/p)
$$

is nondegenerate. Both factors are one-dimensional, so $x\smile y\ne0$. But $x\smile x=0$ because $H^4(M;\mathbb Z/p)=0$, while the derivation rule and [graded commutativity of the cup product](../../../../../graded-commutativity-of-the-cup-product.md) give

$$
0=\beta(x\smile x)
=y\smile x+x\smile y
=2x\smile y.
$$

This contradicts $p>2$. Therefore no such manifold exists.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

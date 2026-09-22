<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Translate the rational [2-torsion](../../../../../../2-torsion.md) point to $(0,0)$ and clear denominators to obtain the integral [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md). Nonsingularity requires $b\ne0$ and $b'=a^2-4b\ne0$. The [two-isogeny descent](../../../../../../two-isogeny-descent.md) uses

$$
E':y^2=x(x^2-2ax+b'),\qquad
\phi(x,y)=\left(x+a+\frac bx,\ y\left(1-\frac b{x^2}\right)\right),
$$

and its [dual isogeny](../../../../../../dual-isogeny.md)

$$
\psi(X,Y)=\left(\frac{X-2a+b'/X}{4},\ \frac{Y(1-b'/X^2)}8\right).
$$

These formulas extend across their missing affine points as degree-two [isogenies of elliptic curves](../../../../../../isogeny-of-elliptic-curves.md), with kernels $\{O,(0,0)\}$ on their respective curves; substitution gives $\psi\phi=[2]$ and $\phi\psi=[2]$.

Define homomorphisms to the [square-class group of a field](../../../../../../square-class-group-of-a-field.md) $\mathbb Q^{\times}/(\mathbb Q^{\times})^2$ by

$$
\alpha(O)=1,\quad\alpha((0,0))=[b],\quad\alpha(x,y)=[x],
\qquad
\alpha'(O)=1,\quad\alpha'((0,0))=[b'],\quad\alpha'(X,Y)=[X].
$$

For ordinary intersections with a line, the product of the three first coordinates is the square of its intercept, proving the homomorphism identity; tangent cases use the same product with multiplicities. For $T=(0,0)$, direct addition gives $x(P+T)=b/x(P)$, so $\alpha(P+T)=[b]\alpha(P)$. Also $\alpha(P)\alpha(-P)=1$ and $\alpha(T)^2=1$, which handle inverse points and $T+T=O$. These verify the exceptional values as well. Their kernels are $\psi E'(\mathbb Q)$ and $\phi E(\mathbb Q)$. One can check the first assertion directly: if $x=s^2\ne0$, solving for the first coordinate of a preimage under $\psi$ gives

$$
X=a+2s^2\pm\frac{2y}{s},
$$

with rational corresponding ordinate. Conversely, on $E'$ one has $\psi_x=Y^2/(4X^2)$, a square. The exceptional point $(0,0)$ has a rational preimage exactly when $b$ is a square. The other kernel assertion follows identically, since the double companion curve is isomorphic to $E$ by scaling its coordinates by four and eight.

We now justify the rank factor in the [square-class index formula for two-isogeny descent](../../../../../../square-class-index-formula-for-two-isogeny-descent.md), rather than forgetting a torsion correction. Put $A=E(\mathbb Q)$, $B=E'(\mathbb Q)$, and

$$
\delta=[\ker\psi:\ker\psi\cap\phi A].
$$

The preimage of $\psi\phi A$ under $\psi$ is $\phi A+\ker\psi$, so

$$
[A:2A]=[A:\psi B]\,[\psi B:\psi\phi A]
=\frac{\#\alpha(A)\,\#\alpha'(B)}\delta.
$$

The [Mordell-Weil theorem](../../../../../../mordell-weil-group.md) gives $[A:2A]=2^r\#A[2]$, where $r$ is the [rank of an abelian group](../../../../../../rank-of-an-abelian-group.md) of $A$. If $b'$ is a square, $\#A[2]=4$ and $(0,0)\in\phi A$, so $\delta=1$. If it is not a square, $\#A[2]=2$ and $\delta=2$. Hence $\delta\#A[2]=4$ in both cases, and

$$
\boxed{2^r=\frac{\#\alpha(E(\mathbb Q))\,\#\alpha'(E'(\mathbb Q))}{4}.}
$$

To bound these two images, let $\ell\nmid b$ and take a point with $x\ne0$. If $v_\ell(x)>0$, then $x^2+ax+b$ is a unit, so $2v_\ell(y)=v_\ell(x)$ is even. If $v_\ell(x)<0$, the leading term $x^3$ uniquely has least [valuation](../../../../../../valuation.md) in the equation, so $2v_\ell(y)=3v_\ell(x)$ and again $v_\ell(x)$ is even. Thus every image class has a signed [square-free integer](../../../../../../square-free-integer.md) representative supported on the [prime](../../../../../../prime-number.md) divisors of $b$. The exceptional class $[b]$ also has that property. There are at most $2^{\nu(b)+1}$ such classes. Applying the same reasoning to $E'$ gives $\#\alpha'(B)\leq2^{\nu(b')+1}$. The [prime-support bound in two-isogeny descent](../../../../../../prime-support-bound-in-two-isogeny-descent.md) is therefore

$$
\boxed{r\leq\nu(b)+\nu(a^2-4b).}
$$

Here $\nu$ counts the distinct [prime](../../../../../../prime-number.md) divisors of the absolute value of a nonzero integer; $\nu(1)=\nu(-1)=0$. The nonsingularity hypotheses exclude the otherwise undefined case $\nu(0)$.

For the unheaded practical procedure, enumerate signed square-free divisors $d$ of $b$, and of $b'$ on the companion curve. A class $d$ is represented by a point of $E$ exactly when its [quartic covering in a two-isogeny descent](../../../../../../quartic-covering-in-a-two-isogeny-descent.md)

$$
C_d:\quad W^2=dU^4+aU^2V^2+\frac bdV^4
$$

has a rational solution with $(U,V)\ne(0,0)$. For $UV\ne0$, reconstruct $x=dU^2/V^2$, $y=dUW/V^3$; substitution verifies the equivalence. Solutions with $V=0$ or $U=0$ account for the identity class or the class of $(0,0)$ respectively. Clearing denominators allows integral $U,V,W$ with $\gcd(U,V)=1$.

Test these finitely many coverings over the real numbers and local fields, especially at two and the [primes](../../../../../../prime-number.md) dividing $bb'$, to exclude impossible classes. Search the survivors for [rational points](../../../../../../rational-point.md), close the witnessed classes under multiplication, and use the index formula once both images are determined. Equivalently, local solubility gives a descent upper bound and independent [rational points](../../../../../../rational-point.md), certified for example by their [canonical height of an elliptic curve](../../../../../../canonical-height-of-an-elliptic-curve.md) pairing, give a lower bound. When the bounds coincide the rank is determined. This procedure often succeeds, but local solubility alone does not prove global solubility: a nonzero [Tate–Shafarevich group](../../../../../../tate-shafarevich-group.md) can leave surviving coverings without [rational points](../../../../../../rational-point.md). In that case the computation gives a rigorous bound rather than a falsely certified exact rank.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

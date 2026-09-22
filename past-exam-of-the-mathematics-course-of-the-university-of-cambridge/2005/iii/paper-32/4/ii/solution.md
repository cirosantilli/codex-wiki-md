<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Retain $E:y^2=x(x^2+ax+b)$ and put $b'=a^2-4b$. The explicit [two-isogeny formula](../../../../../../two-isogeny-formula.md) is

$$
\phi(x,y)=\left(x+a+\frac bx,\ y\left(1-\frac b{x^2}\right)\right),\qquad
\psi(X,Y)=\left(\frac{X-2a+b'/X}{4},\ \frac{Y(1-b'/X^2)}8\right),
$$

with the maps extended at the kernel points. Direct substitution verifies the equations and $\psi\phi=[2]$.

Here is a concrete kernel test for the descent homomorphisms. A preimage of $(X,Y)\in E'$ has $x$ satisfying $x^2+(a-X)x+b=0$, whose discriminant is $(X-a)^2-4b$. The target equation says $Y^2=X((X-a)^2-4b)$, so for nonexceptional points this quadratic has a rational solution precisely when $X$ is a square. The resulting $y$ follows from the displayed [elliptic isogeny](../../../../../../isogeny-of-elliptic-curves.md) formula. For a nonzero target two-torsion point, the preimage quadratic has a double root $x=(X-a)/2$, and the source equation gives $y^2=x^2X$, so the same square condition still applies. At $(0,0)\in E'$, a rational preimage exists precisely when $b'$ is a square, matching the special square-class value $\alpha'((0,0))=[b']$. The dual argument gives the other kernel. Thus

$$
A:=\alpha(E(\mathbb Q))\cong E(\mathbb Q)/\psi E'(\mathbb Q),\qquad
B:=\alpha'(E'(\mathbb Q))\cong E'(\mathbb Q)/\phi E(\mathbb Q).
$$

Let $\delta=[\ker\psi:\ker\psi\cap\phi E(\mathbb Q)]$. The quotient map induced by $\psi$ has this kernel, giving

$$
[E(\mathbb Q):2E(\mathbb Q)]=\frac{\#A\,\#B}{\delta}.
$$

If $b'$ is a rational square, $E$ has four rational two-torsion points and $\delta=1$; otherwise it has two and $\delta=2$. In either case $\delta\,\#E(\mathbb Q)[2]=4$. Combining with finite generation therefore proves the [two-isogeny rank formula](../../../../../../square-class-index-formula-for-two-isogeny-descent.md)

$$
\boxed{2^{g_E}=\frac{\#A\,\#B}{4}.}
$$

This derivation checks the factor four, including curves with full rational two-torsion.

To compute these images, enumerate the signed square-free divisors $d$ of $b$ and $b'$. Substituting $x=d(U/V)^2$ yields the [quartic covering in a two-isogeny descent](../../../../../../quartic-covering-in-a-two-isogeny-descent.md)

$$
W^2=dU^4+aU^2V^2+(b/d)V^4,\qquad(U,V)\ne(0,0).
$$

The class $d$ occurs precisely when this covering has a [rational point](../../../../../../rational-point.md), with the identity and two-torsion handled by the boundary cases. Test at the real place and at primes dividing $2bb'$ to rule out candidates, and search for [rational points](../../../../../../rational-point.md) to prove that surviving classes occur. The locally soluble classes form a finite [elliptic isogeny](../../../../../../isogeny-of-elliptic-curves.md) [Selmer group of an elliptic curve](../../../../../../n-selmer-group.md), giving an upper rank bound. [rational points](../../../../../../rational-point.md) and independent height pairings give a lower bound. When the bounds agree the rank is proved. **Local solubility alone does not prove a [rational point](../../../../../../rational-point.md) exists**: if a gap remains, a higher descent or further information about the covering obstructions is needed. This is why the procedure usually computes the rank but is not an unjustified universal termination claim.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Start with an [elliptic curve](../../../../../elliptic-curve.md) having a rational point $T$ of order $2$. Move that point to $(0,0)$ and take an integral model

$$
E:y^2=x(x^2+ax+b),\qquad a,b\in\mathbb Z,\quad b(a^2-4b)\ne0.
$$

Put $b'=a^2-4b$ and

$$
E':Y^2=X(X^2-2aX+b').
$$

The [two-isogeny formula](../../../../../two-isogeny-formula.md) and its dual are

$$
\phi(x,y)=\left(x+a+\frac bx,\ y\left(1-\frac b{x^2}\right)\right),
$$



$$
\widehat\phi(X,Y)=\left(\frac{X-2a+b'/X}{4},\ \frac{Y(1-b'/X^2)}8\right).
$$

They extend to the projective curves, with kernels $\{O,T\}$ and $\{O,T'\}$, where $T'=(0,0)\in E'$. Substitution verifies their target equations, and the [elliptic-curve addition formula](../../../../../elliptic-curve-addition-formula.md) verifies $\widehat\phi\phi=[2]$ and $\phi\widehat\phi=[2]$. The division by $4,8$ in the dual identifies the twice-transformed curve, with coefficients $4a,16b$, with $E$.

Define the [two-torsion square-class homomorphisms](../../../../../two-torsion-square-class-homomorphism.md)

$$
\alpha(O)=1,\quad\alpha(T)=[b],\quad\alpha(x,y)=[x],
$$



$$
\alpha'(O)=1,\quad\alpha'(T')=[b'],\quad\alpha'(X,Y)=[X].
$$

Question 1(ii) proves these are homomorphisms, since $f'(0)=b$. Their kernels are

$$
\boxed{\ker\alpha=\widehat\phi(E'(\mathbb Q)),\qquad\ker\alpha'=\phi(E(\mathbb Q)).}
$$

For completeness, the first coordinate of the dual is $Y^2/(4X^2)$, so a nonexceptional dual image has square $x$-coordinate. Conversely, if $x=u^2\ne0$, the preimage equation is

$$
X^2-(4x+2a)X+b'=0,
$$

whose discriminant is $16(x^2+ax+b)=16(y/u)^2$. The roots $X=2x+a\pm2y/u$ are rational and nonzero. Choosing $Y=\pm2uX$ gives a point on $E'$, and a choice of sign makes its dual image exactly $(x,y)$. The point $T$ has a rational dual preimage precisely when $b$ is a square, as seen from the roots $a\pm2\sqrt b$ of the nonzero two-torsion polynomial on $E'$. The identity is already a dual image. Applying this argument to the transformed curve proves the second kernel assertion as well, because scaling an $x$-coordinate by $4$ does not change its [square class](../../../../../square-class.md).

The [two-isogeny descent](../../../../../two-isogeny-descent.md) is finite because an image square class has a signed [square-free integer](../../../../../square-free-integer.md) representative dividing $b$. Indeed, if $\ell\nmid b$ and $v_\ell(x)>0$, the other factor $x^2+ax+b$ is a unit, so $v_\ell(y^2)=v_\ell(x)$ forces an even valuation. If $v_\ell(x)<0$, the term $x^2$ dominates that factor and $v_\ell(y^2)=3v_\ell(x)$, again forcing even valuation. Thus odd valuations can occur only at primes dividing $b$. The same argument applies to $b'$ on $E'$.

For each candidate signed squarefree divisor $d\mid b$, put $x=d(U/V)^2$, with coprime integers $U,V$. The curve equation becomes the [two-isogeny descent quartic](../../../../../quartic-covering-in-a-two-isogeny-descent.md)

$$
\boxed{N^2=dU^4+aU^2V^2+(b/d)V^4.}
$$

A solution with $UV\ne0$ yields $x=dU^2/V^2$ and $y=dUN/V^3$. Conversely, every point in that class gives such a primitive integer solution, since a rational square root of an integer is integral. The boundary solutions $U=0$ and $V=0$ account respectively for the classes of $T$ and $O$. Rational solutions prove that a class occurs; a real or congruence obstruction excludes it. Merely finding local solutions everywhere does not automatically prove a rational solution.

To extract the rank, write $A=\alpha(E(\mathbb Q))$ and $A'=\alpha'(E'(\mathbb Q))$. The [Mordell-Weil theorem](../../../../../mordell-weil-group.md) gives

$$
|E(\mathbb Q)/2E(\mathbb Q)|=2^r|E(\mathbb Q)[2]|.
$$

The isogeny factorization gives the index $|A|$ for the first quotient by $\widehat\phi E'$. For the remaining index, apply $\widehat\phi$ to $E'/\phi E$. Its kernel has size $2/e$, where

$$
e=|\ker\widehat\phi\cap\phi E(\mathbb Q)|=|\phi(E(\mathbb Q)[2])|=|E(\mathbb Q)[2]|/2.
$$

The equality follows because $\widehat\phi(\phi P)=2P$. Consequently

$$
|E/2E|=|A|\,|A'|\,e/2=|A|\,|A'|\,|E[2]|/4,
$$

and cancellation yields the [two-isogeny rank formula](../../../../../square-class-index-formula-for-two-isogeny-descent.md)

$$
\boxed{2^r=\frac{|A|\,|A'|}{4}.}
$$

This formula is valid whether there is just one rational nonzero two-torsion point or all three.

For the first curve, $a=-1,b=1$, and the isogenous curve is

$$
E':Y^2=X(X^2+2X-3).
$$

The only candidate square classes on $E$ are $1,-1$. Since $x^2-x+1>0$ for every real $x$, a real affine point has $x\geq0$; the exceptional torsion class is $[b]=1$. Thus

$$
A=\{1\}.
$$

On $E'$, the candidates are $1,-1,3,-3$. They all occur: the identity gives $1$, $T'$ gives $-3$, $(3,6)$ gives $3$, and $(-1,2)$ gives $-1$. Hence $|A'|=4$, and

$$
\boxed{\operatorname{rank}\bigl(y^2=x(x^2-x+1)\bigr)=0.}
$$

The product in the rank formula is $1\cdot4=4$, not $1\cdot2$; all four classes on the companion curve are essential.

For the second curve, $a=5,b=-6$, and

$$
E':Y^2=X(X^2-10X+49).
$$

The candidate classes on $E$ are $\{\pm1,\pm2,\pm3,\pm6\}$. The identity, $T$, $(2,4)$ and $(-3,6)$ show that

$$
\{1,-6,2,-3\}\subseteq A.
$$

This is a subgroup of order $4$. Its other coset is $\{3,6,-1,-2\}$, so it suffices to exclude the representative $3$.

The [modulo-eight obstruction to a two-isogeny descent class](../../../../../modulo-eight-obstruction-to-a-two-isogeny-descent-class.md) uses the corresponding [two-isogeny descent quartic](../../../../../quartic-covering-in-a-two-isogeny-descent.md),

$$
N^2=3U^4+5U^2V^2-2V^4,\qquad\gcd(U,V)=1.
$$

If both $U,V$ are odd, its right side is $6$ modulo $8$. If $U$ is odd and $V$ even, it is $3$ or $7$ modulo $8$. If $U$ is even and $V$ odd, it is $6$ or $2$ modulo $8$. These are all primitive parity cases, and none is a square modulo $8$. Hence the class $3$ is impossible. Since $A$ is a subgroup, every class in its coset is impossible, and therefore

$$
\boxed{A=\{1,2,-3,-6\},\qquad |A|=4.}
$$

On the companion curve, the only candidates are $\pm1,\pm7$. Its quadratic factor is $(X-5)^2+24>0$, so every nonzero real affine $X$ is positive. The exceptional value $[49]$ is $1$, and the point $(7,14)$ supplies the class $7$. Thus

$$
\boxed{A'=\{1,7\},\qquad |A'|=2.}
$$

The rank formula gives $2^r=4\cdot2/4=2$, so

$$
\boxed{\operatorname{rank}\bigl(y^2=x(x^2+5x-6)\bigr)=1.}
$$

Every included class has an explicit rational representative and every excluded coset has a proved real or congruence obstruction, so these are exact ranks rather than bounds obtained from a point search.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 125](../../paper-125-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

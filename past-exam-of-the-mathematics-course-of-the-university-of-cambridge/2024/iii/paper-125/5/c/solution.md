<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [three-isogeny descent](../../../../../../three-isogeny-descent.md) connecting map, identified through the [Weil pairing](../../../../../../weil-pairing.md) with $H^1(\mathbb Q,\mu_3)=\mathbb Q^\times/(\mathbb Q^\times)^3$, is

$$
\alpha:E'(\mathbb Q)\longrightarrow
\mathbb Q^\times/(\mathbb Q^\times)^3.
$$

The long exact sequence attached to $0\to E[\phi]\to E\xrightarrow{\phi}E'\to0$ makes it a group homomorphism with

$$
\ker\alpha=\phi E(\mathbb Q).
$$

The function $f=y$ from part (b) gives the explicit formula

$$
\alpha(O)=1,
\qquad
\alpha(T)=d^{-1}=d^2\pmod{(\mathbb Q^\times)^3},
\qquad
\alpha(x,y)=y\pmod{(\mathbb Q^\times)^3}quad(P\ne O,T).
$$

At $T$, the value $d^{-1}$ is the leading coefficient of $y$ relative to the local parameter $x$, since $y(y+d)=x^3$ gives $y/x^3\to d^{-1}$. At $-T=(0,-d)$ the ordinary formula gives $-d$, whose class is the inverse of $d^{-1}$ because $-1$ is a cube.

Let $S$ be the primes dividing $d$. For a prime $\ell\notin S$, use

$$
y(y+d)=x^3.
$$

If $v_\ell(y)>0$, then $y+d$ is an $\ell$-adic unit, so $v_\ell(y)=3v_\ell(x)$. If $v_\ell(y)<0$, then $v_\ell(y+d)=v_\ell(y)$, so $2v_\ell(y)=3v_\ell(x)$. In either case $v_\ell(y)$ is divisible by three; the special values at $O$ and $T$ have the same property. Therefore

$$
\boxed{\operatorname{im}\alpha\subseteq\mathbb Q(S,3).}
$$

When $d=1$, this power-class group is trivial: a rational number whose valuation at every prime is divisible by three is a cube up to sign, and $-1=(-1)^3$. Thus $\alpha$ is trivial, its kernel is all of $E'(\mathbb Q)$, and

$$
\boxed{\phi:E(\mathbb Q)\twoheadrightarrow E'(\mathbb Q).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

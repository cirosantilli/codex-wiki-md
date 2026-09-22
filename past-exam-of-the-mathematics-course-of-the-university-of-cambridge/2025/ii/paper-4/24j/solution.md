<h1 id="24j/solution">Solution</h1>

↑ **Parent:** [24J](../24j.md)

For a divisor $D$ on a smooth projective curve $X$, define

$$
L(D)=\{h\in k(X)^\times:(h)+D\geq0\}\cup\{0\},
\qquad
\ell(D)=\dim_kL(D).
$$

The [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) states

$$
\boxed{\ell(D)-\ell(K_X-D)=\deg D+1-g},
$$

where $K_X$ is the divisor of a nonzero rational differential, $g$ is the genus of $X$, and $\deg D$ is the sum of the divisor coefficients because the ground field is algebraically closed.

Under the coordinate change $u=1/x$ and $v=y/x^n$, we have

$$
v^2=\frac{y^2}{x^{2n}}
=u^{2n}f(1/u).
$$

Hence

$$
\boxed{g(u)=u^{2n}f(1/u)}.
$$

This is a polynomial, and its value at zero is the nonzero leading coefficient of $f$. Thus the [even-degree hyperelliptic model](../../../../../even-degree-hyperelliptic-model.md) has two points $P_+,P_-$ above $u=0$, distinguished by the two values of $v$.

Consider the rational differential

$$
\omega=\frac{dx}{y}.
$$

At a finite branch point $x=a$, square-freeness gives a local parameter $y$, with $x-a$ a nonzero constant times $y^2$ to first order. Hence $dx/y$ is regular and nonzero there. It is also regular and nonzero at finite unramified points.

At infinity,

$$
dx=-u^{-2}du,
\qquad
y=vu^{-n},
$$

so

$$
\omega=-\frac{u^{n-2}}v\,du.
$$

Because $v(P_\pm)\ne0$ and $u$ is a local parameter at each point, $\omega$ has a zero of order $n-2$ at both. Therefore the [canonical divisor of an even-degree hyperelliptic curve](../../../../../canonical-divisor-of-an-even-degree-hyperelliptic-curve.md) is

$$
\boxed{K_X=(\omega)=(n-2)(P_++P_-)},
$$

and

$$
\boxed{\deg K_X=2n-4}.
$$

Since $\deg K_X=2g-2$, it follows that

$$
2g-2=2n-4,
\qquad
\boxed{g=n-1}.
$$

The function $x$ has a simple pole at each of $P_+$ and $P_-$. Consequently

$$
1,x,x^2,\ldots,x^{n-2}\in L(K_X).
$$

These $n-1$ functions are linearly independent. Riemann-Roch with $D=K_X$ gives $\ell(K_X)=g=n-1$, so

$$
\boxed{L(K_X)=\operatorname{span}_k\{1,x,\ldots,x^{n-2}\}}.
$$

With respect to this basis, the [canonical map of a hyperelliptic curve](../../../../../canonical-map-of-a-hyperelliptic-curve.md) is

$$
(x,y)\longmapsto[1:x:x^2:\cdots:x^{n-2}].
$$

It identifies $(x,y)$ with $(x,-y)$ for general $x$, and hence is not an embedding.

If $X$ embedded in $\mathbb P^2$, its smooth plane image would have degree $d\geq4$: degrees one and two have genus zero, and degree three has genus one, whereas $g=n-1\geq2$. But the [canonical map of a smooth plane curve](../../../../../canonical-map-of-a-smooth-plane-curve.md) of degree $d\geq4$ is an embedding by adjunction, contradicting the preceding calculation. Therefore

$$
\boxed{X\text{ cannot be embedded in }\mathbb P^2}.
$$

## ↑ Ancestors (10)

1. [24J](../24j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

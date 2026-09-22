<h1 id="34e/solution">Solution</h1>

↑ **Parent:** [34E](../34e.md)

For $N=1$, write

$$
q=\exp\left(-2lX-\frac{T}{2l}\right).
$$

The given evolution of the [discrete scattering data](../../../../../discrete-scattering-data.md) gives

$$
\lambda_1=il,
\qquad
c_1(T)=2l\exp\left(-\frac{T}{2l}\right).
$$

Solving the resulting two scalar linear equations for the components of $\psi_1$ and substituting in the reconstruction formula gives

$$
u_X=-\frac{8lq}{1+q^2}.
$$

Choosing the additive multiple of $2\pi$ so that $u\to0$ as $X\to+\infty$ and [integrating](../../../../../integral.md) in $X$ yields the [One-soliton solution of the sine-Gordon equation in light-cone coordinates](../../../../../one-soliton-solution-of-the-sine-gordon-equation-in-light-cone-coordinates.md)

$$
\boxed{u(X,T)=4\arctan\exp\left(-2lX-\frac{T}{2l}\right)}.
$$

It depends only on $X+T$ exactly when the two positive coefficients in the exponent agree:

$$
2l=\frac1{2l}.
$$

The unique positive solution is $l=1/2$, and then

$$
u(X,T)=F(X+T),
\qquad
\boxed{F(z)=4\arctan(e^{-z})}.
$$

The transformations satisfy $g^s g^r=g^{s+r}$, $g^0$ is the [identity map](../../../../../identity-function.md), and $(g^s)^{-1}=g^{-s}$, so they form a [one-parameter group](../../../../../group-split.md). If

$$
U(X,T)=u(e^{-s}X,e^sT),
$$

then the [chain rule](../../../../../chain-rule.md) gives

$$
U_{XT}=e^{-s}e^s u_{XT}=\sin U.
$$

Thus $g^s$ is a [Lie point symmetry](../../../../../lie-point-symmetry.md). Applied to the one-soliton family, it replaces $l$ by $l'=e^{-s}l$. Taking $e^s=2l$ gives $l'=1/2$, so every member is transformed to the function $F(X+T)$ found above.

For the stated $N=2$ solution, set $x=X+T$ and $t=T-X$. When $l^2+m^2=1/4$, its two arguments reduce to

$$
2mX-\frac{2mT}{4(l^2+m^2)}=-2mt,
\qquad
\frac{2lT}{4(l^2+m^2)}+2lX=2lx.
$$

At fixed $x$, only $\sin(2mt)$ varies, so the [Sine-Gordon breather](../../../../../sine-gordon-breather.md) has fundamental period

$$
\boxed{\mathcal T=\frac{\pi}{m}}.
$$

Finally put $r^2=l^2+m^2$. Under the same symmetry, the parameters become

$$
l'=e^{-s}l,
\qquad
m'=e^{-s}m,
$$

and hence $(l')^2+(m')^2=e^{-2s}r^2$. Choosing $e^s=2r$ makes this sum $1/4$, proving that every solution in the family is symmetry-equivalent to the normalized breather.

## ↑ Ancestors (10)

1. [34E](../34e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

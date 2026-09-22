<h1 id="14e/solution">Solution</h1>

↑ **Parent:** [14E](../14e.md)

For a nonzero [holomorphic function](../../../../../holomorphic-function.md), isolated boundary zeros produce only integrable logarithmic singularities: locally a zero of multiplicity $m$ contributes $m\log|\theta-\theta_0|$ plus a bounded term. Thus the circle means below are well-defined. The identically zero function may be assigned $J=-\infty$.

**1. Multiplication.** The pointwise identity $\log|F_1F_2|=\log|F_1|+\log|F_2|$ gives $J(F_1F_2,R)=J(F_1,R)+J(F_2,R)$ by integration, with the same extended interpretation if a factor is identically zero.

**2. Zero-free normalized functions.** [Compactness](../../../../../compact-space.md) lets us choose a slightly larger open disc on which $F$ is holomorphic and zero-free. On this [simply connected](../../../../../simply-connected-space.md) disc, $F'/F$ has a holomorphic primitive $L$ normalized by $L(0)=0$. Differentiating $Fe^{-L}$ shows it is constant and equal to $F(0)=1$, so $F=e^L$ and $L$ is a [holomorphic logarithm](../../../../../holomorphic-logarithm.md) of $F$. The [Cauchy integral formula](../../../../../cauchy-integral-formula.md) gives

$$
\frac1{2\pi}\int_0^{2\pi}L(Re^{i\theta})\,d\theta
=\frac1{2\pi i}\oint_{|z|=R}\frac{L(z)}z\,dz=L(0)=0.
$$

Taking real parts, using $\Re L=\log|F|$, proves **$J(F,R)=0$**. For a zero-free function with arbitrary nonzero value at zero, applying this to $F/F(0)$ gives $J(F,R)=\log|F(0)|$.

**3. Disc factors.** For $|z|=R$,

$$
|R^2-\overline wz|^2=R^2|z-w|^2,
$$

as follows by expansion and $|z|^2=R^2$. The denominator's possible zero is at $R^2/\overline w$, outside the closed disc; when $w=0$ it is constant. Thus the given [Blaschke factor](../../../../../blaschke-factor.md) is holomorphic on a neighbourhood of the disc, has modulus one on its boundary and satisfies $J(\psi_{w,R},R)=0$.

For the general formula, a nonzero [entire function](../../../../../entire-function.md) has finitely many zeros in the compact disc: an infinite set would have an accumulation point in a holomorphic neighbourhood and the [identity theorem](../../../../../identity-theorem.md) would make the function zero identically. List its interior zeros with multiplicities. When $F(0)\ne0$, divide by their factors $\psi_{w_j,R}$ to obtain a [holomorphic function](../../../../../holomorphic-function.md) $G$ zero-free on a neighbourhood of the disc. The preceding parts give $J(F,R)=J(G,R)=\log|G(0)|$, while $\psi_{w_j,R}(0)=-w_j/R$. Hence [Jensen's formula](../../../../../jensen-s-formula.md) is

$$
\boxed{J(F,R)=\log|F(0)|+\sum_{|w_j|<R}\log\frac R{|w_j|}\quad(F(0)\ne0).}
$$

The source does not explicitly rule out a zero at zero in this general step. If its order there is $m$ and $F(z)=z^mF_*(z)$ with $F_*(0)\ne0$, the correct version is

$$
\boxed{J(F,R)=m\log R+\log|F_*(0)|+\sum_{0<|w_j|<R}\log\frac R{|w_j|},\qquad
F_*(0)=\frac{F^{(m)}(0)}{m!}.}
$$

Thus a formula using $\log|F(0)|$ alone requires the indicated nonzero-centre assumption.

Finally, the lattice hypothesis forces quadratic exponential growth. For $R\geq8$, all integer pairs with $|j|,|k|\leq\lfloor R/4\rfloor$ lie inside the disc of radius $R/2$. Excluding zero, there are at least $R^2/16$ such points, and each contributes at least $\log2$ to Jensen's sum. Therefore

$$
J(F,R)\geq C+\frac{\log2}{16}R^2
$$

for boundary-zero-free radii, with the additional nonnegative $m\log R$ term if needed. For all sufficiently large such radii, this is at least $(\log2)R^2/32$. Choose $R_j\to\infty$ avoiding zero moduli and choose $z_j$ on each circle where $|F|$ is maximal. The logarithm of this circle maximum is at least the logarithmic circle mean, so

$$
\boxed{|F(z_j)|>\exp(c|z_j|^2),\qquad c=\frac{\log2}{64}>0.}
$$

This proves [lattice zeros force quadratic exponential growth](../../../../../lattice-zeros-force-quadratic-exponential-growth.md); the smaller constant makes the required inequality strict.

## ↑ Ancestors (10)

1. [14E](../14e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

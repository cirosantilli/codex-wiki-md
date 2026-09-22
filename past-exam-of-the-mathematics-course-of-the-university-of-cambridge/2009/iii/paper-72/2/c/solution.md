<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the method to the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md), put $z=h\lambda$, and retain every root of its [amplification polynomial of a multistep method](../../../../../../amplification-polynomial-of-a-multistep-method.md):

$$
P_z(w)=\left[1-\frac{1+a}{2}z\right]w^2
-\left[1+a+\frac{1-3a}{2}z\right]w+a.
$$

An [A-stable](../../../../../../a-stability.md) convergent method must satisfy the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) for every $\operatorname{Re}z\leq0$.

First take $-1<a<0$. As negative real $z$ tends to minus infinity, one root tends to the nonzero root of $\sigma$,

$$
w_\infty=\frac{3a-1}{1+a},\qquad |w_\infty|>1.
$$

It follows by root continuity that some sufficiently negative finite $z$ is unstable. At $a=-1$, the recurrence has [polynomial](../../../../../../polynomial-split.md) $w^2-2zw-1$; for any negative real $z$, its root $z-\sqrt{z^2+1}$ is below $-1$. Thus all negative convergent parameters are excluded.

For $0\leq a<1$, use the [boundary-locus test for multistep A-stability](../../../../../../boundary-locus-test-for-multistep-a-stability.md). A unit root $w=e^{i\theta}$ with $\sigma(w)\ne0$ would require $z=\rho(w)/\sigma(w)$. Direct multiplication by the conjugate denominator gives

$$
\operatorname{Re}\frac{\rho(e^{i\theta})}{\sigma(e^{i\theta})}
=\frac{a(1+a)(1-\cos\theta)^2}{|\sigma(e^{i\theta})|^2}\geq0.
$$

There is therefore no unit-root crossing in the open left half-plane. The leading coefficient of $P_z$ never vanishes there, since its only zero is the positive real value $2/(1+a)$. For a small negative real $z$, the simple root initially at one moves to $1+z+O(z^2)$, inside the disk, and the other root is close to $a$, also inside. Continuity of [polynomial](../../../../../../polynomial-split.md) roots and connectedness of the open left half-plane then keep both roots strictly inside throughout that half-plane. Possible zeros of $\sigma$ cause no omitted crossing: for $a>0$ its other root lies strictly inside the [unit disk](../../../../../../unit-disk.md), while at $a=0$ its unit-circle zero $w=-1$ has $\rho(-1)\ne0$.

On the imaginary axis, if $a>0$ the displayed real part vanishes only at $w=1$, which corresponds to $z=0$ and is simple. Other imaginary-axis parameters retain strictly interior roots. If $a=0$, the two roots are zero and the [stability function](../../../../../../stability-function.md) $(1+z/2)/(1-z/2)$, whose modulus is one on that axis; the unit root is simple. Thus the required boundary [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) holds as well.

Combining necessity and sufficiency gives

$$
\boxed{\text{The convergent A-stable members are exactly }0\leq a<1.}
$$

In particular, the third-order member $a=-1/5$ is convergent but not [A-stable](../../../../../../a-stability.md), in agreement with the [Second Dahlquist barrier](../../../../../../second-dahlquist-barrier.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

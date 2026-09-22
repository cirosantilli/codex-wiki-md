<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

If $\phi$ is identically zero there are no exceptions. Otherwise choose $x_0$ with $\phi(x_0)>0$ and put $I_+=\{x\ge x_0:\phi'(x)>\phi(x)^2\}$. Monotonicity implies $\phi(x)>0$ thereafter. On this set, $1<\phi'/\phi^2$, whence

$$
|I_+|\le\int_{I_+}\frac{\phi'}{\phi^2}\,dx\le\int_{x_0}^\infty\frac{\phi'}{\phi^2}\,dx
=\frac1{\phi(x_0)}-\lim_{X\to\infty}\frac1{\phi(X)}\le\frac1{\phi(x_0)}.
$$

Adding the finite initial interval $[0,x_0]$ proves

$$
\boxed{\phi'(x)\le\phi(x)^2\quad\text{outside a set of finite measure}.}
$$

This [derivative growth outside a finite-measure set](../../../../../derivative-growth-outside-a-finite-measure-set.md) controls exceptional radii in Nevanlinna estimates. For example let $T_s$ be the smooth spherical characteristic and $A(r)=rT_s'(r)$ its increasing area-counting function. Apply the lemma to $T_s+1$ and $A+1$: outside the union of two finite-measure sets,

$$
A(r)\le r(T_s(r)+1)^2,\qquad A'(r)\le(A(r)+1)^2.
$$

Their logarithms are consequently $O(\log r+\log(T_s+1))$. Such [derivative](../../../../../derivative.md)/area bounds in estimates from the [Poisson-Jensen formula](../../../../../poisson-jensen-formula.md) give the [Nevanlinna logarithmic derivative lemma](../../../../../nevanlinna-logarithmic-derivative-lemma.md), $m(r,f'/f)=O(\log^+T_f+\log r)$ outside a finite-length set. The second main theorem uses that estimate as its error term. The elementary growth lemma controls that error and its exceptional set; it is not itself a substitute for the analytic estimates.

We use the truncated second main theorem stated in the preceding solution, together with the fact that a transcendental [meromorphic function](../../../../../meromorphic-function.md) has $T_f(r)/\log r\to\infty$. Here is a justification of the latter fact. If there are infinitely many [poles](../../../../../pole.md), fixing any arbitrarily large finite [pole](../../../../../pole.md) count gives $N(r;\infty)\ge A\log r-O_A(1)$. If there are only finitely many [poles](../../../../../pole.md), multiply by a [polynomial](../../../../../polynomial-split.md) $p$ removing them to obtain a transcendental entire function $h=pf$. Its [Taylor series](../../../../../taylor-series.md) has nonzero coefficients of arbitrarily high degrees $n$. Cauchy's coefficient estimate gives $\log M_h(r/2)\ge n\log r-O_n(1)$; the [subharmonic function](../../../../../subharmonic-function.md) Poisson estimate gives $\log M_h(r/2)\le3m(r,h)$. Since $T_h\le T_f+O(\log r)$, letting $n$ be arbitrarily large proves the claimed ratio limit. Thus the second-theorem error is $o(T_f)$ along large nonexceptional radii.

Let $N_{\rm simple}(r;a)$ count just the simple $a$-points. A multiple $a$-point of degree $m\ge2$ contributes one to the truncated count and at least two to the full count; a simple point contributes one to each. Hence, with the same positive logarithmic weights for large radii,

$$
\overline N(r;a)\le\tfrac12N(r;a)+\tfrac12N_{\rm simple}(r;a).
$$

If each of the five values had only finitely many simple preimages, each simple counting function would be $O(\log r)$. Summing and using the first main theorem would give $\sum_{j=1}^5\overline N(r;a_j)\le(5/2)T_f+O(\log r)$. But the second theorem requires $3T_f\le\sum\overline N+o(T_f)$, a contradiction. This proves the stronger result [five values force infinitely many simple preimages](../../../../../five-values-force-infinitely-many-simple-preimages.md):

$$
\boxed{\text{At least one of the five values has infinitely many simple preimages.}}
$$

In particular **more than one simple zero is necessary**, but **more than one target with simple zeros is not necessary**.

For the last distinction, take a nonsingular [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) scaled so that $\wp'^2=4\wp(\wp-1)(\wp+1)$; it has branch values $-1,0,1,\infty$. These are the [four totally ramified Weierstrass values](../../../../../four-totally-ramified-weierstrass-values.md): finite branch preimages have local degree two, and all [poles](../../../../../pole.md) are double. Set

$$
f(z)=\frac1{\wp(z)-2},\qquad
\{a_1,\ldots,a_5\}=\{-\tfrac13,-\tfrac12,-1,0,1\}.
$$

The first four targets are the images of those branch values under the [Möbius transformation](../../../../../mobius-transformation.md). Their preimages remain double; at a lattice [pole](../../../../../pole.md), for example, $f(z)\sim(z-z_*)^2$. The last target corresponds to $\wp=3$, where $\wp'^2=96\ne0$, so every such preimage is simple. The degree-two torus map attains that regular value, and periodicity produces infinitely many preimages in the plane. This nonconstant [elliptic function](../../../../../elliptic-function.md) is transcendental because it has infinitely many [poles](../../../../../pole.md). Exactly one of the five selected finite targets therefore has simple preimages.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 86](../../paper-86-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

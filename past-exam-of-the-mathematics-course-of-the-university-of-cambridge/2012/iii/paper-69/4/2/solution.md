<h1 id="4/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Every convergent member is also [A-stable](../../../../../../a-stability.md). For $0<\alpha<2$, put $\zeta=e^{i\theta}$ and calculate its [boundary-locus test for multistep A-stability](../../../../../../boundary-locus-test-for-multistep-a-stability.md):

$$
\frac{\rho(\zeta)}\zeta=-\alpha(1-\cos\theta)+i(2-\alpha)\sin\theta,
\qquad
\frac{\sigma(\zeta)}\zeta=(2-\alpha)\cos\theta+i\frac\alpha2\sin\theta.
$$

The denominator never vanishes on the unit circle in this parameter interval. It follows that

$$
\operatorname{Re}\frac{\rho(e^{i\theta})}{\sigma(e^{i\theta})}
=\frac{\alpha(2-\alpha)(1-\cos\theta)^2}
{2[(2-\alpha)^2\cos^2\theta+\alpha^2\sin^2\theta/4]}\geq0.
$$

Therefore no amplification root can cross the unit circle as $z=h\lambda$ moves in the open left half-plane. For small negative real $z$, the root near one moves to $1+z+O(z^2)$, inside the circle; the other begins at $\alpha-1$, also strictly inside. The leading coefficient $1-(1-\alpha/4)z$ never vanishes in the left half-plane. Continuity of polynomial roots and connectedness of that half-plane now keep both roots inside everywhere. On its imaginary boundary the same locus has zero real part only at $\zeta=1$, corresponding to $z=0$; that root is simple because $2-\alpha>0$.

At $\alpha=0$, the two interlaced subsequences follow the [trapezoidal rule](../../../../../../trapezoidal-rule.md) with step $2h$:

$$
\zeta^2=\frac{1+z}{1-z}.
$$

The right side has modulus at most one for $\operatorname{Re}z\leq0$. Its unit-circle roots are simple; the double zero at $z=-1$ lies strictly inside and is harmless. Thus the endpoint is also [A-stable](../../../../../../a-stability.md). Combining this with part 1, the requested range is **$0\leq\alpha<2$**, including the [BDF2 method](../../../../../../second-order-backward-differentiation-formula.md) at $\alpha=4/3$.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [4](../../4.md)
3. [Section I](../../section-i.md)
4. [Paper 69](../../../paper-69-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)

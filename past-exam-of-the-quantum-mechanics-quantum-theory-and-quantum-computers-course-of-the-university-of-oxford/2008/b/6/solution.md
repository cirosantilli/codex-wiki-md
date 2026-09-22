<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Choose an [orthonormal](../../../../orthonormal-set.md) [eigenbasis](../../../../eigenbasis.md) $H_0|n\rangle=E_n|n\rangle$ and the [phase](../../../../phase-waves.md) convention $\langle0|\psi'\rangle=0$. Comparing coefficients of the [eigenvalue](../../../../eigenvalue.md) equation at first order yields

$$
(H_0-E_0)\psi'=-(H'-E')|0\rangle.
$$

Projecting onto $|0\rangle$ and the other [eigenvectors](../../../../eigenvector.md) gives

$$
\boxed{E'=\langle0|H'|0\rangle,\qquad\psi'=\sum_{n\ne0}\frac{\langle n|H'|0\rangle}{E_0-E_n}|n\rangle.}
$$

Projection of the next-order equation onto $|0\rangle$ gives

$$
\boxed{E''=\langle0|H'|\psi'\rangle=\sum_{n\ne0}\frac{|\langle n|H'|0\rangle|^2}{E_0-E_n}.}
$$

These are coefficients of the printed series, so $E''$ denotes the quadratic coefficient rather than the second derivative itself. Without a [phase](../../../../phase-waves.md) convention an arbitrary purely imaginary multiple of $\psi_0$ can be added to the first vector correction. Continuous spectrum, if present, requires the corresponding [spectral integral](../../../../spectral-theorem.md); the oscillator has a discrete [complete](../../../../completeness.md) [eigenbasis](../../../../eigenbasis.md).

Put $K=m\omega^2/2$ and let $g(x)=(2\pi\sigma^2)^{-1/2}e^{-x^2/(2\sigma^2)}$ denote the ground-state density. Then $H'=K(a^2-x^2)\mathbf1_{[-a,a]}$ and $p=\int_{-a}^ag(x)\,dx$. Because $g'=-xg/\sigma^2$, [integration by parts](../../../../integration-by-parts.md) yields

$$
I_2:=\int_{-a}^ax^2g\,dx=\sigma^2p-2a\sigma^2g(a),\qquad
I_4:=\int_{-a}^ax^4g\,dx=3\sigma^4p-2a\sigma^2(a^2+3\sigma^2)g(a).
$$

Thus the two first-order shifts are

$$
\boxed{E'_0=K[(a^2-\sigma^2)p+2a\sigma^2g(a)],\qquad
E'_1=K[(a^2-3\sigma^2)p+6a\sigma^2g(a)].}
$$

The first is the supplied ground-state expression; the second follows because the excited-state density is $x^2g/\sigma^2$, so $E'_1=K(a^2I_2-I_4)/\sigma^2$.

Subtracting, and using $K\sigma^2=\hbar\omega/4$, gives

$$
\boxed{E'_1-E'_0=-\frac{\hbar\omega}{2}[p(a)-2ag(a)].}
$$

The bracket is zero at $a=0$, tends to one at infinity, and has derivative $2a^2g(a)/\sigma^2\geq0$. Therefore the first-order predicted level gap is

$$
\boxed{E_1^{\rm app}-E_0^{\rm app}=\hbar\omega\left[1-\frac\lambda2\{p(a)-2ag(a)\}\right].}
$$

For every $\lambda>2$ it becomes negative for all sufficiently large $a$, crossing when $p-2ag=2/\lambda$. It is still positive at $a=0$: the stated conclusion must be read with the large-$a$ regime, rather than for every interval width.

For $\lambda>1$ the inner potential curves downward, placing a central barrier between two symmetric minima at $\pm a$. The [even](../../../../even-function.md) unperturbed [ground state](../../../../ground-state.md) has its greatest density at the central barrier, while the [odd](../../../../odd-function.md) first [excited state](../../../../excited-state.md) has a node there and is less penalized. This explains the relative first-order shifts. **A negative predicted gap signals failure of that perturbation approximation**, not inversion of the exact lowest two states: the true one-dimensional [ground state](../../../../ground-state.md) remains [nodeless](../../../../nodeless-eigenfunction.md) and [even](../../../../even-function.md), with the [odd](../../../../odd-function.md) state above it. At a high barrier the actual low levels instead form a close double-well pair. The [apparent level crossing from a finite-interval oscillator perturbation](../../../../apparent-level-crossing-from-a-finite-interval-oscillator-perturbation.md) is useful precisely as a diagnostic of the approximation's range.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

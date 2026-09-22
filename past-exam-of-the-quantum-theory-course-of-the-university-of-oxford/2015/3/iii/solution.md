<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For brevity write $\gamma=mKZ/\hbar^2$. With the physical [indicial root](../../../../indicial-root.md) $c=\ell+1$, substitute $f=\sum_{n\geq0}a_nr^{n+\ell+1}$ into the equation from part (i). The coefficient of $r^{n+\ell}$ is

$$
\bigl[(n+\ell+2)(n+\ell+1)-\ell(\ell+1)\bigr]a_{n+1}+
\bigl[2\gamma-2\alpha(n+\ell+1)\bigr]a_n=0.
$$

The [indicial equation](../../../../indicial-equation.md) has already canceled the still lower power $r^{\ell-1}$. Rearranging gives the [recurrence relation](../../../../recurrence-relation.md)

$$
\boxed{a_{n+1}=2a_n\frac{\alpha(n+\ell+1)-mKZ/\hbar^2}{(n+\ell+2)(n+\ell+1)-\ell(\ell+1)}.}
$$

Its denominator is $(n+1)(n+2\ell+2)>0$ for every $n\geq0$.

To impose [wavefunction normalization](../../../../wavefunction-normalization.md) at infinity, first suppose that the series never terminates. Then

$$
\frac{a_{n+1}}{a_n}\sim\frac{2\alpha}{n},\qquad n\to\infty.
$$

This is the exponential-series growth associated with $e^{2\alpha r}$, which would overwhelm the factor $e^{-\alpha r}$ in $\psi$. A direct lower-bound argument makes the conclusion precise. All sufficiently late recurrence ratios are real and positive, so after a common [global phase](../../../../global-phase.md) choice the tail coefficients have one sign. For any $0<\eta<\alpha$, there is an index $N$ such that

$$
\frac{|a_{n+1}|}{|a_n|}\geq\frac{2\alpha-\eta}{n+1},\qquad n\geq N.
$$

Induction then bounds the tail below by a positive multiple of

$$
r^{\ell+1}\sum_{n\geq N}\frac{[(2\alpha-\eta)r]^n}{n!}.
$$

The finitely many earlier terms form a [polynomial](../../../../polynomial-split.md) and cannot cancel this exponential growth. Thus $|\psi|=r^{-1}e^{-\alpha r}|f|$ grows at least as a positive multiple of $r^\ell e^{(\alpha-\eta)r}$ for large $r$, contradicting [wavefunction normalization](../../../../wavefunction-normalization.md). This proves that the regular series must terminate.

Since the denominator never vanishes, termination requires the numerator to vanish at some nonnegative integer $n$:

$$
\boxed{\alpha=\frac{mKZ}{(n+\ell+1)\hbar^2}.}
$$

Then $a_{n+1}=0$ and every later coefficient is zero. Consequently **$f$ is a polynomial of degree $n+\ell+1$**, with a factor $r^{\ell+1}$; equivalently,

$$
f(r)=r^{\ell+1}P_n(r),\qquad \psi(r)=r^\ell P_n(r)e^{-\alpha r},
$$

where $P_n$ has degree $n$. This is [series-termination quantization of the Coulomb radial equation](../../../../series-termination-quantization-of-the-coulomb-radial-equation.md). If $N_{\rm p}=n+\ell+1$ denotes the [principal quantum number](../../../../principal-quantum-number.md), the associated [energy eigenvalues](../../../../energy-eigenvalue-split.md) are

$$
\boxed{E_{N_{\rm p}}=-\frac{mK^2Z^2}{2\hbar^2N_{\rm p}^2},\qquad N_{\rm p}=1,2,\ldots.}
$$

Here $n$ counts the degree of the remaining radial polynomial; it is not the principal [quantum number](../../../../quantum-number.md) itself.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the quantum theory course of the University of Oxford](../../../split.md)
5. [Quantum theory course of the University of Oxford](../../../../quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

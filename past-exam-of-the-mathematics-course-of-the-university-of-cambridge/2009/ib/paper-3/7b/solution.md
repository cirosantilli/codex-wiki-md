<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

Hermiticity of the [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) gives $\langle\psi_m,H\psi_n\rangle=\langle H\psi_m,\psi_n\rangle$, so

$$
(E_n-E_m)\langle\psi_m,\psi_n\rangle=0.
$$

The distinct [eigenvalues](../../../../../eigenvalue.md) force [orthogonality](../../../../../orthogonal-vectors.md) for $m\ne n$, and the given normalization gives one for $m=n$. Therefore $\langle\psi_m,\psi_n\rangle=\delta_{mn}$.

Under the time-independent [Schrödinger equation](../../../../../schrodinger-equation.md), each energy component acquires its own phase:

$$
\boxed{\Psi(x,t)=\sum_{n=0}^\infty2^{-(n+1)/2}e^{-iE_nt/\hbar}\psi_n(x).}
$$

The sum converges in the state [Hilbert space](../../../../../hilbert-space-split.md) because the squared coefficients are summable. [Orthogonality](../../../../../orthogonal-vectors.md) makes its squared [norm](../../../../../norm.md) $\sum_{n\geq0}2^{-(n+1)}=1$ at every time.

The [Born rule](../../../../../born-rule.md) for energy measurement gives

$$
\boxed{\mathbb P(E=E_m)=2^{-(m+1)},\qquad
\langle H\rangle=\sum_{n=0}^\infty\frac{E_n}{2^{n+1}}.}
$$

Both depend only on squared coefficient magnitudes, so both are time-independent. The expectation follows either by summing energy times measurement probability or by inserting the orthogonal expansion in the quadratic form of $H$.

Normalization alone does not guarantee a finite mean for an arbitrary spectrum. The displayed energy series is finite when $\sum |E_n|2^{-(n+1)}<\infty$. Since the spectrum is bounded below by $E_0$, a divergent positive tail gives an extended expectation $+\infty$, still independent of time; for example an abstract diagonal Hamiltonian with $E_n=4^n$ has this property. No growth assumption on $E_n$ is printed, so finiteness should not be asserted without this qualification.

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

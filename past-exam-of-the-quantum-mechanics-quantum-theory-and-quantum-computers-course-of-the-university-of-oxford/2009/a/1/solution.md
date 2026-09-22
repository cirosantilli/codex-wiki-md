<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Inside the infinite well, the time-independent [Schrödinger equation](../../../../schrodinger-equation.md) is $-\hbar^2\Psi''/(2m)=E\Psi$ with Dirichlet endpoints. Negative or zero [energy](../../../../energy-split.md) gives no nonzero solution satisfying both endpoints. For $E>0$, the sine solution requires $ka=n\pi$. Thus

$$
\boxed{E_n=\frac{n^2\pi^2\hbar^2}{2ma^2},\qquad\Psi_n(x)=\sqrt{\frac2a}\sin\frac{n\pi x}a,\quad n\geq1.}
$$

The [normalization](../../../../normalization.md) follows from $\int_0^a\sin^2(n\pi x/a)\,dx=a/2$. These functions form an [orthonormal basis](../../../../orthonormal-basis.md). Substitute the expansion into $i\hbar\partial_t\psi=H\psi$ and take the [inner product](../../../../inner-product-split.md) with each basis vector: orthonormality gives $i\hbar\dot c_n=E_nc_n$, equivalently

$$
\boxed{c_n(t)=c_n(0)e^{-iE_nt/\hbar}.}
$$

For a general infinite expansion this is interpreted in the usual [Hamiltonian](../../../../hamiltonian.md) domain or its [unitary](../../../../unitary-connection.md) evolution; the particular state below has only two terms.

Put $\theta=\pi x/a$. The identity $\sin\theta(16\cos^2\theta-1)=4\sin3\theta+3\sin\theta$ gives $c_1=3/5$, $c_3=4/5$, all others zero. Their squared magnitudes sum to one. Hence

$$
\boxed{\langle H\rangle=\frac9{25}E_1+\frac{16}{25}E_3=\frac{153\pi^2\hbar^2}{50ma^2}.}
$$

The evolved state is $(3e^{-iE_1t/\hbar}\Psi_1+4e^{-iE_3t/\hbar}\Psi_3)/5$. Its position [probability](../../../../probability.md) includes an [interference](../../../../interference-wave-propagation.md) term with frequency $\Omega=(E_3-E_1)/\hbar=4\pi^2\hbar/(ma^2)$. Specifically,

$$
P(t)=\frac2{25\pi}\int_0^{\pi/4}\left[9\sin^2\theta+16\sin^23\theta+24\sin\theta\sin3\theta\cos(\Omega t)\right]d\theta.
$$

The three required integrals are $\pi/8-1/4$, $\pi/8+1/12$ and $1/4$, respectively. Therefore

$$
\boxed{P(0\leq X\leq a/4;t)=\frac14-\frac{11}{150\pi}+\frac{12}{25\pi}\cos\left(\frac{4\pi^2\hbar t}{ma^2}\right).}
$$

The [energy](../../../../energy-split.md) [expectation](../../../../expected-value-split.md) is constant while the spatial [probability](../../../../probability.md) oscillates, because relative [energy](../../../../energy-split.md) phases affect [interference](../../../../interference-wave-propagation.md) but not the [energy](../../../../energy-split.md) probabilities.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

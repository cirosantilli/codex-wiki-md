<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take $m,\omega>0$ and use the usual common invariant domain for the [position operator](../../../../position-operator.md), [momentum operator](../../../../momentum-operator.md) and their products. Since $X$ and $P$ are [self-adjoint](../../../../self-adjoint-operator.md),

$$
\boxed{a_+=\frac{P+im\omega X}{\sqrt{2m\omega\hbar}}.}
$$

Expanding the [commutator](../../../../commutator.md) and using $[P,X]=-i\hbar I$ gives

$$
[a_-,a_+]=\frac{im\omega[P,X]-im\omega[X,P]}{2m\omega\hbar}=I.
$$

The two products are

$$
a_+a_-=\frac{P^2+m^2\omega^2X^2-m\omega\hbar}{2m\omega\hbar},\qquad
a_-a_+=\frac{P^2+m^2\omega^2X^2+m\omega\hbar}{2m\omega\hbar}.
$$

Consequently the [quantum harmonic oscillator](../../../../quantum-harmonic-oscillator-split.md) [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) is

$$
\boxed{H=\hbar\omega(a_+a_-+\tfrac12 I)=\hbar\omega(a_-a_+-\tfrac12 I).}
$$

The identity $[AB,C]=A[B,C]+[A,C]B$ now gives

$$
\boxed{[H,a_-]=-\hbar\omega a_-,\qquad[H,a_+]=\hbar\omega a_+.}
$$

Thus $H(a_\pm\psi)=(E\pm\hbar\omega)a_\pm\psi$. **Each ladder image is an [eigenstate](../../../../eigenstate.md) if it is nonzero**; a zero [vector](../../../../vector.md) is not an [eigenstate](../../../../eigenstate.md). The distinction is needed for lowering the [ground state](../../../../ground-state.md). Their squared [norms](../../../../norm.md) are

$$
\boxed{\|a_-\psi\|^2=\left(\frac E{\hbar\omega}-\frac12\right)\|\psi\|^2,\qquad
\|a_+\psi\|^2=\left(\frac E{\hbar\omega}+\frac12\right)\|\psi\|^2.}
$$

These follow by moving the operator to the other side of the [inner product](../../../../inner-product-split.md) with its [adjoint operator](../../../../adjoint-operator.md). The first inequality implies $E\geq\hbar\omega/2$ for every [eigenstate](../../../../eigenstate.md).

For a lowest-energy [quantum state](../../../../quantum-state.md), $a_-\psi_0$ must vanish, since otherwise it would be an [eigenstate](../../../../eigenstate.md) with lower energy. The [norm](../../../../norm.md) formula then forces $E_0=\hbar\omega/2$. Raising never vanishes and produces

$$
\boxed{E_n=\hbar\omega(n+\tfrac12),\qquad\psi_n=(a_+)^n\psi_0,\qquad n=0,1,2,\ldots.}
$$

To see that there are no other [eigenvalues](../../../../eigenvalue.md), repeatedly lower any [eigenstate](../../../../eigenstate.md). If $E/(\hbar\omega)-1/2$ were not a nonnegative integer, there would be a final nonzero lowered [quantum state](../../../../quantum-state.md) with energy strictly between $\hbar\omega/2$ and $3\hbar\omega/2$. Its lower image would have positive [norm](../../../../norm.md) but energy below the lower bound, a contradiction. Thus every [eigenstate](../../../../eigenstate.md) reaches the ground eigenspace after an integer number of lowerings. On a positive level, lowering is injective by its strictly positive [norm](../../../../norm.md) factor. The assumed one-dimensional ground eigenspace therefore makes every eigenspace one-dimensional, so the displayed raised [quantum states](../../../../quantum-state.md) give all [eigenstates](../../../../eigenstate.md) up to nonzero multiples. If $\psi_0$ is normalized, their [norms](../../../../norm.md) are $\|\psi_n\|^2=n!$.

For $k\geq1$, $(a_+)^k\psi$ has [eigenvalue](../../../../eigenvalue.md) $E+k\hbar\omega$, distinct from $E$. [eigenstates](../../../../eigenstate.md) of a [self-adjoint operator](../../../../self-adjoint-operator.md) with distinct [eigenvalues](../../../../eigenvalue.md) are [orthogonal](../../../../orthogonal-vectors.md): applying self-adjointness to their [inner product](../../../../inner-product-split.md) gives $(E'-E)\langle\psi,\phi\rangle=0$. Therefore

$$
\boxed{\langle\psi,(a_+)^k\psi\rangle=0.}
$$

The [expectation](../../../../expected-value-split.md) of $(a_-)^k$ also vanishes, either by lowering and [orthogonality](../../../../orthogonal-vectors.md) or by conjugating the adjoint relation.

Solving the ladder definitions for $X$ and $P$ gives

$$
T=\frac{\hbar\omega}{4}(a_-+a_+)^2,\qquad V=-\frac{\hbar\omega}{4}(a_+-a_-)^2,
$$

so $T-V=\frac12\hbar\omega((a_+)^2+(a_-)^2)$. Both terms have zero [expectation](../../../../expected-value-split.md) by the preceding [orthogonality](../../../../orthogonal-vectors.md). Since $T+V=H$, the oscillator form of the [quantum virial theorem](../../../../quantum-virial-theorem.md) is

$$
\boxed{\mathbb E_\psi(T)=\mathbb E_\psi(V)=E/2.}
$$

Expectations here are divided by $\|\psi\|^2$ if the [eigenstate](../../../../eigenstate.md) is not normalized; no [normalization](../../../../normalization.md) assumption was used in the ladder argument.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the quantum mechanics and electromagnetism course of the University of Oxford](../../../split.md)
5. [Quantum mechanics and electromagnetism course of the University of Oxford](../../../../quantum-mechanics-and-electromagnetism-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

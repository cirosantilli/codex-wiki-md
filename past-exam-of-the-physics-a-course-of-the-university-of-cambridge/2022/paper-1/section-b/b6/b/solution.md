<h1 id="section-b/b6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For either [number operator](../../../../../../number-operator.md) $\hat N=\hat a^\dagger\hat a$, positivity follows from

$$
\langle u|\hat N|u\rangle=\|\hat a|u\rangle\|^2\ge0.
$$

Hence an [eigenvalue](../../../../../../eigenvalue.md) $\nu$ cannot be negative. The [commutators](../../../../../../commutator.md)

$$
[\hat N,\hat a]=-\hat a,\qquad [\hat N,\hat a^\dagger]=\hat a^\dagger
$$

show that $\hat a|\nu\rangle$, if nonzero, is an [eigenstate](../../../../../../eigenstate.md) with [eigenvalue](../../../../../../eigenvalue.md) $\nu-1$. For a normalized [eigenstate](../../../../../../eigenstate.md), $\|\hat a|\nu\rangle\|^2=\nu$.

If $\nu$ were not an integer, successive nonzero lowerings would eventually reach an [eigenstate](../../../../../../eigenstate.md) with $0<\nu'<1$. Its next lowering would have nonzero [norm](../../../../../../norm.md) but a negative [eigenvalue](../../../../../../eigenvalue.md), contradicting positivity. The ladder must therefore terminate at $\nu=0$, with $\hat a|0\rangle=0$. Conversely, successive applications of the [creation operator](../../../../../../creation-operator.md) never vanish, because

$$
\|\hat a^\dagger|n\rangle\|^2=\langle n|(\hat N+1)|n\rangle=n+1>0.
$$

The normalizable bottom state exists explicitly: solving $\hat a\psi_0=0$ gives $\psi_0(x)\propto\exp[-m\omega x^2/(2\hbar)]$. Thus the [number operator](../../../../../../number-operator.md) has exactly the non-negative integer [eigenvalues](../../../../../../eigenvalue.md).

Since the two coordinate [number operators](../../../../../../number-operator.md) commute, use the product [eigenstates](../../../../../../eigenstate.md) $|n_x,n_y\rangle$. Their [energy eigenvalues](../../../../../../energy-eigenvalue-split.md) are

$$
\boxed{E_{n_x,n_y}=\hbar\omega(n_x+n_y+1),\qquad n_x,n_y=0,1,2,\ldots.}
$$

At fixed $N=n_x+n_y$, the allowed pairs are $(0,N),(1,N-1),\ldots,(N,0)$. Thus the [energy level](../../../../../../energy-level.md) $E_N=(N+1)\hbar\omega$ has [quantum degeneracy](../../../../../../degenerate-energy-levels.md) $N+1$, and the [ground-state energy](../../../../../../ground-state-energy.md) is $\hbar\omega$.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)

<h1 id="15b/solution">Solution</h1>

↑ **Parent:** [15B](../15b.md)

Using the [momentum operator](../../../../../momentum-operator.md) $\hat p=-i\hbar\,d/dx$ and its commutator with multiplication by $A$, expansion of the [factorized quantum Hamiltonian](../../../../../factorized-quantum-hamiltonian.md) gives

$$
\hat H=\frac1{2m}[\hat p^2+s^2A^2-s\hbar A'],\qquad
\boxed{V(x)=\frac{s^2A(x)^2-s\hbar A'(x)}{2m}.}
$$

The first-order zero-mode equation integrates to

$$
\boxed{\chi(x)=C\exp\left[-\frac s\hbar\int^x A(t)\,dt\right].}
$$

For $A=x^n$, its exponent is $-s x^{n+1}/[\hbar(n+1)]$. It decays at both ends exactly when $n+1$ is even. If $n$ is even it grows at negative infinity. Thus **a nonzero square-integrable zero mode exists exactly for odd $n$**.

For $n=1$ the Gaussian zero mode is $\chi=(s/(\pi\hbar))^{1/4}e^{-s x^2/(2\hbar)}$. More generally, on normalized states with finite second moments and the usual integration-by-parts boundary conditions, $\hat H=Q^\dagger Q/(2m)$ is nonnegative. With zero means this implies, for every $s>0$,

$$
0\le (\Delta p)^2+s^2(\Delta x)^2-s\hbar.
$$

Minimizing the quadratic in $s$ at $s=\hbar/[2(\Delta x)^2]$ yields

$$
\boxed{\Delta x\Delta p\ge\hbar/2.}
$$

The Gaussian mode attains equality. The argument concerns the same state for the whole positive family of factorized operators, which permits the minimization.

## ↑ Ancestors (10)

1. [15B](../15b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

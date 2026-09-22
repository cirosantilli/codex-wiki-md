<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Complex conjugation reverses the order of the Grassmann variables. Thus the conjugate of $i\bar\psi\dot\psi$ differs from itself only by integration by parts, while the remaining terms are manifestly real. The action is therefore real up to a boundary term.

Substituting the stated transformations into the Lagrangian, using anticommutation of $\psi,\bar\psi,\epsilon,\bar\epsilon$, and integrating the terms containing $\ddot x$ and $\dot\psi$ by parts leaves a total derivative. A convenient convention for the resulting [Noether charges](../../../../../noether-charge.md) is

$$
\boxed{Q=\psi\left(p-ih'(x)\right),
\qquad
\bar Q=\bar\psi\left(p+ih'(x)\right)},
\qquad p=\dot x.
$$

Overall signs can be moved between the charges and the Grassmann transformation parameters. These charges generate the displayed transformations and obey the classical supersymmetry algebra.

Canonical quantization gives

$$
[x,p]=i,
\qquad
\{\psi,\bar\psi\}=1,
\qquad
\psi^2=\bar\psi^2=0,
$$

with all other elementary graded commutators zero. Represent $p=-i\,d/dx$, let $\psi$ act by exterior multiplication by $dx$, and let $\bar\psi$ act by contraction with $\partial_x$. The Hilbert space is then

$$
\mathcal H=L^2\Omega^0(\mathbb R)\oplus L^2\Omega^1(\mathbb R),
$$

the square-integrable complex differential forms on the line. Up to an inessential factor of $-i$, $Q$ is the [twisted de Rham differential](../../../../../twisted-de-rham-differential.md)

$$
d_h=e^{-h}de^h=d+dh\wedge,
$$

and $\bar Q$ is its Hilbert-space adjoint. The Hamiltonian is $H=\{Q,\bar Q\}/2$, so a zero-energy state must be annihilated by both charges.

On zero-forms the zero-mode equation is $(d/dx+h')u=0$, giving $u=Ce^{-h}$. On one-forms it is $(-d/dx+h')v=0$, giving $v=Ce^h$. For $h=-x^4$, only the one-form is square integrable, so the unique ground state is

$$
\boxed{\Psi_0=C e^{-x^4}dx}.
$$

For a generic cubic polynomial, $h(x)$ tends to opposite infinities at the two ends of the real line. Each of $e^h$ and $e^{-h}$ therefore diverges at one end, so neither candidate is square integrable. There is consequently no normalizable zero-energy state.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 307](../../paper-307-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

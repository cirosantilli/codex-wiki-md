<h1 id="b/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [permutation](../../../../permutation.md) $\pi$ of [identical particles](../../../../indistinguishable-particles.md) multiplies a fermionic state by $\operatorname{sgn}(\pi)$; a bosonic state is invariant. Particle exchange keeps $y_+$ fixed and sends $y_-$ to $-y_-$. Consequently the spatial [wave function](../../../../wave-function-split.md) is even in $y_-$ for the stated bosonic model and odd for the stated fermionic model. This assumes no additional spin variables in the supplied model; exchange of full particle states is the underlying rule.

The coordinate change is orthogonal, with unit [Jacobian determinant](../../../../jacobian-determinant.md), so the [kinetic energy](../../../../kinetic-energy.md) becomes

$$
H=-\frac{\hbar^2}{2m}(\partial_{y_+}^2+\partial_{y_-}^2)
$$

on the square $|y_+|,|y_-|<a$ with zero boundary values. Product states $\psi_r(y_+)\psi_s(y_-)$ have energy

$$
E_{r,s}=K(r^2+s^2),\qquad K=\frac{\pi^2\hbar^2}{8ma^2}.
$$

The one-dimensional [eigenfunction](../../../../eigenfunction.md) is even for odd $s$ and odd for even $s$. [Bosons](../../../../boson.md) therefore allow odd $s$, whereas [fermions](../../../../fermion.md) require even $s$. The lowest bosonic pair is $(r,s)=(1,1)$; its first excited pair is $(2,1)$. The lowest fermionic pair is $(1,2)$. Thus

$$
\boxed{E_{B,0}=2K=\frac{\pi^2\hbar^2}{4ma^2},\qquad
E_{B,1}=E_{F,0}=5K=\frac{5\pi^2\hbar^2}{8ma^2}.}
$$

The printed bosonic ground-energy claim omits the factor $\pi^2/4$; the value above follows directly from the supplied one-dimensional spectrum and [kinetic energy](../../../../kinetic-energy.md).

The separation is $|x_1-x_2|=\sqrt2|y_-|$. The normalized $y_+$ factor integrates out. In the fermionic [ground state](../../../../ground-state.md), the relative-coordinate density is $a^{-1}\sin^2(\pi y_-/a)$, giving

$$
\langle|y_-|\rangle_F=\frac2a\int_0^a y\sin^2(\pi y/a)\,dy=\frac a2.
$$

For the bosonic [ground state](../../../../ground-state.md) it is $a^{-1}\cos^2(\pi y_-/(2a))$, giving

$$
\langle|y_-|\rangle_B=\frac2a\int_0^a y\cos^2(\pi y/(2a))\,dy
=a\left(\frac12-\frac2{\pi^2}\right).
$$

Both [integrals](../../../../integral-split.md) follow by replacing squared trigonometric functions by their constant and cosine parts and integrating once by parts. Hence

$$
\boxed{\langle|x_1-x_2|\rangle_F=\frac a{\sqrt2},\quad
\langle|x_1-x_2|\rangle_B=\sqrt2a\left(\frac12-\frac2{\pi^2}\right),}
$$

and the difference is $\boxed{2\sqrt2a/\pi^2}$. The odd relative state vanishes at coincidence, which increases its expected separation.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

<h1 id="15c/solution">Solution</h1>

↑ **Parent:** [15C](../15c.md)

Differentiate under the [integral](../../../../../integral.md) and use $\nabla_x|x-x'|^{-1}=-\nabla_{x'}|x-x'|^{-1}$:

$$
\begin{aligned}
\nabla\cdot A
&=-\frac{\mu_0}{4\pi}\int J_i(x')
\partial_i'\frac1{|x-x'|}\,d^3x'\\
&=\frac{\mu_0}{4\pi}\int
\frac{\nabla'\cdot J(x')}{|x-x'|}\,d^3x'.
\end{aligned}
$$

The omitted boundary term vanishes if the current is localized sufficiently rapidly. A steady current obeys charge conservation $\nabla'\cdot J=0$, hence

$$
\boxed{\nabla\cdot A=0}.
$$

For $r=|x|$ much larger than the source size,

$$
\frac1{|x-x'|}=\frac1r+\frac{x\cdot x'}{r^3}+O(r^{-3}|x'|^2).
$$

Localization and $\nabla'\cdot J=0$ imply $\int J\,d^3x'=0$. They also imply

$$
\int(x_i'J_j+x_j'J_i)\,d^3x'=0,
$$

by integrating $\partial_k'(x_i'x_j'J_k)$. Thus the first nonzero moment is antisymmetric and can be written using the [magnetic dipole moment](../../../../../magnetic-dipole-moment.md)

$$
\boxed{m=\frac12\int x'\times J(x')\,d^3x'}.
$$

Consequently the [Coulomb-gauge vector potential of a localized steady current](../../../../../coulomb-gauge-vector-potential-of-a-localized-steady-current.md) has far field

$$
\boxed{A(x)=\frac{\mu_0}{4\pi}\frac{m\times x}{r^3}+\cdots}.
$$

The dimensions are

$$
\boxed{[J]=\mathrm{A\,m^{-2}}},
\qquad
\boxed{[m]=\mathrm{A\,m^2}}.
$$

## ↑ Ancestors (10)

1. [15C](../15c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

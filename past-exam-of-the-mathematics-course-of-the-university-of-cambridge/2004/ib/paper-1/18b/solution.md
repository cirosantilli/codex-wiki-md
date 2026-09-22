<h1 id="18b/solution">Solution</h1>

↑ **Parent:** [18B](../18b.md)

Using $E=-\nabla\phi$ and the electrostatic [Poisson equation](../../../../../poisson-equation.md), $\rho=-\epsilon_0\nabla^2\phi$, [integration by parts](../../../../../integration-by-parts.md) gives

$$
W=-\frac{\epsilon_0}{2}\int_D\phi\nabla^2\phi\,dV
=\frac{\epsilon_0}{2}\int_D|\nabla\phi|^2dV
-\frac{\epsilon_0}{2}\int_{\partial D}\phi\,\partial_n\phi\,dS.
$$

The boundary potential is zero, so the surface term vanishes. Hence **$\boxed{W=(\epsilon_0/2)\int_DE^2dV}$**.

For the [capacitor](../../../../../capacitor.md) use the usual parallel-plate approximation, neglecting edge fields. The two gaps have widths $H+a$ and $H-a$, and their field magnitudes are $V/(H+a)$ and $V/(H-a)$. The field-[energy](../../../../../energy.md) expression gives

$$
\boxed{W=\frac{\epsilon_0AV^2}{2}\left(\frac1{H+a}+\frac1{H-a}\right)
=\frac{\epsilon_0AV^2H}{H^2-a^2}.}
$$

The two faces of the middle plate carry charges $Q_-=\epsilon_0AV/(H+a)$ and $Q_+=\epsilon_0AV/(H-a)$. Its total charge is their sum; the grounded plates have zero potential and contribute zero to $\frac12\sum Q_j\phi_j$. The charge-potential expression therefore gives $W=\frac12V(Q_-+Q_+)$, exactly the same result. Since $H^2-a^2$ is largest at $a=0$, **the [energy](../../../../../energy.md) at fixed $V$ is minimized when the middle plate is centered**, with value $\epsilon_0AV^2/H$.

This is the [electrostatic energy of a three-plate capacitor](../../../../../electrostatic-energy-of-a-three-plate-capacitor.md) in the intended uniform-field model. Finite circular plates have fringing corrections; no small-gap-to-radius ratio is explicitly stated in the source, so the simple formula should not be described as an exact finite-disc solution.

## ↑ Ancestors (10)

1. [18B](../18b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

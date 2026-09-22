<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $L=\log\psi$, with $\psi>0$. Under the [Cole-Hopf transformation](../../../../../../cole-hopf-transformation.md) $q=2\epsilon L_\theta$, direct differentiation gives

$$
q_Z-qq_\theta-\epsilon q_{\theta\theta}=2\epsilon\partial_\theta\{L_Z-\epsilon(L_{\theta\theta}+L_\theta^2)\}.
$$

Since $L_{\theta\theta}+L_\theta^2=\psi_{\theta\theta}/\psi$, [Burgers' equation](../../../../../../burgers-equation.md) is equivalent to

$$
\partial_\theta\left(\frac{\psi_Z-\epsilon\psi_{\theta\theta}}\psi\right)=0.
$$

The ratio is therefore a function $a(Z)$ alone. Multiplying $\psi$ by $\exp[-\int a(Z)\,dZ]$ leaves $q$ unchanged and removes this scalar freedom. Thus one may choose the normalization for which

$$
\boxed{\psi_Z=\epsilon\psi_{\theta\theta}.}
$$

This is the [heat equation](../../../../../../heat-equation.md). The positive sign in $q=2\epsilon\partial_\theta\log\psi$ corresponds to the negative conservative flux $-q^2/2$ used here; the more usual positive-flux convention has the opposite sign.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

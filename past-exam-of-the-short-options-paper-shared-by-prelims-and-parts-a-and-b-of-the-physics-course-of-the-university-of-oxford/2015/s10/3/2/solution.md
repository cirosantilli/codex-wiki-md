<h1 id="s10/3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $x=\Delta E/(k_{\rm B}T)$ and $r=N_\uparrow/N_\downarrow=e^{-x}$. Since $N=N_\uparrow+N_\downarrow$, eliminate the individual populations:

$$
\frac{N_\uparrow-N_\downarrow}{N}=\frac{r-1}{r+1}=\frac{e^{-x}-1}{e^{-x}+1}=-\tanh\frac x2.
$$

The [Taylor expansion](../../../../../taylor-expansion.md) $e^{-x}=1-x+O(x^2)$ gives the same result, and the odd expansion of the [hyperbolic tangent](../../../../../hyperbolic-tangent.md) yields

$$
\boxed{\frac{N_\uparrow-N_\downarrow}{N}=-\frac x2+O(x^3)\simeq-\frac{\hbar\gamma B}{2k_{\rm B}T}.}
$$

Equivalently, $N_\uparrow\simeq(N/2)(1-x/2)$ and $N_\downarrow\simeq(N/2)(1+x/2)$. Their sum is still $N$. The negative sign follows directly from the stated higher-energy up-state population, and does not mean a negative magnitude of the equilibrium magnetization.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [3](../../3.md)
3. [S10](../../../s10.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

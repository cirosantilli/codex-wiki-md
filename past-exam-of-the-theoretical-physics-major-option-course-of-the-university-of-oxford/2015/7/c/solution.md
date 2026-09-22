<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $m=0$, the frequencies are $\omega_n=n\pi/L$. The stipulated spectral regulator therefore supplies $e^{-n/(L\Lambda)}$. With $\epsilon=1/(L\Lambda)$,

$$
E_0^{\rm BC}(L,\Lambda)=\frac\pi{2L}\sum_{n=1}^\infty ne^{-\epsilon n}
=\boxed{\frac\pi{2L}\frac{e^\epsilon}{(e^\epsilon-1)^2}.}
$$

The sum identity follows by differentiating the convergent geometric series $\sum_{n\geq1}z^n=z/(1-z)$ with $z=e^{-\epsilon}$. Its small-$\epsilon$ expansion is

$$
\frac{e^\epsilon}{(e^\epsilon-1)^2}
=\frac1{\epsilon^2}-\frac1{12}+\frac{\epsilon^2}{240}+O(\epsilon^4),
$$

so

$$
\boxed{E_0^{\rm BC}(L,\Lambda)
=\frac{\pi L\Lambda^2}{2}-\frac\pi{24L}
+O\!\left(\frac1{L^3\Lambda^2}\right).}
$$

In the [frequency-regulated Dirichlet Casimir energy](../../../../frequency-regulated-dirichlet-casimir-energy.md), the inverse-length scale $\Lambda$ suppresses modes with frequency much above $\pi\Lambda$ in units $c=1$. It is an ultraviolet cutoff, removed after comparing the same underlying vacuum convention in the two geometries. Physically an ideal perfectly reflecting boundary also ceases to be adequate at sufficiently high frequency, but that material scale is not specified here. The source calls this heat-kernel regularization; its explicit regulator is exponential in frequency, rather than the alternative exponential in frequency squared.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

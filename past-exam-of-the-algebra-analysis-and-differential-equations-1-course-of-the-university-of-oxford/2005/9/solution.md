<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Integrating $e^{-pt}\sin(ct)$, or taking the imaginary part of $\int_0^\infty e^{-(p-ic)t}\,dt$, gives

$$
\boxed{\mathcal L\{\sin ct\}(p)=\frac{c}{p^2+c^2}\qquad(\operatorname{Re}p>0).}
$$

The [Laplace transform convolution theorem](../../../convolution-theorem-for-laplace-transforms.md) states $\mathcal L(f*g)=\bar f\,\bar g$ whenever the transforms and convolution are defined. Applying it to the [Volterra integral equation](../../../volterra-integral-equation.md) gives $\bar x+\bar x/(p^2+1)=\bar F$, so

$$
\boxed{\bar x(p)=\frac{p^2+1}{p^2+2}\bar F(p)=\left(1-\frac1{p^2+2}\right)\bar F(p).}
$$

Since $\mathcal L^{-1}[(p^2+2)^{-1}]=\sin(\sqrt2t)/\sqrt2$, a second application of the convolution theorem yields the [sine-kernel Volterra resolvent](../../../sine-kernel-volterra-resolvent.md)

$$
\boxed{x(t)=F(t)-\frac1{\sqrt2}\int_0^t\sin(\sqrt2(t-s))F(s)\,ds.}
$$

The transform argument assumes suitable growth for the transforms to exist. The resulting causal resolvent formula also applies to locally integrable forcing on finite intervals, as can be checked by substitution and exchanging integrals over a finite triangle.

## ↑ Ancestors (11)

1. [9](../9.md)
2. [2005](../../2005-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)

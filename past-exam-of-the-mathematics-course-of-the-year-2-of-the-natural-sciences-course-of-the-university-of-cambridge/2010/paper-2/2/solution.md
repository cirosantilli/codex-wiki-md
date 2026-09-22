<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use [separation of variables](../../../../separation-of-variables.md), $\Phi=F(r)H(\theta)$, in the [Laplace equation in polar coordinates](../../../../laplace-equation-in-polar-coordinates.md). Dividing by $FH/r^2$ gives

$$
\frac{r(rF')'}F=-\frac{H''}H=n^2.
$$

Single-valued $2\pi$-periodic angular factors have [integer](../../../../integer-split.md) $n\geq0$. For $n\geq1$, they are $\cos n\theta,\sin n\theta$, and the radial equation $r^2F''+rF'-n^2F=0$ has solutions $r^n,r^{-n}$. The zero angular mode gives $F=a_0+b_0\log r$. These separated products give the requested solutions; arbitrary sums may use independent coefficients for each radial-angular combination.

Boundedness at the origin removes the logarithm and all negative radial powers. The boundary function is even, so its sine [Fourier coefficients](../../../../fourier-coefficient.md) vanish. With the convention $f(\theta)=a_0+\sum_{n\geq1}a_n\cos n\theta$, its [Fourier coefficients](../../../../fourier-coefficient.md) are

$$
a_0=\frac1{2\pi}\int_{-\pi}^{\pi}f(\theta)d\theta=\frac C2,\qquad
a_n=\frac1\pi\int_{-\pi}^{\pi}f(\theta)\cos n\theta\,d\theta=\frac{2C}{\pi n}\sin\frac{n\pi}{2}.
$$

Thus the bounded interior [harmonic extension](../../../../harmonic-extension.md) is

$$
\boxed{\Phi_{\rm in}(r,\theta)=\frac C2+\frac{2C}{\pi}\sum_{m=0}^\infty\frac{(-1)^m}{2m+1}\left(\frac rR\right)^{2m+1}\cos((2m+1)\theta).}
$$

For $r<R$ the series and its derivatives converge locally uniformly, so it is [harmonic](../../../../harmonic-function.md). It is a rotated and scaled instance of the [harmonic measure of a semicircle in a disk](../../../../harmonic-measure-of-a-semicircle-in-a-disk.md). For example, summing the [power series](../../../../power-series.md) for the complex arctangent, or differentiating the following expression, gives the equivalent real form

$$
\Phi_{\rm in}=\frac C2+\frac C\pi\arctan\left(\frac{2(r/R)\cos\theta}{1-(r/R)^2}\right),\qquad r<R.
$$

This also proves boundedness directly.

**At the two jumps, the boundary interpretation matters.** At every continuity point the radial limit equals the prescribed value. At $\theta=\pm\pi/2$, the radial limit is $C/2$, the midpoint of the two one-sided values. Consequently for $C\ne0$ there is no harmonic solution continuous on the closed disk with exactly the printed boundary values. The standard bounded [Dirichlet problem](../../../../dirichlet-problem.md) imposes the trace away from the jumps, or almost everywhere; assigning zero separately at those two boundary points does not alter the interior solution.

For uniqueness let $w=\widetilde\Phi-\Phi$. Formally the [divergence theorem](../../../../divergence-theorem.md) applied to $w\nabla w$ gives

$$
0=\int_Dw\Delta w\,dA=\int_{\partial D}w\partial_nw\,ds-\int_D|\nabla w|^2dA.
$$

For continuous zero boundary data, this immediately forces $w=0$. With the actual discontinuous data, one should justify the two exceptional points rather than assume finite [Dirichlet energy](../../../../dirichlet-energy.md) there. Let $|w|\leq M$ and choose a cutoff $\eta_\epsilon$ which is zero within $\epsilon^2$ of those points, one beyond $\epsilon$, and linear in logarithmic distance between. Its gradient satisfies $\int|\nabla\eta_\epsilon|^2=O(1/|\log\epsilon|)$. Applying the [divergence theorem](../../../../divergence-theorem.md) to $\eta_\epsilon^2w\nabla w$ gives

$$
\int_D\eta_\epsilon^2|\nabla w|^2dA=-2\int_D\eta_\epsilon w\nabla\eta_\epsilon\cdot\nabla w\,dA
\leq\frac12\int_D\eta_\epsilon^2|\nabla w|^2dA+2M^2\int_D|\nabla\eta_\epsilon|^2dA.
$$

The resulting energy tends to zero. Hence $\nabla w=0$ on every compact subset and $w$ is constant; its zero boundary trace on the open arcs makes it zero. This is the [logarithmic cutoff proof of harmonic uniqueness with finitely many boundary exceptions](../../../../logarithmic-cutoff-proof-of-harmonic-uniqueness-with-finitely-many-boundary-exceptions.md).

For the [exterior harmonic extension of disk boundary data](../../../../exterior-harmonic-extension-of-disk-boundary-data.md), boundedness instead excludes $r^n$ and the logarithm. The same boundary coefficients give

$$
\boxed{\Phi_{\rm out}(r,\theta)=\frac C2+\frac{2C}{\pi}\sum_{m=0}^\infty\frac{(-1)^m}{2m+1}\left(\frac Rr\right)^{2m+1}\cos((2m+1)\theta),\qquad r>R.}
$$

This is $\Phi_{\rm in}(R^2/r,\theta)$, using [inversion in a circle](../../../../inversion-in-a-circle.md). Its limit at infinity is **$C/2$**. To see why that value is forced independently of this construction, average any bounded exterior [harmonic function](../../../../harmonic-function.md) over a circle. The mean satisfies $(r\overline\Phi')'=0$, hence is $A+B\log r$. Boundedness forces $B=0$, and the boundary mean fixes $A=C/2$. A constant limit at infinity must therefore be $C/2$.

Finally suppose two bounded exterior solutions have this limit. Their difference $w$ tends to zero. Under planar [inversion in a circle](../../../../inversion-in-a-circle.md), it is bounded and [harmonic](../../../../harmonic-function.md) near the origin, so the isolated point there is removable. Its local expansion gives $w=O(r^{-1})$, $\partial_rw=O(r^{-2})$ in the original exterior. Apply the preceding [divergence theorem](../../../../divergence-theorem.md) energy argument on $R<r<L$, with logarithmic cutoffs at the two boundary jumps. After removing those cutoffs, the inner boundary term vanishes; the outer one is $\int_{r=L}w\partial_rw\,ds=O(L^{-2})$. Letting $L\to\infty$ forces $\nabla w=0$, and the zero limit gives $w=0$. Thus the bounded exterior solution is unique as well.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [2010](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

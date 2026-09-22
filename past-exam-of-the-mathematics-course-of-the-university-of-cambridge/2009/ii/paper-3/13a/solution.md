<h1 id="13a/solution">Solution</h1>

↑ **Parent:** [13A](../13a.md)

The species $u$ is the [activator](../../../../../activator-in-a-reaction-diffusion-system.md), since increasing $u$ increases its own production $u^2/v$; $v$ is the [inhibitor](../../../../../inhibitor-in-a-reaction-diffusion-system.md), since increasing $v$ reduces that production. The unique positive uniform [steady state](../../../../../steady-state.md) solves $v=u^2$ and $u^2/v=bu$, giving $\boxed{u_*=1/b,\ v_*=1/b^2}$.

The reaction [Jacobian matrix](../../../../../jacobian-matrix.md) at this state is

$$
J=\begin{pmatrix}b&-b^2\\2/b&-1\end{pmatrix},\qquad \operatorname{tr}J=b-1,\qquad\det J=b.
$$

Its [eigenvalues](../../../../../eigenvalue.md) solve $\lambda^2+(1-b)\lambda+b=0$. Since $b>0$, both have negative real part precisely for $0<b<1$. This proves stability of the spatially uniform reaction kinetics.

A perturbation proportional to $e^{\lambda t+ikx}$ replaces $J$ by $J-k^2\operatorname{diag}(1,d)$. Put $q=k^2$. Its trace is $b-1-(1+d)q<0$ in the kinetically stable range, and its determinant is

$$
D(q)=dq^2+(1-bd)q+b.
$$

A growing spatial mode exists exactly when this determinant is negative for some $q>0$. Its minimum occurs at $q=(bd-1)/(2d)$, which is positive only if $bd>1$, and the minimum is negative precisely if $(bd-1)^2>4bd$. Together these conditions reduce to the [Turing threshold of the quadratic activator-inhibitor model](../../../../../turing-threshold-of-the-quadratic-activator-inhibitor-model.md),

$$
\boxed{0<b<1,\qquad bd>3+2\sqrt2.}
$$

The unstable band is

$$
\frac{bd-1-\sqrt{(bd-1)^2-4bd}}{2d}<k^2<\frac{bd-1+\sqrt{(bd-1)^2-4bd}}{2d}.
$$

At the [Turing instability](../../../../../turing-instability.md) threshold the band shrinks to its double root, yielding $\boxed{k_c^2=(1+\sqrt2)/d}$. On a bounded spatial interval, an allowed [wavenumber](../../../../../wavenumber.md) must additionally lie in the unstable band; the displayed parameter condition assumes the continuous spatial spectrum.

<a id="13a/image-diffusion-driven-instability-above-the-threshold-curve-for-b-between-zero-and-one"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3-turing-region.png)

**[Figure 2](#13a/image-diffusion-driven-instability-above-the-threshold-curve-for-b-between-zero-and-one). Diffusion-driven instability above the threshold curve for b between zero and one**.

## ↑ Ancestors (10)

1. [13A](../13a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

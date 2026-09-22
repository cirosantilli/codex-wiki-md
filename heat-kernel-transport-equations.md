# Heat-kernel transport equations

↑ **Parent:** [Heat parametrix](heat-parametrix.md)

In [normal coordinates](normal-coordinates.md) $q=\exp_p x$, write the [Riemannian volume form](riemannian-volume-form.md) as $J(p,x)\,dx$ and let $r=|x|$. With the [heat operator](heat-operator.md) $\partial_t-\Delta_q$, the Gaussian times a power-series amplitude has its singular terms cancelled by the displayed radial equations for $i\geq1$. The initial coefficient is $w_0=J^{-1/2}$, and

$$
w_i(p,\exp_p x)=J(p,x)^{-1/2}\int_0^1s^{i-1}J(p,sx)^{1/2}(\Delta_qw_{i-1})(p,\exp_p(sx))\,ds.
$$

Multiplying the equation by $r^{i-1}J^{1/2}$ gives the derivative of $r^iJ^{1/2}w_i$. Smoothness forces the integration constant to vanish. The integral on a fixed compact interval proves smoothness across the diagonal by induction; it yields $w_i(p,p)=\Delta_qw_{i-1}(p,p)/i$. A truncated [heat parametrix](heat-parametrix.md) therefore has residual $-g t^k\Delta_qw_k$.

## ↑ Ancestors (10)

1. [Heat parametrix](heat-parametrix.md)
2. [Riemannian heat kernel](riemannian-heat-kernel.md)
3. [Heat kernel](heat-kernel.md)
4. [Heat equation](heat-equation.md)
5. [Diffusion equation](diffusion-equation-split.md)
6. [Partial differential equation](partial-differential-equation-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Curvature coefficient of the scalar heat kernel](curvature-coefficient-of-the-scalar-heat-kernel.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-18/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-19/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-55/3/solution.md)

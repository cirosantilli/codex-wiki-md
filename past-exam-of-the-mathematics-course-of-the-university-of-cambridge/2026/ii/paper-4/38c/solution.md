<h1 id="38c/solution">Solution</h1>

↑ **Parent:** [38C](../38c.md)

Curling Navier-Stokes and using incompressibility gives $\omega_t+(u\cdot\nabla)\omega=(\omega\cdot\nabla)u+\nu\nabla^2\omega$. For pure swirl, $\omega=r^{-1}(rv)_r$, so regularity gives $v(r,t)=r^{-1}\int_0^rs\omega(s,t)ds$. Adding strain $(-\alpha r,v,2\alpha z)$ yields

$$
\omega_t-\alpha r\omega_r=2\alpha\omega+\nu(\omega_{rr}+r^{-1}\omega_r).
$$

Multiplication by $2\pi r$ and integration proves $\dot\Gamma=0$. The decaying steady [Burgers vortex](../../../../../burgers-vortex.md) is

$$
\boxed{\omega_s(r)=\frac{\Gamma\alpha}{2\pi\nu}e^{-\alpha r^2/(2\nu)}.}
$$

## ↑ Ancestors (10)

1. [38C](../38c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

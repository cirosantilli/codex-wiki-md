<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Retain terms quadratic in the small displacements and velocities. The approximations $1-\cos\theta\simeq\theta^2/2$ and $\cos(\theta_1-\theta_2)\simeq1$ yield

$$
U\simeq\frac{mgl}{2}(4\theta_1^2+\theta_2^2),\qquad K\simeq\frac{ml^2}{2}(8\dot\theta_1^2+4\dot\theta_1\dot\theta_2+\dot\theta_2^2).
$$

Thus the correct [quadratic forms](../../../../quadratic-form-split.md) are

$$
\boxed{U=\frac12\boldsymbol\theta^{\mathsf T}\mathbf V\boldsymbol\theta,\quad K=\frac12\dot{\boldsymbol\theta}^{\mathsf T}\mathbf T\dot{\boldsymbol\theta},\quad \mathbf V=mgl\begin{pmatrix}4&0\\0&1\end{pmatrix},\quad\mathbf T=ml^2\begin{pmatrix}8&2\\2&1\end{pmatrix}.}
$$

**Source correction.** The printed kinetic-energy matrix formula omits both time-derivative dots. It cannot hold as a function of angles alone: at $\boldsymbol\theta=0$, $\dot\theta_1\ne0$, $\dot\theta_2=0$, the actual kinetic energy is $4ml^2\dot\theta_1^2>0$, whereas the printed undifferentiated quadratic form vanishes.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

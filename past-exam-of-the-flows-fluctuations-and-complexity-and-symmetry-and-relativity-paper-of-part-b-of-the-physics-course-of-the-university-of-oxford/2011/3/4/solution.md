<h1 id="3/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For an infinitesimal perturbation $\boldsymbol\eta$, $\dot{\boldsymbol\eta}=J\boldsymbol\eta$, and

$$
\frac{d}{dt}\log|\boldsymbol\eta|=\frac{\boldsymbol\eta^TS\boldsymbol\eta}{|\boldsymbol\eta|^2},\qquad
S=\frac{J+J^T}{2}=\begin{pmatrix}0&0&(z-1)/2\\0&a&0\\(z-1)/2&0&x-c\end{pmatrix}.
$$

Thus the principal [instantaneous stretching rates](../../../../instantaneous-stretching-rate.md), called local [Lyapunov exponents](../../../../lyapunov-exponent.md) in the question, are

$$
\boxed{\lambda_y=a,\qquad
\lambda_\pm=\frac{x-c\pm\sqrt{(x-c)^2+(z-1)^2}}{2}.}
$$

For $z\ne1$, $\lambda_+>0$ and $\lambda_-<0$, while $a>0$. There are two instantaneously expanding orthogonal directions and one contracting direction. These are instantaneous norm-growth rates; the directions rotate along a trajectory, so this does not imply two positive long-time [Lyapunov exponents](../../../../lyapunov-exponent.md) or indefinitely exponential growth along fixed axes.

At $x=c$, put $s=\operatorname{sgn}(z-1)$. The [eigenvectors](../../../../eigenvector.md) and rates are

$$
\boxed{\mathbf e_+=\frac{(1,0,s)}{\sqrt2},\quad\lambda_+=\frac{|z-1|}{2};\qquad
\mathbf e_-=\frac{(1,0,-s)}{\sqrt2},\quad\lambda_-=-\frac{|z-1|}{2}.}
$$

The condition $|z-1|>2a$ makes $\mathbf e_+$ the fastest-growing direction, faster than $\mathbf e_y$; $\mathbf e_-$ is the fastest-contracting direction. Both lie at $45^\circ$ to the $x,z$ axes.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the flows, fluctuations and complexity and symmetry and relativity paper of Part B of the physics course of the University of Oxford](../../../split.md)
5. [Flows, fluctuations and complexity and symmetry and relativity paper of Part B of the physics course of the University of Oxford](../../../../flows-fluctuations-and-complexity-and-symmetry-and-relativity-paper-of-part-b-of-the-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

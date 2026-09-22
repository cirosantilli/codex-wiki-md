<h1 id="14a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the [Fourier transform](../../../../../../fourier-transform.md) in $x$. Since $\widetilde{\theta_{xx}}=-k^2\widetilde\theta$, the transformed [heat equation](../../../../../../heat-equation.md) is

$$
\frac{\partial\widetilde\theta}{\partial t}
=-Dk^2\widetilde\theta,
\qquad
\widetilde\theta(k,0)=\widetilde\Theta(k).
$$

Therefore

$$
\widetilde\theta(k,t)=e^{-Dk^2t}\widetilde\Theta(k).
$$

The given transform pair and the [convolution theorem](../../../../../../convolution-theorem.md) yield the [heat-kernel solution](../../../../../../heat-kernel-solution.md)

$$
\boxed{
\theta(x,t)=\frac1{\sqrt{4\pi Dt}}
\int_{-\infty}^{\infty}
\exp\left[-\frac{(x-\xi)^2}{4Dt}\right]
\Theta(\xi)\,d\xi}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14A](../../14a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

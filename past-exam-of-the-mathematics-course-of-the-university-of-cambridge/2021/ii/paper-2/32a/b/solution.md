<h1 id="32a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\Phi(t)=2t^4-t^2$. Its stationary points on $[0,1]$ are the endpoint $0$ and the interior point $1/2$, with

$$
\Phi(0)=0,quad \Phi''(0)=-2,\qquad
\Phi(1/2)=-\frac18,quad \Phi''(1/2)=4.
$$

The endpoint stationary-phase contribution to $\int_0^1e^{ix\Phi(t)}dt$ is

$$
\frac{\sqrt\pi}{2\sqrt x}e^{-i\pi/4},
$$

and the interior contribution is

$$
\sqrt{\frac\pi{2x}}e^{i(\pi/4-x/8)}.
$$

The nonstationary endpoint contributes only $O(x^{-1})$. Taking imaginary parts gives

$$
\boxed{I(x)\sim\sqrt{\frac\pi{2x}}
\left[\sin\left(\frac\pi4-\frac x8\right)-\frac12\right]}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [32A](../../32a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

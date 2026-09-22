<h1 id="39c/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Assume the condition in part (ii), so $m_0<0$. Substituting the wavevector solution into the vertical ray equation gives the linear [ordinary differential equation](../../../../../../../ordinary-differential-equation.md)

$$
\dot z+\gamma z=F(t),
$$

where

$$
F(t)
=\frac{-Nk_0m_0}
{\left(k_0^2e^{-2\gamma t}+m_0^2e^{2\gamma t}\right)^{3/2}}
>0.
$$

The [integrating factor](../../../../../../../integrating-factor.md) $e^{\gamma t}$ gives

$$
z(t)
=e^{-\gamma t}
\left[
z_0+\int_0^te^{\gamma s}F(s)\,ds
\right].
$$

The bracket is strictly positive, so $z(t)>0$ at every finite time. Moreover,

$$
F(t)=O(e^{-3\gamma t}),
\qquad
e^{\gamma t}F(t)=O(e^{-2\gamma t}),
$$

so the improper integral converges to a finite positive value. It follows that

$$
\boxed{z(t)\sim Ce^{-\gamma t}\longrightarrow0
\quad(t\to\infty)}
$$

for some $C>0$. The packet therefore approaches $z=0$ asymptotically and never reaches it at finite time. This is the [vertical trapping of an internal gravity wave by planar strain](../../../../../../../vertical-trapping-of-an-internal-gravity-wave-by-planar-strain.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [39C](../../../39c.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

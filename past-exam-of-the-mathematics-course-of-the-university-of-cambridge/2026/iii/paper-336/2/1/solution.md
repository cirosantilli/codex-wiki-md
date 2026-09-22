<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Set $\delta=\sqrt\epsilon$. The outer scale found below shows that the inner expansion requires the four asymptotic scales

$$
1,\qquad\delta,\qquad\epsilon\log\epsilon,\qquad\epsilon.
$$

Solving successively with $f_j(1)=0$ and matching the free homogeneous terms gives

$$
\boxed{
\begin{aligned}
f(r)\sim{}&
1-r^{-1/2}
+\sqrt{\pi\epsilon}\,(1-r^{-1/2})\\
&+\epsilon\log\epsilon\,(1-r^{-1/2})\\
&+\epsilon\left[
-\sqrt r+\log r+\pi+\frac C4
-\left(\pi+\frac C4-1\right)r^{-1/2}
\right].
\end{aligned}}
$$

This is valid for fixed $r=O(1)$.

To verify the differential-equation hierarchy, let $L[y]=y''+3y'/(2r)$. The leading terms satisfy

$$
L[f_0]=L[f_1]=0,
\qquad
f_0=1-r^{-1/2},
\qquad
f_1=\sqrt\pi f_0.
$$

At order $\epsilon$,

$$
L[f_2]=-f_0f_0',
$$

whose particular integral is $-\sqrt r+\log r+1$; the displayed homogeneous multiple of $1-r^{-1/2}$ is fixed by matching.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2](../../2.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

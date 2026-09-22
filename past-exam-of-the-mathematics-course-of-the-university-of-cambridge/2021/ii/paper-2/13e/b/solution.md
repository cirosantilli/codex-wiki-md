<h1 id="13e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the principal square root and deform the [Bromwich contour](../../../../../../bromwich-contour.md) around the negative real-axis branch cut. The pole at $p=0$ contributes $a$. The two boundary values at $p=-b$ combine to

$$
-ae^{-bt}\cos\left(x\sqrt{b/\kappa}\right).
$$

On the cut put $p=-v^2$; the jump of $e^{-x\sqrt{p/\kappa}}$ is $-2i\sin(xv/\sqrt\kappa)$ and $dp=-2v,dv$. Taking the principal value at $v=\sqrt b$ gives

$$
\boxed{T(x,t)=a\left[1-e^{-bt}\cos\left(\sqrt{b/\kappa}\,x\right)\right]
+\frac{2ab}{\pi}\mathcal P\int_0^\infty
\frac{e^{-v^2t}\sin(xv/\sqrt\kappa)}{v(v^2-b)}\,dv}.
$$

The expression has the prescribed boundary value and decays into the bar.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [13E](../../13e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

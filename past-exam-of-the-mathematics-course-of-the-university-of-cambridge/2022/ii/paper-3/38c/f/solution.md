<h1 id="38c/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Let $\mathbf e$ be the downward vertical unit vector and let the rod's weight after buoyancy be $W\mathbf e$. Force balance gives

$$
\mathbf R\mathbf U=W\mathbf e.
$$

Because

$$
\mathbf R
=c_1\mathbf t\mathbf t
+c_2(\mathbf 1-\mathbf t\mathbf t),
$$

its [matrix inverse](../../../../../../matrix-inverse.md) is

$$
\mathbf R^{-1}
=\frac1{c_1}\mathbf t\mathbf t
+\frac1{c_2}(\mathbf 1-\mathbf t\mathbf t).
$$

Using $\mathbf e\cdot\mathbf t=\cos\theta$ gives

$$
\mathbf U
=W\left[
\frac{\cos\theta}{c_1}\mathbf t
+\frac1{c_2}\left(\mathbf e-\cos\theta\,\mathbf t\right)
\right].
$$

Therefore

$$
\mathbf e\cdot\mathbf U
=W\left(\frac{\cos^2\theta}{c_1}
+\frac{\sin^2\theta}{c_2}\right),
$$

and

$$
|\mathbf U|
=W\sqrt{
\frac{\cos^2\theta}{c_1^2}
+\frac{\sin^2\theta}{c_2^2}
}.
$$

The required angle is consequently

$$
\boxed{
\cos\alpha
=
\frac{\cos^2\theta/c_1+\sin^2\theta/c_2}
{\sqrt{\cos^2\theta/c_1^2+\sin^2\theta/c_2^2}}
}.
$$

If $c_1=c_2$, then $\cos\alpha=1$, so the rod falls vertically. For an anisotropic rod with $c_2>c_1$, the component parallel to its long axis encounters less drag, and the settling direction is generally deflected toward that axis.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [38C](../../38c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

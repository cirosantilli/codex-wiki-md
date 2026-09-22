<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

Direct [matrix multiplication](../../../../../matrix-multiplication.md) gives

$$
\begin{array}{c|cc}
&|\uparrow\rangle&|\downarrow\rangle\\\hline
\hat S_x&\frac\hbar2|\downarrow\rangle&\frac\hbar2|\uparrow\rangle\\
\hat S_y&\frac{i\hbar}2|\downarrow\rangle&-\frac{i\hbar}2|\uparrow\rangle\\
\hat S_z&\frac\hbar2|\uparrow\rangle&-\frac\hbar2|\downarrow\rangle
\end{array}
$$

The normalized $S_x$ [eigenvectors](../../../../../eigenvector.md) are $(|\uparrow\rangle\pm|\downarrow\rangle)/\sqrt2$, and the $S_y$ [eigenvectors](../../../../../eigenvector.md) are $(|\uparrow\rangle\pm i|\downarrow\rangle)/\sqrt2$, with [eigenvalues](../../../../../eigenvalue.md) $\pm\hbar/2$ in each case.

For $N=|a|^2+|b|^2>0$, allowing for a possibly unnormalized input pair of coefficients,

$$
\boxed{\langle\hat S_z\rangle=\frac\hbar2\frac{|a|^2-|b|^2}{N},\qquad\langle\hat S^2\rangle=\frac{3\hbar^2}{4}.}
$$

For a normalized state $N=1$. The second result follows because each squared [Spin operator](../../../../../spin-operator.md) matrix equals $\hbar^2\hat I/4$.

The tilted component is $\hat S_{z'}=(\hbar/2)\begin{pmatrix}\cos\theta&\sin\theta\\\sin\theta&-\cos\theta\end{pmatrix}$. Its [eigenvalues](../../../../../eigenvalue.md) remain $\pm\hbar/2$, with one real phase convention for the normalized [eigenvectors](../../../../../eigenvector.md)

$$
\boxed{|+z'\rangle=\cos(\theta/2)|\uparrow\rangle+\sin(\theta/2)|\downarrow\rangle,\qquad|-z'\rangle=-\sin(\theta/2)|\uparrow\rangle+\cos(\theta/2)|\downarrow\rangle.}
$$

Projecting the initial $|\uparrow\rangle$ onto them gives **$P_+=\cos^2(\theta/2)$** and **$P_-=\sin^2(\theta/2)$**. Thus

$$
\boxed{\langle\hat S_{z'}\rangle=\frac\hbar2(P_+-P_-)=\frac\hbar2\cos\theta.}
$$

A smaller [expectation](../../../../../expected-value-split.md) does not imply a smaller individual [spin](../../../../../spin.md) [eigenvalue](../../../../../eigenvalue.md); it describes the probabilities of the same two measurement outcomes.

<a id="section-b/b9/image-rotating-the-measurement-axis-changes-spin-half-outcome-probabilities-rather-than-the-outcome-magnitudes"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-1-spin-projection.png)

**[Figure 3](#section-b/b9/image-rotating-the-measurement-axis-changes-spin-half-outcome-probabilities-rather-than-the-outcome-magnitudes). Rotating the measurement axis changes spin-half outcome probabilities rather than the outcome magnitudes**. [Source](paper-1-spin-projection.py).

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

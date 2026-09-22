<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Fourier transform of a derivative](../../../../../fourier-transform-of-a-derivative.md) gives $(-\omega^2-1)\widetilde y=-\widetilde f$. For $\lambda=1$,

$$
\boxed{\widetilde y(\omega)=\frac1{1+\omega^2}\left[\frac{1-i\omega}{(1-i\omega)^2+4}+\frac{1+i\omega}{(1+i\omega)^2+1}\right].}
$$

This selects the solution decaying at both time infinities. Indeed, the inverse transform of $1/(1+\omega^2)$ is the [one-dimensional modified Helmholtz Green function](../../../../../one-dimensional-modified-helmholtz-green-function.md) $K(t)=e^{-|t|}/2$, and the [convolution theorem](../../../../../convolution-theorem.md) gives $y=K*f$. The printed equation has homogeneous solutions $e^t,e^{-t}$, so these two decay conditions matter; no causal initial-value condition was specified.

For $t<0$, evaluate [Fourier inversion](../../../../../fourier-inversion-theorem.md) by closing the contour in the lower half-plane, where $e^{i\omega t}$ decays. The contour is clockwise. The enclosed [simple poles](../../../../../simple-pole.md) and [residues](../../../../../residue.md) of $\widetilde y$ are

$$
\begin{array}{c|c}
\omega&\operatorname{Res}\widetilde y\\\hline
-i&i/5\\
2-i&(-1+i)/16\\
-2-i&(1+i)/16
\end{array}
$$

Thus inversion equals $-i$ times the sum of the residues of $e^{i\omega t}\widetilde y$, giving

$$
\boxed{y(t)=e^t\left[\frac15+\frac18\cos(2t)-\frac18\sin(2t)\right],\qquad t<0.}
$$

As a check, applying $d^2/dt^2-1$ gives $-e^t\cos2t$. The convolution also gives $y(t)=e^{-t}[\tfrac18+\tfrac15\cos t+\tfrac25\sin t]$ for $t\geq0$; the two pieces have matching values $13/40$ and matching first derivatives $3/40$ at zero.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

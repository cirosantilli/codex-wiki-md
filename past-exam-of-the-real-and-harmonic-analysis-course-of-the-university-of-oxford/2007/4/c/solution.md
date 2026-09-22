<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $n\geq1$ put $q_n(t)=2nK_{n-1}(t)\sin(nt)$. Using $\sin(nt)=(e^{int}-e^{-int})/(2i)$ and the [Fourier coefficients](../../../../fourier-coefficient.md) of $K_{n-1}$ gives

$$
\widehat q_n(k)=-ik\quad(|k|\leq n).
$$

Indeed, when $1\leq k\leq n$ only the $e^{int}$ shift contributes, with coefficient $(-in)(1-|k-n|/n)=-ik$. For $-n\leq k\leq-1$ only the opposite shift contributes and gives $in(1-|k+n|/n)=-ik$; at $k=0$ both coefficients vanish.

If $P=\sum_{|k|\leq n}a_ke^{ikt}$, [convolution](../../../../convolution.md) multiplies its [Fourier coefficients](../../../../fourier-coefficient.md) by those of $q_n$. Thus $-P*q_n=\sum ika_ke^{ikt}=P'$, proving the exact identity. Since $K_{n-1}\geq0$ and has integral one,

$$
\boxed{\|P'\|_\infty\leq\|P\|_\infty\|q_n\|_1\leq2n\|P\|_\infty.}
$$

For $n=0$ the polynomial is constant and the bound is immediate. This elementary Fejér-kernel argument proves the requested estimate; the sharp [Bernstein inequality for trigonometric polynomials](../../../../bernstein-inequality-for-trigonometric-polynomials.md) has constant $n$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../split.md)
5. [Real and harmonic analysis course of the University of Oxford](../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

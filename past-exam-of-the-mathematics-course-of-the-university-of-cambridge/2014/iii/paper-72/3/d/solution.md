<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $y_n=\langle e_n,y\rangle$. Using the phase of $u_n$ in the [singular value system](../../../../../../singular-system-of-a-compact-operator.md), the [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md) becomes

$$
\boxed{f^\dagger=\sum_{n\in\mathbb Z}\frac{y_n}{c_n}e_n,\qquad\sum_{n\in\mathbb Z}\frac{|y_n|^2}{|c_n|^2}<\infty.}
$$

This gives the [admissible data for a periodic convolution inverse](../../../../../../admissible-data-for-a-periodic-convolution-inverse.md). Because the range is dense and the kernel is zero here, the domain of the inverse is exactly the range, not all of $L^2$.

For $y(x)=e^{\alpha x}$ and $\alpha\notin i\mathbb Z$,

$$
y_n=\frac1{\sqrt{2\pi}}\int_0^{2\pi}e^{(\alpha-in)x}dx=\frac{e^{2\pi\alpha}-1}{\sqrt{2\pi}(\alpha-in)}.
$$

The formal expression would consequently be

$$
f_{\rm formal}(x)=\frac{e^{2\pi\alpha}-1}{2\pi}\sum_{n\in\mathbb Z}\frac{e^{inx}}{(\alpha-in)c_n}.
$$

However, the [high-frequency obstruction for nonperiodic exponential data](../../../../../../high-frequency-obstruction-for-nonperiodic-exponential-data.md) prevents this from being a Hilbert-space solution. The numerator is nonzero, $|y_n|$ is asymptotic to a nonzero constant divided by $|n|$, and part (c) proved $|c_n|=o(1/|n|)$. Hence $|y_n/c_n|\to\infty$, so the [Picard criterion](../../../../../../picard-criterion.md) fails. **For $\alpha\notin i\mathbb Z$, $A^\dagger y$ is not defined in the specified [Hilbert space](../../../../../../hilbert-space-split.md).** The formal series is not a convergent generalized solution.

If $\alpha=im$ with $m\in\mathbb Z$, the data are a single periodic Fourier mode: $y_n=\sqrt{2\pi}\delta_{nm}$. Then there is an exact unique solution,

$$
\boxed{f^\dagger(x)=\frac{e^{imx}}{c_m}\quad\text{when }\alpha=im.}
$$

In particular, if the intended parameter is real, only $\alpha=0$ is admissible, giving $f^\dagger=1/c_0$.

For the inadmissible cases the inverse problem still has approximate solutions $f_N=\sum_{|n|\leq N}(y_n/c_n)e_n$: their images are Fourier projections converging to $y$ in $L^2$, while their [norms](../../../../../../norm.md) diverge. Thus the least-squares residual has infimum zero but no minimizer. This distinguishes an undefined exact inverse from a regularized truncated reconstruction; it is the necessary qualification to the question's unrestricted constant $\alpha$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

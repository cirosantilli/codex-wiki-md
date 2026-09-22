<h1 id="4b/solution">Solution</h1>

↑ **Parent:** [4B](../4b.md)

Use the angular-frequency [Fourier transform](../../../../../fourier-transform.md)

$$
\widehat f(k)=\int_{-\infty}^{\infty}f(x)e^{-ikx}\,dx.
$$

Then

$$
\boxed{\widehat f(k)=A\int_{-1}^{1}e^{-ikx}\,dx
=2A\frac{\sin k}{k}},
$$

with the continuous value $\widehat f(0)=2A$.

The [convolution](../../../../../convolution.md) $(f*f)(x)$ is $A^2$ times the length of the overlap of the intervals $[-1,1]$ and $[x-1,x+1]$. Thus

$$
\boxed{(f*f)(x)=
\begin{cases}
A^2(2-|x|),&|x|\le2,\\
0,&|x|>2.
\end{cases}}
$$

The [convolution theorem](../../../../../convolution-theorem.md) states, for this convention, that

$$
\widehat{u*v}(k)=\widehat u(k)\widehat v(k).
$$

Since $g=(B/A^2)(f*f)$, it follows that

$$
\boxed{\widehat g(k)
=4B\left(\frac{\sin k}{k}\right)^2},
$$

again interpreted continuously at $k=0$, where $\widehat g(0)=4B$.

## ↑ Ancestors (10)

1. [4B](../4b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="10f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $x\ne0$, $f(x)=|x|^x=e^{x\log|x|}$, so $f'(x)=|x|^x(\log|x|+1)$. Although $x\log|x|\to0$ makes $f$ continuous at zero, $(f(x)-1)/x\sim\log|x|\to-\infty$, so it is not differentiable there.

Since the [cosine function](../../../../../../cosine.md) is even, $g(x)=\cos|x|=\cos x$, so it is differentiable everywhere with $g'(x)=-\sin x$. Finally, $h(x)=x|x|$ is differentiable everywhere, including at zero, and $h'(x)=2|x|$. Therefore

$$
\boxed{f'(x)=|x|^x(\log|x|+1)\ (x\ne0),\qquad g'(x)=-\sin x,\qquad h'(x)=2|x|.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10F](../../10f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

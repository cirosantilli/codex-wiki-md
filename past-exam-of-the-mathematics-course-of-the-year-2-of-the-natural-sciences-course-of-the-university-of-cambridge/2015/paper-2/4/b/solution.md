<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a branch of the [complex logarithm](../../../../../complex-logarithm.md) with $-\pi/2<\arg z<3\pi/2$, placing its [branch cut](../../../../../branch-cut.md) down the negative imaginary axis. Thus $\operatorname{Log} x=\ln x$ for $x>0$, while $\operatorname{Log}(-x)=\ln x+i\pi$ on the negative real axis for $x>0$.

Integrate $\operatorname{Log} z/(z^2+a^2)$ around an upper [semicircle](../../../../../semicircle.md), with a small clockwise semicircular indentation above zero. The large arc contributes $O(\ln R/R)\to0$, and the small arc contributes $O(\varepsilon|\ln\varepsilon|)\to0$. The only enclosed [pole](../../../../../pole.md) is $ia$, with

$$
\operatorname{Res}_{z=ia}\frac{\operatorname{Log} z}{z^2+a^2}=\frac{\ln a+i\pi/2}{2ia}.
$$

Writing $I(a)$ for the required integral, the negative real segment contributes $I(a)+i\pi\int_0^\infty dx/(x^2+a^2)$. Hence the [residue theorem](../../../../../residue-theorem.md) gives

$$
2I(a)+\frac{i\pi^2}{2a}=\frac\pi a\left(\ln a+\frac{i\pi}{2}\right).
$$

The imaginary terms cancel, leaving

$$
\boxed{\int_0^\infty\frac{\ln x}{x^2+a^2}\,dx=\frac{\pi\ln a}{2a}.}
$$

The integral converges at both endpoints because $|\ln x|$ is integrable near zero and $\ln x/x^2$ is integrable at infinity. As a real-variable check, scaling $x=au$ reduces the result to the vanishing first logarithmic moment at $a=1$, one of the [logarithmic moments of the Cauchy kernel](../../../../../logarithmic-moments-of-the-cauchy-kernel.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

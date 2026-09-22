<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [function](../../../../../function-split.md) is even, so every sine coefficient is zero. Its mean coefficient is

$$
a_0=\frac2\pi\int_0^\pi\sin x\,\mathrm dx=\frac4\pi.
$$

For $n\geq1$, compute $a_n=(2/\pi)\int_0^\pi\sin x\cos(nx)\,\mathrm dx$. The product-to-sum identity makes this integral zero for odd $n$ and gives $-4/(\pi(n^2-1))$ for even $n$. Thus the missing [Fourier coefficients](../../../../../fourier-coefficient.md) are **$a_n=0$ for odd $n$ and $b_n=0$ for every $n$**, with $a_0=4/\pi$. Equivalently,

$$
|\sin x|=\frac2\pi-\frac4\pi\sum_{m=1}^\infty\frac{\cos(2mx)}{4m^2-1}.
$$

The [Fourier series](../../../../../fourier-series-split.md) converges to this continuous periodic [function](../../../../../function-split.md); there is no jump value to average.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

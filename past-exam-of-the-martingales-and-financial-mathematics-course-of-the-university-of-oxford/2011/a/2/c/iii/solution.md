<h1 id="a/2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $E_n=\{|X_n-1|=n\}$. These events are independent and $\sum_{n\geq2}\mathbb P(E_n)=\sum_{n\geq2}1/(n\log n)=\infty$. By the [Borel-Cantelli second lemma](../../../../../../borel-cantelli-second-lemma.md), they occur infinitely often almost surely.

If $S_n/n$ had any finite sample-path limit, then

$$
\frac{X_{n+1}}n=\frac{S_n}n-\frac{n-1}{n}\frac{S_{n-1}}{n-1}\longrightarrow0.
$$

But on $E_{n+1}$, $|X_{n+1}|/n$ is either $1$ or $(n+2)/n$, contradicting this convergence infinitely often. Therefore **the averages have no finite almost sure limit**. This is a [rare-jump counterexample to a strong law with convergent first-moment averages](../../../../../../rare-jump-counterexample-to-a-strong-law-with-convergent-first-moment-averages.md).

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)

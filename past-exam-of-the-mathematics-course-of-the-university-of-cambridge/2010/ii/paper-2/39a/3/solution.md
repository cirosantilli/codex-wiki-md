<h1 id="39a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Counting every twiddle-factor product, including multiplication by one, the recurrence is $M(n)=2M(n/2)+n/2$, with $M(1)=0$. Each of the $p$ levels costs $n/2$ products, so

$$
\boxed{M(2^p)=p\,2^{p-1}=\tfrac n2\log_2n}.
$$

If products by one are omitted, every block saves one product. There are $n-1$ blocks across all stages, giving $M_{\rm nonunit}(n)=\frac n2\log_2n-n+1$. The conventional complexity in either convention is $O(n\log n)$; additional savings are possible by treating multiplication by $\pm i$ as component swaps and sign changes.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [39A](../../39a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

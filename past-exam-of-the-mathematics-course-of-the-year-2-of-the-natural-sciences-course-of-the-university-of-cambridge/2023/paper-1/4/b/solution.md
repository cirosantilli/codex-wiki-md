<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the necessary [derivatives](../../../../../derivative.md) decay enough for all boundary terms to vanish. One [integration by parts](../../../../../integration-by-parts.md) gives

$$
\widetilde{f'}(k)=\int_{\mathbb R}f'(x)e^{-ikx}\,dx=ik\widetilde f(k).
$$

Repeating proves the [Fourier transform of a derivative](../../../../../fourier-transform-of-a-derivative.md) rule $\boxed{\widetilde{f^{(m)}}=(ik)^m\widetilde f}$. On the other hand, differentiation under the [integral](../../../../../integral-split.md) gives

$$
\frac{d^m\widetilde f}{dk^m}=\int_{\mathbb R}(-ix)^mf(x)e^{-ikx}\,dx,
$$

and therefore $\boxed{\widetilde{x^mf}=i^m\widetilde f^{(m)}}$.

Write $p_n(x)=\sum_{j=0}^na_jx^j$, with $a_n\ne0$. Applying the second rule and part (a) gives

$$
\mathcal F[p_n(x)g(x)](k)=\sqrt{2\pi}\sum_{j=0}^na_ji^jg^{(j)}(k)=q_n(k)e^{-k^2/2},
$$

where

$$
\boxed{q_n(k)=\sqrt{2\pi}\sum_{j=0}^na_ji^jr_j(k).}
$$

Only the $j=n$ term can contribute degree $n$. Its leading coefficient is $\sqrt{2\pi}a_n(-i)^n\ne0$, so $q_n$ has exactly the same degree $n$, with no possible leading-term cancellation. The coefficients of this transformed [polynomial](../../../../../polynomial-split.md) can be complex even when those of $p_n$ are real.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
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

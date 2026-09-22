<h1 id="18h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [primitive root of unity](../../../../../../primitive-root-of-unity.md) $\xi_n$ satisfies $\xi_n^n=1$ and $\xi_n^j\ne1$ for $1\le j<n$, equivalently it has multiplicative order $n$. A positive [characteristic of a field](../../../../../../characteristic-of-a-field.md) must be prime: if its least positive value $p$ factored as $ab$ with $1<a,b<p$, the two nonzero field elements $a\cdot1$ and $b\cdot1$ would have product zero. If this prime $p$ divides $n$, put $m=n/p$. In characteristic $p$, the binomial coefficients $\binom pj$ for $0<j<p$ vanish because their integer numerators contain $p$ and their denominators do not. Thus $(X-1)^p=X^p-1$. It follows that $(\xi_n^m-1)^p=\xi_n^n-1=0$. A field has no nonzero nilpotent element, so $\xi_n^m=1$, contradicting primitivity. Consequently $\boxed{\operatorname{char}K\nmid n}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18H](../../18h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

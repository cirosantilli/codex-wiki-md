<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write

$$
V(\phi)=\frac12(q^2-\phi^2)^2(p^2-\phi^2)^2,
\qquad q>p>0.
$$

The four vacua are $-q,-p,p,q$. Hence there are three adjacent [scalar-field kink](../../../../../scalar-field-kink.md) sectors, $(-q,-p)$, $(-p,p)$ and $(p,q)$, together with their three reversed antikinks. With

$$
W'(\phi)=(q^2-\phi^2)(p^2-\phi^2),
\qquad
W(\phi)=p^2q^2\phi-\frac{p^2+q^2}{3}\phi^3+\frac15\phi^5,
$$

the [Bogomolny bound](../../../../../bogomolny-bound.md) gives $E=|W(\phi_+)-W(\phi_-)|$. The central kink obeys $\phi'=W'(\phi)$ and has

$$
E_c=\frac{4p^3}{15}(5q^2-p^2).
$$

The two outer kinks obey $\phi'=-W'(\phi)$ and have equal energy

$$
E_o=\frac{2}{15}(q-p)^3(p^2+3pq+q^2).
$$

For the kink passing through zero, choose $\phi(0)=0$. Its profile is determined implicitly by

$$
\boxed{
\frac1{q^2-p^2}\left[\frac1p\operatorname{artanh}\frac{\phi}{p}-\frac1q\operatorname{artanh}\frac{\phi}{q}\right]=x
}.
$$

If $q=p$, the central equation becomes $\phi'=(p^2-\phi^2)^2$, so

$$
\boxed{
\frac{\phi}{2p^2(p^2-\phi^2)}+\frac1{2p^3}\operatorname{artanh}\frac\phi p=x
}.
$$

For $q=p+\varepsilon$,

$$
E_o=\frac23p^2\varepsilon^3+O(\varepsilon^4),
\qquad
E_c=\frac{16}{15}p^5+O(\varepsilon),
$$

so the leading ratio is

$$
\boxed{E_o:E_c:E_o=1:\frac85(p/\varepsilon)^3:1}.
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 308](../../paper-308-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

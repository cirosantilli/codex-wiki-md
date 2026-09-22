<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For an [algebraically closed field](../../../../../../algebraically-closed-field.md) $k$, the [Weak Hilbert Nullstellensatz](../../../../../../weak-hilbert-nullstellensatz.md) says that every maximal ideal of $k[x_1,\ldots,x_n]$ is

$$
(x_1-a_1,\ldots,x_n-a_n)
$$

for a unique $a\in k^n$. Equivalently, every proper ideal has a common zero. The [Strong Hilbert Nullstellensatz](../../../../../../strong-hilbert-nullstellensatz.md) says that for every ideal $I$,

$$
\boxed{I(V(I))=\sqrt I}.
$$

To deduce the strong form, let $f$ vanish on $V(I)$ and introduce a variable $y$. The equations in $I$ together with $1-yf$ have no common zero: a common zero would satisfy both $f=0$ and $yf=1$. The weak theorem therefore gives

$$
1=\sum_i a_i(x,y)g_i(x)+b(x,y)(1-yf(x)),
\qquad g_i\in I.
$$

Substitute $y=f^{-1}$ in the localization $k[x_1,\ldots,x_n,f^{-1}]$. The last term vanishes, and clearing a power of $f$ yields $f^N\in I$. Thus $f\in\sqrt I$. The reverse inclusion is immediate, completing the [Rabinowitsch trick](../../../../../../rabinowitsch-trick.md) proof.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

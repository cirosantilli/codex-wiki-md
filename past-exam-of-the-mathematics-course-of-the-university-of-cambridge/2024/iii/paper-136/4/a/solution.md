<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Because $k$ is a [perfect field](../../../../../../perfect-field.md), for each $a\in k$ choose a compatible sequence

$$
a_0=a,
\qquad a_{n+1}^p=a_n,
$$

and choose arbitrary lifts $x_n\in\mathcal O_K$ of $a_n$. If $u\equiv v\pmod{\pi^m}$, the [binomial theorem](../../../../../../binomial-theorem.md) and the fact that the residue characteristic is $p$ give

$$
u^p\equiv v^p\pmod{\pi^{m+1}}.
$$

It follows that $x_{n+1}^{p^{n+1}}\equiv x_n^{p^n}\pmod{\pi^{n+1}}$. Thus $(x_n^{p^n})$ is Cauchy, and completeness defines

$$
[a]=\lim_{n\to\infty}x_n^{p^n}.
$$

The same congruence shows that the limit is independent of all lift choices. Taking products before passing to the limit proves $[ab]=[a][b]$, and reduction gives $[a]\equiv a\pmod\pi$.

For uniqueness, let $s,t:k\to\mathcal O_K$ be two multiplicative lifts. Given $a$ and any $n$, choose $b\in k$ with $b^{p^n}=a$. Since $s(b)\equiv t(b)\pmod\pi$, repeated powering yields

$$
s(a)=s(b)^{p^n}\equiv t(b)^{p^n}=t(a)\pmod{\pi^{n+1}}.
$$

Completeness and separation force $s(a)=t(a)$. This is the unique [Teichmuller lift](../../../../../../teichmuller-representative.md).

For $x\in\mathcal O_K$, let $a_0$ be its residue and put $x_1=(x-[a_0])/\pi$. Repeat with $x_1,x_2,\ldots$. Induction gives

$$
x=\sum_{i=0}^{N-1}[a_i]\pi^i+\pi^Nx_N.
$$

The remainder tends to zero, proving the [Teichmuller expansion](../../../../../../teichmuller-expansion.md)

$$
x=\sum_{i=0}^{\infty}[a_i]\pi^i.
$$

Reduction after subtracting successive partial sums also proves uniqueness of the digits.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

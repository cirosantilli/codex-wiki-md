<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Church numeral](../../../../../../church-numeral.md) corresponding to the [natural number](../../../../../../natural-number.md) $n$ is

$$
c_n=\lambda f.\lambda x.f^n x.
$$

A function $g:\mathbb N^k\to\mathbb N$ is a [lambda-definable function](../../../../../../lambda-definable-function.md) if some closed lambda term $G$ satisfies

$$
G c_{n_1}\cdots c_{n_k}\equiv_\beta c_{g(n_1,\ldots,n_k)}
$$

for all natural numbers $n_1,\ldots,n_k$.

Define

$$
\operatorname{Succ}=\lambda n.\lambda f.\lambda x.f(nfx).
$$

Then [beta reduction](../../../../../../beta-reduction.md) gives

$$
\operatorname{Succ}\,c_n
\equiv_\beta\lambda f.\lambda x.f(f^n x)
=c_{n+1}.
$$

**Therefore the [successor function](../../../../../../successor-function.md) is lambda-definable; this is the [lambda definition of the successor function](../../../../../../lambda-definition-of-the-successor-function.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

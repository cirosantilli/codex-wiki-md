<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each [prime number](../../../../../../prime-number.md) $p\nmid a$, the congruence $an+1\equiv0\pmod p$ removes exactly one [residue class](../../../../../../residue-class.md) of $n$ modulo $p$; for $p\mid a$, it removes none. The dimension-one [upper-bound sieve](../../../../../../upper-bound-sieve.md) therefore gives

$$
\bigl|\{n\leq x:(an+1,\prod_{w\leq p\leq z}p)=1\}\bigr|
\ll x\prod_{\substack{w\leq p\leq z\\p\nmid a}}
\left(1-\frac1p\right).
$$

Separating the primes that divide $a$ bounds the product by

$$
\prod_{w\leq p\leq z}\left(1-\frac1p\right)
\prod_{p\mid a}\left(1-\frac1p\right)^{-1}.
$$

The ratio form of [Mertens theorem](../../../../../../mertens-theorems.md) says that the first product is $\ll\log w/\log z$. Hence

$$
\boxed{\bigl|\{n\in[1,x]:an+1\text{ has no prime factor in }[w,z]\}\bigr|
\ll x\frac{\log w}{\log z}
\prod_{p\mid a}\left(1-\frac1p\right)^{-1}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

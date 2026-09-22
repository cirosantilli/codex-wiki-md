<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a positive integer $n$, let $v_2(n)$ be its [2-adic valuation](../../../../../../2-adic-valuation.md) and let $k(n)=\lfloor\log_2 n\rfloor$. Use the four-colour [dyadic valuation and scale colouring](../../../../../../dyadic-valuation-and-scale-colouring.md)

$$
\boxed{\chi(n)=\bigl(v_2(n)\bmod2,\ k(n)\bmod2\bigr).}
$$

Suppose an increasing infinite sequence had all its two indicated kinds of pair sums in one colour. There are two exhaustive possibilities for its valuations.

If the valuations are bounded, infinitely many terms have one fixed valuation $t$. Among them, infinitely many have the same odd part modulo four. Choose two such terms $a<b$. Their odd parts have sum congruent to two modulo four, while the odd part of $a+2b$ is odd. Hence

$$
v_2(a+b)=t+1,\qquad v_2(a+2b)=t.
$$

Their first colour coordinates differ, contradicting monochromaticity.

If the valuations are unbounded, fix one term $a$ and choose a later $b$ with $2^{v_2(b)}>a$. Put $k=\lfloor\log_2b\rfloor$. The distance $2^{k+1}-b$ is a positive multiple of $2^{v_2(b)}$, so it exceeds $a$. Similarly $2^{k+2}-2b$ exceeds $a$. Therefore adding $a$ crosses neither upper dyadic boundary:

$$
\lfloor\log_2(a+b)\rfloor=k,\qquad \lfloor\log_2(a+2b)\rfloor=k+1.
$$

Their second colour coordinates differ, again a contradiction. Thus **this four-colouring admits no such increasing infinite sequence**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

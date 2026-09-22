<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One form of [Hensel lemma](../../../../../../hensel-s-lemma.md) is: if $R$ is a complete [discrete valuation ring](../../../../../../discrete-valuation-ring.md), $f\in R[X]$, and $f(a_1)\equiv0\pmod\pi$ while $f'(a_1)\not\equiv0\pmod\pi$, then there is a unique $\alpha\in R$ with $f(\alpha)=0$ and $\alpha\equiv a_1\pmod\pi$.

Inductively, if $f(a_n)\equiv0\pmod{\pi^n}$, choose $t$ modulo $\pi$ so that

$$
f(a_n)+\pi^ntf'(a_n)\equiv0\pmod{\pi^{n+1}}
$$

and put $a_{n+1}=a_n+\pi^nt$. The unit $f'(a_n)$ makes $t$ unique. The resulting sequence is Cauchy, so completeness gives a root $\alpha$. Applying the same first-order congruence to two roots proves uniqueness.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

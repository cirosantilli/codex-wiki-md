# Cauchy mean value theorem

↑ **Parent:** [Mean value theorem](mean-value-theorem.md)

For $a<b$ and [real-valued functions](real-valued-function.md) $f,g$ that are [continuous](continuous-function.md) on the [closed interval](closed-real-interval.md) $[a,b]$ and [differentiable](differentiable-function.md) on the [open interval](open-interval.md) $(a,b)$, there exists $\xi\in(a,b)$ with

$$
[f(b)-f(a)]g'(\xi)=[g(b)-g(a)]f'(\xi).
$$

Apply [Rolle's theorem](rolle-theorem.md) to the [linear combination](linear-combination.md) $h(x)=[f(b)-f(a)]g(x)-[g(b)-g(a)]f(x)$, which has equal endpoint values. The displayed product identity permits zero [derivatives](derivative.md). For the ratio form, additionally assume $g'(x)\ne0$ for every $x\in(a,b)$. Then [Rolle's theorem](rolle-theorem.md) ensures $g(b)\ne g(a)$, so both denominators below are nonzero:

$$
\frac{f(b)-f(a)}{g(b)-g(a)}=\frac{f'(\xi)}{g'(\xi)}.
$$

Neither [derivative](derivative.md) needs to be [continuous](continuous-function.md), and $f'$ may vanish. Choosing $g(x)=x$ recovers the [mean value theorem](mean-value-theorem.md); the ratio form also gives the zero-over-zero endpoint case of [L'Hôpital's rule](l-hopital-s-rule.md). [Jiří Lebl, Basic Analysis I, Section 4.2, Theorem 4.2.5](https://www.jirka.org/ra/html/sec_mvt.html)

## ↑ Ancestors (7)

1. [Mean value theorem](mean-value-theorem.md)
2. [Calculus](calculus-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-1/9d/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-1/11d/solution.md)

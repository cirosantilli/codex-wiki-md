# Weighted dilation kernel

↑ **Parent:** [Fubini's theorem](fubini-s-theorem.md)

Let $f$ be a [Borel measurable function](borel-measurable-function.md) in [L1 space](l1-space.md) on $\mathbb R$, and let $a,b$ be measurable real functions of $x$ with $b(x)>0$ and $W=\int_{\mathbb R}|a(x)|/b(x)\,dx<\infty$. The joint integrand $G(x,y)=a(x)f(b(x)y)$ is measurable, and [Tonelli's theorem](tonelli-theorem.md) followed by [Lebesgue substitution on an interval](lebesgue-substitution-on-an-interval.md) gives

$$
\|G\|_{L^1(\mathbb R^2)}=W\|f\|_{L^1(\mathbb R)}.
$$

For each fixed $x$, substitute $z=b(x)y$ in the inner $y$ integral. The absolute Jacobian is $1/b(x)$, leaving $|a(x)|\|f\|_1/b(x)$. Integrating in $x$ proves the formula and [absolute integrability](integrability.md). [Fubini's theorem](fubini-s-theorem.md) then permits both orders of signed integration, giving

$$
\iint_{\mathbb R^2}G(x,y)\,dx\,dy=
\left(\int_{\mathbb R}\frac{a(x)}{b(x)}\,dx\right)
\left(\int_{\mathbb R}f(y)\,dy\right).
$$

The one-dimensional sections are integrable for [almost every](almost-everywhere.md) value of the other variable; the theorem does not assert integrability of every section.

## ↑ Ancestors (7)

1. [Fubini's theorem](fubini-s-theorem.md)
2. [Measure theory](measure-theory-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-integration-course-of-the-university-of-oxford/2017/3/b/ii/solution.md)

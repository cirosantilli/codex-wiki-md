# Lavrentiev phenomenon

↑ **Parent:** [Direct method in the calculus of variations](direct-method-in-the-calculus-of-variations.md)

A Lavrentiev gap is a strict change in an [infimum](infimum.md) when the admissible regularity class is restricted, despite retaining the same endpoint values. For example $I(u)=\int_0^1(u^3-x)^2u'^6dx$ with $u(0)=0,u(1)=1$ has value zero at the absolutely continuous function $u=x^{1/3}$. Every Lipschitz competitor has a uniform positive lower energy bound. Indeed its ratio to $x^{1/3}$ starts at zero, so let $x_0$ be its first crossing of $u(x)=x^{1/3}/2$. Before that point, $|u^3-x|\geq7x/8$. [Holder inequality](holder-inequality.md) gives

$$
\left(\frac{x_0^{1/3}}2\right)^6\leq\left(\int_0^{x_0}x^2|u'|^6dx\right)\left(\frac53x_0^{3/5}\right)^5.
$$

Thus $I(u)\geq(49/4096)(3/5)^5/x_0\geq(49/4096)(3/5)^5>0$. This proves a gap directly. The example's integrand lacks a uniform superlinear lower bound along its zero set; it illustrates the admissible-class issue rather than by itself furnishing a counterexample under stronger coercivity assumptions.

## ↑ Ancestors (6)

1. [Direct method in the calculus of variations](direct-method-in-the-calculus-of-variations.md)
2. [Calculus of variations](calculus-of-variations-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford/2008/b/8/a/iv/solution.md)

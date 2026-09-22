# Resultant as a product over roots

↑ **Parent:** [Resultant](resultant.md)

Write $f(x)=a_m\prod_{i=1}^m(x-\alpha_i)$ and $g(x)=b_n\prod_{j=1}^n(x-\beta_j)$ in an [algebraic closure](algebraic-closure.md), counting [multiplicity of a root](multiplicity-of-a-root.md). The coefficient-row convention above gives

$$
\operatorname{Res}(f,g)
=a_m^n\prod_{i=1}^m g(\alpha_i)
=a_m^n b_n^m\prod_{i=1}^m\prod_{j=1}^n(\alpha_i-\beta_j).
$$

This makes the shared-[root of a polynomial](root-of-a-polynomial.md) test transparent: a factor vanishes precisely when one $\alpha_i$ equals one $\beta_j$. Swapping the two [polynomials](polynomial-split.md) reverses the sign of all $mn$ differences, giving $\operatorname{Res}(g,f)=(-1)^{mn}\operatorname{Res}(f,g)$.[Algebraic Techniques and Semidefinite Optimization, MIT 6.972, Spring 2006; MIT 6.972, Lecture 6, pp. 6-1–6-2, root products, equation (1), and argument-swap sign](algebraic-techniques-and-semidefinite-optimization-mit-6-972-spring-2006/lecture-6-resultants-and-discriminants.md)

The value measures an algebraic product, not a normalized geometric distance. Replacing $f$ by $cf$ for nonzero $c\in K$ leaves its [roots of a polynomial](root-of-a-polynomial.md) unchanged but multiplies the [resultant](resultant.md) by $c^n$. Therefore a small numerical [resultant](resultant.md) alone does not quantify how close two sets of [roots of a polynomial](root-of-a-polynomial.md) are. Exact zero testing and numerical sensitivity are different questions.

A [multiple root](multiple-root.md) of a [polynomial](polynomial-split.md) is also a [root of a polynomial](root-of-a-polynomial.md) of its [formal derivative](formal-derivative.md). In [characteristic zero](characteristic-zero.md), for $\deg f=m\geq2$, the associated [discriminant](discriminant.md) is

$$
\operatorname{Disc}(f)=\frac{(-1)^{m(m-1)/2}}{a_m}\operatorname{Res}(f,f').
$$

For example, $h(x)=x^2+s$ gives $\operatorname{Res}(h,2x)=4s$ and $\operatorname{Disc}(h)=-4s$. The two [roots of a polynomial](root-of-a-polynomial.md) merge precisely at $s=0$.[Algebraic Techniques and Semidefinite Optimization, MIT 6.972, Spring 2006; MIT 6.972, Lecture 6, p. 6-2, Definition 2: discriminant as a polynomial–derivative resultant](algebraic-techniques-and-semidefinite-optimization-mit-6-972-spring-2006/lecture-6-resultants-and-discriminants.md)

## ↑ Ancestors (6)

1. [Resultant](resultant.md)
2. [Polynomial](polynomial-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

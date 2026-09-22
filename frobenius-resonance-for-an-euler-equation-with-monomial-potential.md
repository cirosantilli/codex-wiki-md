# Frobenius resonance for an Euler equation with monomial potential

↑ **Parent:** [Frobenius method](frobenius-method.md)

For $a>0$, $b\ne0$, and a positive integer $\beta$, consider $x^2y''+xy'+(-a^2+bx^\beta)y=0$ near $x=0$. Its [indicial roots](indicial-root.md) are $a,-a$. The first [Frobenius solution](frobenius-solution.md), normalized to leading coefficient one, is $y_+=x^a\sum_{k\geq0}c_{k\beta}x^{k\beta}$, with $c_{k\beta}=-bc_{(k-1)\beta}/[k\beta(k\beta+2a)]$. If $N=2a$ is a positive integer, a second pure [Frobenius solution](frobenius-solution.md) with leading coefficient one would require

$$
n(n-N)d_n=-bd_{n-\beta},\qquad d_0=1,\qquad d_j=0\ (j<0).
$$

Before $n=N$, induction makes $d_n=0$ for indices not divisible by $\beta$. If $\beta$ divides $N$, the coefficient $d_{N-\beta}$ is nonzero, and the exceptional equation $0=-bd_{N-\beta}$ is impossible. If $\beta$ does not divide $N$, the right-hand side is zero and $d_N$ is free. Thus, in the [Frobenius case classification](frobenius-case-classification.md), a positive integer gap gives Case IIIa exactly when $\beta$ divides $2a$, and Case IIIb otherwise.

The coefficient of the necessary [logarithm](logarithm.md) can also be calculated. Let $L=x^2d^2/dx^2+x\,d/dx-a^2+bx^\beta$. The [product rule](product-rule.md) gives $L(y_+\log x)=2xy_+'$. Therefore a second solution $x^{-a}\sum d_nx^n+Ky_+\log x$, with $d_0=1$, has

$$
K=-\frac{bd_{N-\beta}}{N}.
$$

For $N=m\beta$ the preceding [recurrence relation](recurrence-relation.md) gives $d_{(m-1)\beta}=b^{m-1}/[\beta^{2m-2}((m-1)!)^2]$, so

$$
K=-\frac{b^m}{m\beta^{2m-1}((m-1)!)^2}\ne0.
$$

This proves that the [logarithm](logarithm.md) cannot disappear for a special nonzero value of $b$. For $a=0$, [reduction of order](reduction-of-order.md) instead produces the repeated-root [Logarithmic Frobenius solution](logarithmic-solution-from-a-repeated-frobenius-exponent.md) directly.

## ↑ Ancestors (8)

1. [Frobenius method](frobenius-method.md)
2. [Regular singular point](regular-singular-point.md)
3. [Fuchsian differential equation](fuchsian-differential-equation.md)
4. [Complex analysis](complex-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-differential-equations-2-course-of-the-university-of-oxford/2021/2/c/solution.md)

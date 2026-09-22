<h1 id="g/g1/solution">Solution</h1>

↑ **Parent:** [G1](../g1.md)

Let $\eta$ be a smooth [variation](../../../../variation.md) with $\eta(a)=\eta(b)=0$. Assuming the usual continuous second derivatives of $F$, stationarity of the [functional](../../../../functional.md) under $y+t\eta$ gives its [first variation](../../../../first-variation.md)

$$
0=\left.\frac d{dt}J[y+t\eta]\right|_{t=0}=\int_a^b(F_y\eta+F_{y'}\eta')\,dx.
$$

[Integration by parts](../../../../integration-by-parts.md) removes the derivative of $\eta$; its boundary term vanishes because the endpoint values are fixed. Thus

$$
\int_a^b\left(F_y-\frac d{dx}F_{y'}\right)\eta\,dx=0
$$

for every such [variation](../../../../variation.md). The [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) implies the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) $F_y=(d/dx)F_{y'}$.

For [arc length](../../../../arc-length.md), $F=\sqrt{1+(y')^2}$, so

$$
\frac d{dx}\frac{y'}{\sqrt{1+(y')^2}}=0.
$$

The function $s\mapsto s/\sqrt{1+s^2}$ is strictly increasing; hence $y'$ is constant. With endpoints $(a,A)$ and $(b,B)$, $a<b$, the extremal is

$$
\boxed{y(x)=A+\frac{B-A}{b-a}(x-a)}.
$$

It is also the global shortest curve: integrating the unit displacement vector dotted with the curve velocity gives the endpoint distance, which is at most the integrated speed by [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md); the straight segment attains equality. A vertical segment is described parametrically or after rotating axes, since it cannot be represented by $y(x)$ on a nontrivial horizontal interval.

## ↑ Ancestors (12)

1. [G1](../g1.md)
2. [G](../../g.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

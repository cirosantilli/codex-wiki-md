<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $\tan x=a_1x+a_3x^3+a_5x^5+O(x^7)$. Multiplying by the [cosine](../../../cosine.md) [Maclaurin series](../../../maclaurin-series.md) and comparing with the [sine](../../../sine.md) series gives

$$
(a_1x+a_3x^3+a_5x^5)\left(1-\frac{x^2}{2}+\frac{x^4}{24}\right)=x-\frac{x^3}{6}+\frac{x^5}{120}+O(x^7).
$$

Coefficient comparison yields $a_1=1$, $a_3-a_1/2=-1/6$ and $a_5-a_3/2+a_1/24=1/120$. Hence

$$
\boxed{\tan x=x+\frac{x^3}{3}+\frac{2x^5}{15}+O(x^7)}.
$$

Substitute $u=\tan x$ into $e^u=1+u+u^2/2+u^3/6+O(u^4)$. Keeping one extra order to make the term-counting explicit,

$$
e^{\tan x}=1+x+\frac{x^2}{2}+\frac{x^3}{2}+O(x^4).
$$

Counting the constant term, the first three nonzero terms are $\boxed{1+x+x^2/2}$. If the phrase is taken to mean the first three nonconstant terms, they are $x+x^2/2+x^3/2$; the displayed expansion supplies both conventions. The cubic coefficient is $1/3+1/6=1/2$, combining the cubic term in $\tan x$ with the cubic exponential term.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2015](../../2015-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)

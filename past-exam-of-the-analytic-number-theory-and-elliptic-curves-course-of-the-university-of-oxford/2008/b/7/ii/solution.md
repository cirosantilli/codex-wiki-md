<h1 id="b/7/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For [rank-one two-isogeny descent with parameters three and minus three](../../../../../rank-one-two-isogeny-descent-with-parameters-three-and-minus-three.md), use the standard [two-isogeny rank formula](../../../../../square-class-index-formula-for-two-isogeny-descent.md). For $C:y^2=x(x^2+ax+b)$ and its dual curve $D:y^2=x(x^2-2ax+a^2-4b)$, let $\alpha_C,\alpha_D$ be the abscissa [square-class](../../../../../square-class.md) maps, with their usual values at $(0,0)$ and the identity. If $r_C$ is the [Mordell–Weil rank](../../../../../rank-of-an-elliptic-curve.md), then

$$
\boxed{2^{r_C+2}=|\operatorname{im}\alpha_C|\,|\operatorname{im}\alpha_D|.}
$$

For the present curve $a=3,b=-3$, its possible classes are $1,-1,3,-3$, and the identity and $(0,0)$ supply $1,-3$. Exclude the class three as follows. A point in that class has $x=3(U/V)^2$, with coprime [integers](../../../../../integer-split.md) $U,V$, and substitution in the curve gives the necessary quartic equation

$$
N^2=3U^4+3U^2V^2-V^4
$$

with [integer](../../../../../integer-split.md) $N$. Modulo three this forces $3\mid V,N$. Coprimality then makes $U$ a [unit](../../../../../unit-in-a-ring.md) modulo three, and modulo nine the right side is $3U^4\equiv3$, while $N^2\equiv0$, a contradiction. The class minus one is excluded as well, since multiplying it by the known class minus three would give three. Therefore the first image has size two.

The dual curve is $D:y^2=x(x^2-6x+21)$. Its quadratic factor is $(x-3)^2+12>0$ on the [real line](../../../../../real-line.md), so every nonzero rational abscissa is positive. By (i) its image is contained in $\{1,3,7,21\}$. The point $(0,0)$ supplies 21 and the point $(3,6)$ supplies three. As the [square-class](../../../../../square-class.md) map is a homomorphism, their product supplies seven. All four occur. Hence the descent formula gives $2^{r_C+2}=2\cdot4=8$, so

$$
\boxed{\operatorname{rank}C(\mathbb Q)=1.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

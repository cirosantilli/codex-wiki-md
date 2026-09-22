<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Introduce [slack variables](../../../../../slack-variable.md) $s_1,s_2,s_3$. The initial [simplex dictionary](../../../../../simplex-dictionary.md) is

$$
s_1=5-x_1,\qquad
s_2=25-4x_1-x_2,\qquad
s_3=125-8x_1-4x_2-x_3,\qquad
z=4x_1+2x_2+x_3.
$$

All six variables are nonnegative. The given rule is the [Dantzig pivot rule](../../../../../dantzig-pivot-rule.md): select the [nonbasic variable](../../../../../nonbasic-variable.md) with the largest positive [reduced cost](../../../../../reduced-cost.md). It applies to [slack variables](../../../../../slack-variable.md) too once they become nonbasic. At each step the [simplex ratio test](../../../../../simplex-ratio-test.md) limits how far that entering variable can increase before a [basic variable](../../../../../basic-variable.md) reaches zero.

The successive objective rows of the [simplex dictionary](../../../../../simplex-dictionary.md), expressed in the current [nonbasic variables](../../../../../nonbasic-variable.md), are

$$
\begin{aligned}
z&=4x_1+2x_2+x_3,\\
z&=20-4s_1+2x_2+x_3,\\
z&=30+4s_1-2s_2+x_3,\\
z&=50-4x_1-2s_2+x_3,\\
z&=75+4x_1+2s_2-s_3,\\
z&=95-4s_1+2s_2-s_3,\\
z&=105+4s_1-2x_2-s_3,\\
z&=125-4x_1-2x_2-s_3.
\end{aligned}
$$

These rows identify each entering variable unambiguously. Performing the corresponding [simplex ratio tests](../../../../../simplex-ratio-test.md) gives the complete pivot sequence:

$$
\begin{array}{c|c|c|r|c|r}
\text{pivot}&\text{enter}&\text{leave}&\text{step}&(x_1,x_2,x_3)&z\\ \hline
1&x_1&s_1&5&(5,0,0)&20\\
2&x_2&s_2&5&(5,5,0)&30\\
3&s_1&x_1&5&(0,25,0)&50\\
4&x_3&s_3&25&(0,25,25)&75\\
5&x_1&s_1&5&(5,5,65)&95\\
6&s_2&x_2&5&(5,0,85)&105\\
7&s_1&x_1&5&(0,0,125)&125
\end{array}
$$

For example, after pivot two the dictionary has $x_1=5-s_1$, $x_2=5+4s_1-s_2$ and $s_3=65-8s_1+4s_2-x_3$. Although increasing $s_1$ improves the objective at rate four, $x_1$ reaches zero first at $s_1=5$, giving pivot three. After pivot four, $x_2=25-4x_1-s_2$ and $x_3=25+8x_1+4s_2-s_3$; the [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md) $x_1\leq5$ gives pivot five.

In the final objective row every [reduced cost](../../../../../reduced-cost.md) is nonpositive. Since $x_1,x_2,s_3\geq0$, it also directly certifies the [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md) $z\leq125$, attained only when all three vanish. Thus

$$
\boxed{x^*=(0,0,125),\qquad z^*=125,\qquad\text{seven pivots}.}
$$

A [greatest improvement pivot rule](../../../../../greatest-improvement-pivot-rule.md) uses the total feasible increase in the objective, rather than its increase per unit of the entering variable. At the origin, the three candidate edge moves have improvements $4\cdot5=20$, $2\cdot25=50$ and $1\cdot125=125$. It therefore brings $x_3$ into the [simplex basis](../../../../../simplex-basis.md) first, with $s_3$ leaving, and immediately reaches the optimum. **This rule solves this instance in one pivot.**

This is a three-dimensional [Klee-Minty cube](../../../../../klee-minty-cube.md) example: the specified [Dantzig pivot rule](../../../../../dantzig-pivot-rule.md) visits every vertex before reaching the optimum. Higher-dimensional versions require $2^d-1$ pivots, so that rule has exponential worst-case running time despite its strong practical performance. Each pivot requires only polynomially many arithmetic operations. An anti-cycling rule such as the [Bland pivoting rule](../../../../../bland-pivoting-rule.md) ensures finite termination; without one, degenerate pivots can cycle. A crude terminating bound is the number of possible bases, $\binom{m+n}{m}$ for $m$ constraints and $n$ original variables, which can be exponential. This does not show that every conceivable pivot rule must take exponential time. [Linear programming](../../../../../linear-programming.md) itself has [polynomial-time algorithms](../../../../../polynomial-time-algorithm.md), including the [ellipsoid method](../../../../../ellipsoid-method.md) and suitable [interior-point methods](../../../../../interior-point-method.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

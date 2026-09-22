<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

Fix any starting village and let $A$ be the pickup distance, $B$ the subsequent passenger distance. From each vertex, the four possible pickup distances are $0,5,10,15$, each with [probability](../../../../../probability.md) $1/4$. From each pickup village, the three other possible destinations have distances $5,10,15$, each with [probability](../../../../../probability.md) $1/3$.

Sharing the pickup village does not by itself give [independence](../../../../../independent-random-variables.md). Here it does hold because the [conditional distribution](../../../../../conditional-distribution.md) of $B$ is the same for every pickup village: for all allowed $a,b$,

$$
P(A=a,B=b)=\sum_{u:\,d(\text{start},u)=a}P(U=u)P(B=b\mid U=u)
=P(A=a)\frac13=P(A=a)P(B=b).
$$

Thus $D=A+B$ has the [taxi distance convolution on a rectangular road cycle](../../../../../taxi-distance-convolution-on-a-rectangular-road-cycle.md). Counting the twelve equally likely pairs gives

$$
\boxed{\begin{array}{c|rrrrrr}
d\text{ (miles)}&5&10&15&20&25&30\\\hline
P(D=d)&1/12&2/12&3/12&3/12&2/12&1/12
\end{array}}
$$

No other distances are possible. The [probability distribution](../../../../../probability-distribution.md) is the same for every starting village, so no assumption about the previous customer's destination is needed.

The separate moments are $\mathbb EA=15/2$, $\mathbb EB=10$, $\operatorname{Var}A=125/4$ and $\operatorname{Var}B=50/3$. [Independence](../../../../../independent-random-variables.md) therefore gives

$$
\boxed{\mathbb ED=\frac{35}{2}\text{ miles},\qquad
\operatorname{Var}D=\frac{125}{4}+\frac{50}{3}=\frac{575}{12}\text{ miles}^2.}
$$

As a check from the displayed [probability mass function](../../../../../probability-mass-function.md), $\mathbb ED^2=2125/6$ and subtracting $(35/2)^2$ gives the same [variance](../../../../../variance-split.md).

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

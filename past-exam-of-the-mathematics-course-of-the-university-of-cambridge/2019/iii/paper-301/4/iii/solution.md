<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For [Phi-six theory](../../../../../../phi-six-theory.md), let $D_0=D_F(0)$ and $D_{xy}=D_F(x-y)$. The [Dyson series](../../../../../../dyson-series.md) gives

$$
Z[0]=\langle0|T\{S\}|0\rangle
=1-\frac{i\lambda}{6!}\int d^4x\,\langle\phi(x)^6\rangle_0
+\frac{(-i\lambda)^2}{2(6!)^2}\int d^4x\,d^4y\,
\langle\phi(x)^6\phi(y)^6\rangle_0+O(\lambda^3).
$$

At one vertex, [Wick theorem](../../../../../../wick-s-theorem.md) supplies $5!!=15$ pairings. At two vertices let $r$ be the number of propagators joining them. It must be $0,2,4,$ or $6$, and the number of contractions is

$$
N_r=\binom6r^2r!\bigl((5-r)!!\bigr)^2,
\qquad
(N_0,N_2,N_4,N_6)=(225,4050,5400,720).
$$

Therefore

$$
\boxed{
\begin{aligned}
Z[0]={}&1-\frac{i\lambda}{48}\int d^4x\,D_0^3\\
&+(-i\lambda)^2\int d^4x\,d^4y\left[
\frac{D_0^6}{4608}
+\frac{D_0^4D_{xy}^2}{256}
+\frac{D_0^2D_{xy}^4}{192}
+\frac{D_{xy}^6}{1440}
\right]+O(\lambda^3).
\end{aligned}}
$$

The four [Vacuum Feynman diagram](../../../../../../vacuum-feynman-diagram.md) types are shown below. The $r=0$ term is two disconnected copies of the order-$\lambda$ three-tadpole graph; the other three are connected.

<a id="4/iii/image-vacuum-diagrams-in-phi-six-theory-through-second-order"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-301-vacuum-bubbles.png)

**[Figure 3](#4/iii/image-vacuum-diagrams-in-phi-six-theory-through-second-order). Vacuum diagrams in phi-six theory through second order**. At first order one six-valent vertex is paired into three tadpoles. At second order the two vertices can have two, four, or six connecting propagators, with the remaining legs paired into tadpoles.

Define

$$
B_1=-\frac{i\lambda}{48}\int d^4x\,D_0^3
$$

and let $B_2$ be the sum of the $r=2,4,6$ terms in the second line. The disconnected $r=0$ contribution is exactly $B_1^2/2$. Hence

$$
\boxed{Z[0]=\exp\{B_1+B_2+O(\lambda^3)\},}
$$

which is the [linked-cluster theorem](../../../../../../linked-cluster-theorem.md): the logarithm of the vacuum amplitude is the sum of connected vacuum bubbles.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

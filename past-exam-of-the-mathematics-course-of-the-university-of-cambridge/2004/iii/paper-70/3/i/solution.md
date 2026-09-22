<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let the original abscissae be $x_i=ih$ and vary only the ordinate of vertex $i$. Under [Chaikin subdivision](../../../../../../chaikin-subdivision.md), the two child values on an edge are $\tfrac34y_j+\tfrac14y_{j+1}$ and $\tfrac14y_j+\tfrac34y_{j+1}$. All influence weights are nonnegative, so no cancellation removes an active descendant.

At level $r$ the spacing is $h_r=h/2^r$. If the leftmost influenced vertex is at $a_r$, the next leftmost is the quarter point on the preceding edge, $a_{r+1}=a_r-3h_r/4$; the rightmost advances by the same amount. Starting at $x_i$, the influenced vertex range is therefore

$$
\left[x_i-\frac{3h}{4}\sum_{j=0}^{r-1}2^{-j},\ x_i+\frac{3h}{4}\sum_{j=0}^{r-1}2^{-j}\right].
$$

The neighboring zero vertices bound any extra affected polygon segments by one refined spacing, which tends to zero. Passing to the limit gives

$$
\boxed{\operatorname{supp}\text{ influence}=[x_i-3h/2,\ x_i+3h/2].}
$$

It spans three original grid intervals, with its endpoints at original edge centers. Positive descendant weights occur arbitrarily close to each endpoint, so this is the exact support closure. The [support of a stationary subdivision scheme](../../../../../../support-of-a-stationary-subdivision-scheme.md) concerns the limit curve, not only the first pair of adjacent original edges. This describes interior vertices or an infinite uniform sequence; a finite open polygon needs an endpoint convention.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

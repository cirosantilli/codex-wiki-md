<h1 id="28i/solution">Solution</h1>

↑ **Parent:** [28I](../28i.md)

Put $\beta=2/3$. The [Bellman equation](../../../../../bellman-equation.md) is $F(x)=\inf_u\{x^2+u^2+\beta\mathbb EF(x+u+\epsilon)\}$. For the quadratic candidate $G(x)=Px^2+d$, the quantity minimized is

$$
x^2+u^2+\beta P[(x+u)^2+1]+\beta d.
$$

For $P\ge0$, completing the square gives $u_*=-\beta P x/(1+\beta P)$. Matching the $x^2$ and constant terms requires

$$
P=1+\frac{\beta P}{1+\beta P},\qquad d=\beta(P+d).
$$

The first equation is $2P^2-P-3=0$. Its admissible nonnegative root is $P=3/2$, and $d=3$. Hence $\boxed{G(x)=\tfrac32x^2+3,\quad u_t=-x_t/2}$.

A suitable discounted verification theorem is: if a nonnegative candidate satisfies the [Bellman equation](../../../../../bellman-equation.md), a stationary minimizing selector has finite cost and its discounted expected terminal candidate tends to zero, and the same terminal limit holds for every finite-cost competing policy, then that selector is optimal and the candidate is the value function. Iterating the Bellman inequality proves the lower bound for each competing cost; iterating equality along the selector proves attainment. Here finite cost implies $\sum_t\beta^t\mathbb Ex_t^2<\infty$, so $\beta^t\mathbb EG(x_t)\to0$. Under the selector $x_{t+1}=x_t/2+\epsilon_t$, the second moments are bounded by a geometric recursion, giving finite cost and the same terminal limit. Thus $F=G$. Infinite-cost policies cannot improve the value.

For $\lambda=0$, the two coordinates decouple and have the same discount, so $\boxed{u_t=-x_t/2,\quad w_t=-y_t/2}$. The total value is $(3/2)(x^2+y^2)+6$.

For $\lambda=1$, the discount is $\beta=3/4$ and the state cost is $(x+y)^2$. Introduce the [orthogonal transformation](../../../../../orthogonal-transformation.md) $s=(x+y)/\sqrt2$, $q=(x-y)/\sqrt2$, with controls $v=(u+w)/\sqrt2$, $z=(u-w)/\sqrt2$. The cost becomes $2s^2+v^2+z^2$. Each transformed noise has mean zero and variance one; they need not be independent unless the original noises are Gaussian, and no such independence is needed here. The unpenalized difference coordinate has optimal control $z=0$. For the sum coordinate, the quadratic coefficient solves

$$
P=2+\frac{(3/4)P}{1+(3/4)P},\qquad 3P^2-5P-8=0,
$$

so $P=8/3$, $v=-2s/3$, and the constant is $d=\beta P/(1-\beta)=8$. Therefore

$$
\boxed{u_t=w_t=-\frac{x_t+y_t}{3},\qquad V(x,y)=\frac43(x+y)^2+8.}
$$

The sum state is mean-square stable under this feedback; the uncontrolled difference state may wander, but its value function and state cost are both zero. The same verification argument applies to the penalized sum coordinate.

## ↑ Ancestors (10)

1. [28I](../28i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

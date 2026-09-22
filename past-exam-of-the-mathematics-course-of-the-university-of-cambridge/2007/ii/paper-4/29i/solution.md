<h1 id="29i/solution">Solution</h1>

↑ **Parent:** [29I](../29i.md)

Let $P=\mathbb E\Delta_n^2$ in equilibrium, with $\Delta_n=X_n-\widehat X_n$. The innovation is $Z_{n+1}=Y_{n+1}-\widehat X_n=\Delta_n+\eta_{n+1}$. The given filter gives

$$
\Delta_{n+1}=(1-H)\Delta_n+\varepsilon_{n+1}-H\eta_{n+1}.
$$

Orthogonality to the new innovation requires $(1-H)P-H=0$, hence $H=P/(P+1)$. Since the variables are jointly Gaussian, this orthogonality is independence. Stationary variance gives $P=(1-H)^2P+1+H^2=P/(P+1)+1$, so

$$
P^2-P-1=0,\qquad P=(1+\sqrt5)/2,
\qquad \boxed{H=(\sqrt5-1)/2.}
$$

The added process noise reflects the fact that the new observation concerns $X_n$, not $X_{n+1}$.

For the control calculation choose a quadratic value coefficient $R>0$. Conditional minimization of $x^2+u^2+R\mathbb E[(x+u+\varepsilon)^2]$ gives $K=R/(1+R)$ and the Riccati equation $R=1+R-R^2/(1+R)$, hence $R^2=R+1$. Separation replaces $x$ by its conditional estimate, giving

$$
\boxed{K=R/(1+R)=H=(\sqrt5-1)/2.}
$$

To determine the average cost without solving an additional state covariance, complete the square:

$$
x^2+u^2+R\mathbb E[X_{n+1}^2-x^2\mid x,u]
=R+(1+R)(u+Kx)^2.
$$

With $u=-K\widehat X_n$, the final square is $K^2\Delta_n^2$. In equilibrium the expected telescoping value term is zero, so the minimal cost is

$$
\boxed{\bar J=R+(1+R)K^2P=1+\sqrt5.}
$$

The identity also proves optimality: conditional mean minimization of the square uniquely selects the stated control. Here $1-K\in(0,1)$ ensures stable closed-loop estimates, making the equilibrium averaging valid. This is the [Scalar delayed-observation LQG regulator](../../../../../scalar-delayed-observation-lqg-regulator.md).

## ↑ Ancestors (10)

1. [29I](../29i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

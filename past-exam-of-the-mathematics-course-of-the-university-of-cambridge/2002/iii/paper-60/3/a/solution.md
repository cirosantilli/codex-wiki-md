<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $e$ be the vector of ones. For a general nonautonomous [Runge-Kutta method](../../../../../../runge-kutta-method.md) the stages satisfy $k_i=f(t+c_ih,y+h\sum_ja_{ij}k_j)$ and the update is $Y=y+h\sum_ib_ik_i$. Expansion at $(t,y)$ gives

$$
k_i=f+h\{c_if_t+(Ae)_if_yf\}+O(h^2),
$$

and therefore

$$
Y=y+h(b^Te)f+h^2\{(b^Tc)f_t+(b^TAe)f_yf\}+O(h^3).
$$

The exact solution is $y(t+h)=y+hf+h^2(f_t+f_yf)/2+O(h^3)$. Matching the independent terms gives the necessary and sufficient [second-order conditions with independent Runge-Kutta abscissae](../../../../../../second-order-conditions-with-independent-runge-kutta-abscissae.md)

$$
\boxed{b^Te=1,\qquad b^Tc=\tfrac12,\qquad b^TAe=\tfrac12.}
$$

Under the usual internally consistent [Butcher tableau](../../../../../../butcher-tableau.md) convention $c=Ae$, this reduces to $c=Ae$, $b^Te=1$, $b^Tc=1/2$. If the abscissae are allowed to be independent of the row sums, $c=Ae$ is a sufficient simplifying convention rather than a logically necessary order-two condition.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

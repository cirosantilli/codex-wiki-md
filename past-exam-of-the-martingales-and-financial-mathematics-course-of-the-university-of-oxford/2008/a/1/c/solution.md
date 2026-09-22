<h1 id="a/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Both stopped variables are integrable, since $|X_S|,|X_T|\leq\sum_{j=0}^N|X_j|$. Also $X_S$ is $\mathcal F_S$-measurable: intersecting $\{X_S\in B\}$ with $\{S\leq n\}$ gives the finite union $\bigcup_{j\leq\min(n,N)}\{S=j,X_j\in B\}$ in $\mathcal F_n$ for each Borel $B$.

The increment identity is

$$
X_T-X_S=\sum_{k=0}^{N-1}(X_{k+1}-X_k)1_{\{S\leq k<T\}}.
$$

For $A\in\mathcal F_S$, the event $A\cap\{S\leq k\}\cap\{T>k\}$ belongs to $\mathcal F_k$. The [martingale](../../../../../martingale-split.md) increment has conditional mean zero given that sigma-algebra. Multiplying by its indicator and using the [tower property](../../../../../law-of-total-expectation.md) gives zero expectation for each summand. Therefore

$$
\mathbb E[1_A(X_T-X_S)]=0\qquad(A\in\mathcal F_S).
$$

Together with measurability and integrability, this is the defining property of [conditional expectation](../../../../../conditional-expectation.md), proving the bounded [optional sampling theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md)

$$
\boxed{\mathbb E(X_T\mid\mathcal F_S)=X_S\quad\text{almost surely}.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

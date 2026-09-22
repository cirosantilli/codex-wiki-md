<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Direct integration of the [uniform distribution](../../../../../continuous-uniform-distribution.md) yields $\mathbb E U_j=b/2$ and $\mathbb E U_j^2=b^2/3$. The [expectation of a product of independent random variables](../../../../../expectation-of-a-product-of-independent-random-variables.md) gives

$$
\mathbb EW_n=\prod_{j=1}^n\mathbb E U_j=(b/2)^n,\qquad \mathbb EW_n^2=(b^2/3)^n.
$$

Subtracting the square of the [expected value](../../../../../expected-value-split.md) gives the [variance](../../../../../variance-split.md):

$$
\boxed{\mathbb EW_n=(b/2)^n,\qquad\operatorname{Var}(W_n)=(b^2/3)^n-(b^2/4)^n.}
$$

Since $W_n\geq0$, [Markov's inequality](../../../../../markov-s-inequality.md) implies, for every $\varepsilon>0$,

$$
\mathbb P(W_n>\varepsilon)\leq\frac{(b/2)^n}{\varepsilon}\longrightarrow0\quad(0<b<2).
$$

Hence $\boxed{W_n\to0\text{ in probability for }0<b<2.}$ The first [moment](../../../../../moment.md) suffices: the [variance](../../../../../variance-split.md) need not tend to zero throughout this range.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

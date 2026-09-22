<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [infinite occupation time of one-dimensional Brownian motion](../../../../../../infinite-occupation-time-of-one-dimensional-brownian-motion.md) implies

$$
A_\infty=\int_0^\infty\frac{ds}{1+B_s^2}\geq\frac12\int_0^\infty\mathbf1_{\{|B_s|\leq1\}}ds=\infty\quad\text{almost surely}.
$$

For a start $x\ne0$, first wait until $B$ hits zero, which happens in finite time by [recurrence of one-dimensional Brownian motion](../../../../../../recurrence-of-one-dimensional-brownian-motion.md), and apply the [Strong Markov property](../../../../../../strong-markov-property.md). The repeated exit-and-return argument in Question 4(c) then proves the infinite occupation integral. Since $f\geq C>0$, the [Feynman-Kac formula](../../../../../../feynman-kac-formula.md) gives $u(t,x)\geq C\mathbb E_x e^{A_t}$. The random variables $e^{A_t}$ increase to infinity [almost surely](../../../../../../almost-sure-convergence.md); the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) therefore yields the intended [positive-potential growth from Brownian recurrence](../../../../../../positive-potential-growth-from-brownian-recurrence.md):

$$
\boxed{\lim_{t\to\infty}u(t,x)=+\infty\quad\text{for every fixed }x\in\mathbb R.}
$$

**Under global boundedness, no such solution exists when the initial function is bounded below by a positive constant.** The PDF prints $C_b^{1,2}(\mathbb R_+\times\mathbb R)$; if the subscript means bounded over the whole product, its hypotheses with $f\geq C>0$ are incompatible, rather than an example of growth within that class. The precise correction is to require $u$ and its indicated derivatives to be bounded on $[0,T]\times\mathbb R$ for every finite $T$. The derivation above then gives the requested limit. Already $f\equiv1$ satisfies the printed initial-data assumption but cannot have a globally bounded [classical solution](../../../../../../classical-solution.md), by this formula. Also the PDF's $u(x,t)$ in this clause reverses the argument order from $u(t,x)$ used in the equation; the limit above keeps the equation's time-first convention.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

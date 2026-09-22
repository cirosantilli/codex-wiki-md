<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

Substitution of the [power series](../../../../../power-series.md), with termwise [differentiation](../../../../../differentiation.md), gives the coefficient identity

$$
-(n+2)(n+1)a_{n+2}+2na_n=Ea_n,
\qquad a_{n+2}=\frac{2n-E}{(n+2)(n+1)}a_n.
$$

Thus $a_0$ and $a_1$ are arbitrary, and all [power series](../../../../../power-series.md) solutions of the [Hermite differential equation](../../../../../hermite-differential-equation.md) are

$$
\boxed{W(x)=a_0\sum_{j=0}^\infty\frac{\prod_{r=0}^{j-1}(4r-E)}{(2j)!}x^{2j}
+a_1\sum_{j=0}^\infty\frac{\prod_{r=0}^{j-1}(4r+2-E)}{(2j+1)!}x^{2j+1}.}
$$

An empty product is one. For a nonterminating branch the ratio of consecutive terms in its own parity subsequence is asymptotic to $|x|^2/j$, hence tends to zero for every fixed $x$. The [ratio test](../../../../../ratio-test.md) proves convergence everywhere; the resulting [power series](../../../../../power-series.md) can be differentiated termwise and indeed solve the [differential equation](../../../../../differential-equation-split.md). A terminating branch is already a [polynomial](../../../../../polynomial-split.md).

The [boundary condition](../../../../../boundary-condition.md) $W(0)=0$ forces $a_0=0$; the solution is odd. Apart from the zero solution, which works for every $E$, a [polynomial](../../../../../polynomial-split.md) occurs exactly when an odd index $d$ satisfies $2d-E=0$. Before that index the odd coefficients are nonzero, and after it they vanish. Thus the [odd polynomial solutions of the Hermite differential equation](../../../../../odd-polynomial-solutions-of-the-hermite-differential-equation.md) have

$$
\boxed{E=4j+2,\quad \deg W=2j+1,\quad j=0,1,2,\ldots.}
$$

Equivalently, comparison of leading [polynomial](../../../../../polynomial-split.md) coefficients gives $E=2\deg W$, proving that no other nonzero polynomial is possible. Normalizing by $a_1=1$, the [polynomials](../../../../../polynomial-split.md) of degree below six are

$$
\begin{array}{c|c}
E&W(x)\\\hline
2&x\\
6&x-\frac23x^3\\
10&x-\frac43x^3+\frac4{15}x^5.
\end{array}
$$

Each can be multiplied by an arbitrary nonzero constant; these are normalized odd [Hermite polynomials](../../../../../hermite-polynomial.md).

Let $L=-d^2/dx^2+2x\,d/dx$. The forcing in the final [inhomogeneous linear differential equation](../../../../../inhomogeneous-linear-differential-equation.md) is precisely the displayed degree-five [eigenfunction](../../../../../eigenfunction.md) $P_5$, with $LP_5=10P_5$. Hence

$$
\boxed{W(x)=\frac1{10}P_5(x)=\frac{x}{10}-\frac{2x^3}{15}+\frac{2x^5}{75}.}
$$

Direct [differentiation](../../../../../differentiation.md) gives $LW=x-4x^3/3+4x^5/15$, and $W(0)=0$. Among [polynomial](../../../../../polynomial-split.md) solutions this choice is unique: a polynomial in the [kernel](../../../../../kernel-of-a-linear-map.md) of $L$ must be constant, and its value at zero eliminates that constant.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

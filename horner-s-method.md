<h1 id="horner-s-method">Horner's method</h1>

↑ **Parent:** [Polynomial](polynomial-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Horner's_method)

[Horner's method](horner-s-method.md) evaluates a [polynomial](polynomial-split.md) by nested multiplication, requiring one multiplication and one addition per degree after initialization.

For $p(X)=a_nX^n+\cdots+a_0$, start with $b_n=a_n$ and compute $b_j=xb_{j+1}+a_j$ for $j=n-1,\ldots,0$. The final value is $b_0=p(x)$. Equivalently,

$$
p(x)=a_0+x\bigl(a_1+x\bigl(a_2+\cdots+xa_n\bigr)\bigr).
$$

This reorganization reuses intermediate results, avoiding separate computation of every power. A dense degree-$n$ [polynomial](polynomial-split.md) takes $n$ [multiplications](multiplication.md) and $n$ coefficient [additions](addition.md) after reading its [leading coefficient](leading-coefficient-of-a-polynomial.md); special zero coefficients may permit further simplifications.

For our cubic, the coefficient list in descending order is $1,-3,0,4$. The zero is important: it occupies the missing $X$ term's position. At $x=2$, the accumulated values are

$$
1\ \longrightarrow\ 2\cdot1-3=-1\ \longrightarrow\ 2(-1)+0=-2\ \longrightarrow\ 2(-2)+4=0.
$$

At $x=3$, the same operations give $1,0,0,4$, confirming $p(3)=4$.

<a id="image-the-same-nested-arithmetic-evaluates-a-polynomial-and-produces-the-coefficients-for-division-by-a-linear-factor"></a>
![](horner-evaluation-and-division.png)

**[Figure 2](#image-the-same-nested-arithmetic-evaluates-a-polynomial-and-produces-the-coefficients-for-division-by-a-linear-factor). The same nested arithmetic evaluates a polynomial and produces the coefficients for division by a linear factor**.

The intermediate values do more than evaluate. They are the [coefficients](coefficient.md) of the [polynomial quotient](quotient-of-polynomial-division.md) in [polynomial division](polynomial-division.md) by $X-x$, with the final value as the [polynomial remainder](remainder-of-polynomial-division.md). At $x=2$, the first three values give $X^2-X-2$, so

$$
p(X)=(X-2)(X^2-X-2)+0.
$$

At $x=3$, they give $X^2$, so $p(X)=(X-3)X^2+4$. This links an efficient numerical calculation with the exact [factor theorem](factor-theorem.md).

[William George Horner](william-george-horner.md)'s 1819 paper concerns solving numerical [equations](equation.md) by successive approximation. The Royal Society archive records the manuscript and its reading on 1 July 1819; it provides a historical reference for the method's name. [Royal Society archive, Horner's 1819 manuscript](https://makingscience.royalsociety.org/items/pt_13_23/paper-a-new-method-of-solving-numerical-equations-of-all-orders-by-continuous-approximation-by-w-g-william-george-horner)

// Target: geometry-and-topology.bigb

## ↑ Ancestors (5)

1. [Polynomial](polynomial-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Horner's method](horner-s-method.md)
- [Newton polynomial](newton-polynomial.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77/3/ii/solution.md)
- [Polynomial](polynomial-split.md)

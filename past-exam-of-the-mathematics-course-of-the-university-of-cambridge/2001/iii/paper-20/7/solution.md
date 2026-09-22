<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

A [logarithmic form](../../../../../linear-form-in-logarithms-of-algebraic-numbers.md) is $\Lambda=b_1\log\alpha_1+\cdots+b_s\log\alpha_s$ in fixed choices of logarithms of nonzero [algebraic numbers](../../../../../algebraic-number.md), with [integer](../../../../../integer.md) coefficients. The indispensable condition is $\Lambda\ne0$. Put $B\ge\max(e,|b_1|,\ldots,|b_s|)$ and take $A_j\ge\max(Dh(\alpha_j),|\log\alpha_j|,1)$ for a [number field](../../../../../number-field.md) of degree $D$ containing the arguments. A typical effective estimate is

$$
\log|\Lambda|>-C(s,D)(1+\log B)\prod_j A_j,
$$

with an explicitly computable constant. For fixed arguments this is a power-type lower bound $|\Lambda|>B^{-C}$. It is fundamentally stronger for applications than a crude norm estimate exponential in $B$.

The basic estimates follow the auxiliary-function pattern already used here, in a multivariable form. Choose a [polynomial](../../../../../polynomial-split.md) or an interpolation determinant in powers of the algebraic arguments; impose many derivative or interpolation conditions by [Siegel lemma](../../../../../siegel-s-lemma.md). Analytic extrapolation near the chosen logarithms makes the determinant tiny. Arithmetic denominator and norm estimates prevent a nonzero algebraic determinant from being so small, while a [multiplicity](../../../../../multiplicity-mathematics.md) or zero estimate ensures the necessary determinant does not vanish identically. Balancing the degree, [multiplicity](../../../../../multiplicity-mathematics.md) and [arithmetic height](../../../../../height-function.md) parameters produces dependence on the individual $A_j$ and only logarithmic dependence on $B$. The nonvanishing argument and the arithmetic [arithmetic height](../../../../../height-function.md) control are both necessary parts of this outline.

For practical equations the output is a finite, certified computation. Factor the equation in a [number field](../../../../../number-field.md), record the finitely many [ideal](../../../../../ideal.md) and torsion possibilities, and express its factors in [fundamental units](../../../../../fundamental-unit-number-theory.md). At a place where the original equation gives an exponentially small remainder, choose the principal logarithm and include a multiple of $2\pi i$ for the branch. Compare that upper bound with the effective lower bound to obtain an initial exponent bound. Question 5 shows this for a [unit](../../../../../unit-in-a-ring.md) equation, and Question 6 shows why a rational argument of variable [arithmetic height](../../../../../height-function.md) can still bound a common power exponent. Zero forms and degenerate families are separated before any estimate is applied.

A concrete two-logarithm example is $2^u-3^v=1$, with positive exponents. Here

$$
0<u\log2-v\log3=\log(1+3^{-v})<3^{-v}.
$$

The lower bound and $u=v\log3/\log2+O(1)$ give an effective upper bound for $u,v$. The exponents are [coprime](../../../../../coprime-integers.md): a common [divisor](../../../../../divisor.md) greater than one would factor a difference of two positive [integer](../../../../../integer.md) powers equal to $1$, which is impossible. For large $v$ the same upper estimate makes $u/v$ a continued-fraction convergent of $\log3/\log2$, since its error is smaller than $1/(2v^2)$. One checks only the finitely many convergents up to the proven bound, with small cases checked directly. Higher-dimensional problems use the [LLL algorithm](../../../../../lenstra-lenstra-lovasz-lattice-basis-reduction-algorithm.md) to obtain analogous improvements from the first large bound.

Every numerical logarithm must be evaluated with a certified error interval, so that a proposed reduction really is an inequality and an exact [integer](../../../../../integer.md) check can certify each surviving candidate. [Continued fractions](../../../../../continued-fraction.md) or lattice reduction accelerate the search; the prior effective upper bound is what makes the search complete. This explains how [linear forms in logarithms of algebraic numbers](../../../../../linear-form-in-logarithms-of-algebraic-numbers.md) turn qualitative finiteness into practical Diophantine algorithms, while also outlining the auxiliary machinery behind the estimates.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The first coefficient is the [posterior mean](../../../../../../posterior-mean.md) log odds of choosing invertebrates rather than fish for smaller alligators at Lake Hancock. It corresponds to

$$
\boxed{\exp(-1.852)\approx0.157}
$$

for those invertebrate-to-fish odds. This is not the absolute probability of choosing the second category, because the other categories also enter the normalization.

The size coefficient adds $-1.524$ to the invertebrate-to-fish log odds on changing to the larger class, holding lake fixed. Its common-across-lakes [odds ratio](../../../../../../odds-ratio.md) is

$$
\boxed{\exp(-1.524)\approx0.218,}
$$

about a 78 percent reduction in the relative odds. Exponentiating a [posterior mean](../../../../../../posterior-mean.md) log odds is a geometric summary, not the arithmetic [posterior mean](../../../../../../posterior-mean.md) of the odds.

There are $(K-1)p=4\cdot5=20$ free category coefficients plus $I=8$ group intercepts, giving **28 free parameters in the fitted Poisson model**. The [effective parameter count in DIC](../../../../../../effective-parameter-count-in-dic.md), $26.8$, is close to 28 and slightly smaller, consistent with some regularization or incomplete information. Comparing it with 20 would omit the nuisance intercepts. A direct conditional multinomial fit has 20 coefficients but a different observational likelihood, since it conditions on the totals.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

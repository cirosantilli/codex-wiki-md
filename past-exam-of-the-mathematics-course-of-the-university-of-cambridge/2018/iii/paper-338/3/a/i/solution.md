<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First include the mean-gain calculation preceding the numbered clauses. At each [electron-multiplying CCD](../../../../../../../electron-multiplying-ccd.md) stage one electron contributes an expected $1+p$ electrons to the next stage. If $N_j$ is the charge after stage $j$, [conditional expectation](../../../../../../../conditional-expectation.md) gives $\mathbb E[N_{j+1}\mid N_j]=(1+p)N_j$. Iteration from $n$ input electrons yields

$$
\boxed{g=(1+p)^r,\qquad \mathbb E[x_n]=ng.}
$$

For small $p$, $g\simeq e^{rp}$ if corrections of order $rp^2$ are negligible.

In the high-gain approximation the output from one input electron has an [exponential distribution](../../../../../../../exponential-distribution.md) of scale $g$. Independent input electrons produce independent cascades, and their charges add. By [convolution of independent random variables](../../../../../../../convolution-of-independent-random-variables.md), assuming the formula for $n$ inputs,

$$
P_{n+1}(x)=\int_0^x P_n(y)P_1(x-y)\,dy
=\frac{e^{-x/g}}{g^{n+1}(n-1)!}\int_0^x y^{n-1}\,dy
=\frac{x^ne^{-x/g}}{g^{n+1}n!}.
$$

Together with the single-electron base case this proves

$$
\boxed{P_n(x)=\frac{x^{n-1}e^{-x/g}}{g^n(n-1)!},\qquad x\geq0,\ n\geq1.}
$$

It is a [gamma distribution](../../../../../../../gamma-distribution.md) with shape $n$ and scale $g$, so it is normalized and has [expected value](../../../../../../../expected-value.md) $ng$ and [variance](../../../../../../../variance-split.md) $ng^2$. The formula is a continuous approximation to discrete output charge, not an exact integer-valued branching distribution; for $n=0$ there is a point mass at zero instead.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 338](../../../../paper-338-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

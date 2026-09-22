<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The squares in the [finite field](../../../../../../finite-field.md) $\mathbb F_7$ are $0,1,2,4$. For $x=0,1,\ldots,6$, the values of $x^3-x+1$ and the numbers of possible $y$ are respectively

$$
\begin{array}{c|rrrrrrr}
x&0&1&2&3&4&5&6\\\hline
x^3-x+1&1&1&0&4&5&2&1\\
\#y&2&2&1&2&0&2&2
\end{array}
$$

Adding $O$ yields **$\#E(\mathbb F_7)=12$**. The [Trace of Frobenius](../../../../../../trace-of-frobenius.md) is $a=8-12=-4$. The [trace of the square of an elliptic-curve endomorphism](../../../../../../trace-of-the-square-of-an-elliptic-curve-endomorphism.md) is $a^2-2q=16-14=2$, so the [elliptic-curve point count over a finite field](../../../../../../elliptic-curve-point-count-over-a-finite-field.md) gives

$$
\boxed{\#E(\mathbb F_{49})=49+1-2=48.}
$$

For example, this trace identity follows from $\pi^2-[a]\pi+[q]=0$ and $\operatorname{tr}[q]=2q$.

One suitable second [elliptic curve](../../../../../../elliptic-curve.md) is

$$
\boxed{E^{\prime}:y^2=x^3+3x+6\quad\text{over }\mathbb F_7.}
$$

Here $4\cdot3^3+27\cdot6^2\equiv2\pmod7$, so its [elliptic-curve discriminant](../../../../../../elliptic-curve-discriminant.md) is nonzero. Its complete list of [rational points](../../../../../../rational-point.md) is $O,(3,0),(6,3),(6,4)$, obtained by checking the seven $x$-values. For $P=(6,3)$ the tangent slope is $1$ in $\mathbb F_7$, and the [elliptic-curve addition formula](../../../../../../elliptic-curve-addition-formula.md) gives $2P=(3,0)$. Consequently $P$ has order four and **$E^{\prime}(\mathbb F_7)\cong\mathbb Z/4\mathbb Z$**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

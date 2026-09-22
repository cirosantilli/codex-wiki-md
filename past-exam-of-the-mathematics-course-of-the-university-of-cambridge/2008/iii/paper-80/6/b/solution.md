<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the ordered [matrix exponential](../../../../../../matrix-exponential.md) product $\Phi(t)=e^{tA}e^{tB}$, differentiation gives

$$
\begin{aligned}
\Phi'(t)-(A+B)\Phi(t)
&=e^{tA}Be^{tB}-Be^{tA}e^{tB}\\
&=[e^{tA},B]e^{tB}.
\end{aligned}
$$

The [matrix commutator](../../../../../../commutator.md) here is $[X,Y]=XY-YX$. Put $E(t)=\Phi(t)-e^{t(A+B)}$. Then $E(0)=0$ and

$$
E'-(A+B)E=[e^{tA},B]e^{tB}.
$$

Multiplying on the left by $e^{-t(A+B)}$ gives an exact product derivative. Integration from zero to $t$, followed by multiplication by $e^{t(A+B)}$, proves the [exponential product defect identity](../../../../../../exponential-product-defect-identity.md):

$$
\boxed{\Phi(t)=e^{t(A+B)}+
\int_0^t e^{(t-x)(A+B)}[e^{xA},B]e^{xB}\,dx.}
$$

No commutation of $A$ and $B$ was assumed. The ordered product is the usual [Lie-Trotter splitting](../../../../../../lie-product-formula.md); the PDF calls this product the Beam-Warming splitting. If $[A,B]=0$, the commutator term vanishes and the product is exact. In general its small-step expansion has local error $t^2[A,B]/2+O(t^3)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

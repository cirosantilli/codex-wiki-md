<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The density axiom and continuity of the [Fourier transform](../../../../../../../fourier-transform.md) at zero imply $|\widehat\varphi(0)|=1$. Here is a proof that avoids assuming a normalization of the integral. Choose a nonzero $f$ whose [Fourier transform](../../../../../../../fourier-transform.md) has bounded support. The [MRA projection Fourier identity](../../../../../../../mra-projection-fourier-identity.md), with no aliasing once $j$ is sufficiently large, is

$$
\|P_jf\|_2^2=\frac1{2\pi}\int_{\mathbb R}|\widehat f(\xi)|^2|\widehat\varphi(2^{-j}\xi)|^2\,d\xi.
$$

Since $\varphi\in L^1$, its [Fourier transform](../../../../../../../fourier-transform.md) is continuous and bounded, so this tends to $|\widehat\varphi(0)|^2\|f\|_2^2$. Density and nesting give $P_jf\to f$ in $L^2$. Thus $|\widehat\varphi(0)|=1$, in particular it is nonzero. Evaluating the [scaling refinement equation](../../../../../../../scaling-refinement-equation.md) in frequency at zero now gives

$$
\widehat\varphi(0)=m(0)\widehat\varphi(0),\qquad \boxed{m(0)=1},
$$

which is stronger than the requested absolute-value equality. Multiplying the [scaling function](../../../../../../../scaling-function.md) by a constant of modulus one normalizes its integral to one without changing $m$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 340](../../../../paper-340-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

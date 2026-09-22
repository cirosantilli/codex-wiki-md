<h1 id="3/d/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $W(s)=a_1\operatorname{Ai}(Z(s))+a_2\operatorname{Bi}(Z(s))$, using the independent [Airy functions](../../../../../../../airy-function.md). To solve $(D^2-1)\widehat v=W$, the [variation of parameters](../../../../../../../variation-of-parameters.md) formula, equivalently a direct convolution, gives the [velocity reconstruction from the Orr-Sommerfeld vorticity](../../../../../../../velocity-reconstruction-from-the-orr-sommerfeld-vorticity.md):

$$
\boxed{\widehat v(y)=C_+e^y+C_-e^{-y}
+\int_{y_0}^y\sinh(y-s)\left[a_1\operatorname{Ai}(Z(s))+a_2\operatorname{Bi}(Z(s))\right]ds.}
$$

The reference point $y_0$ is arbitrary. Twice differentiating the integral produces $W(y)$ because $\sinh0=0$ and its derivative at zero is one, verifying the formula. The four constants are independent: applying $D^2-1$ to an identically zero combination first forces $a_1=a_2=0$, then the complementary solutions force $C_+=C_-=0$. The boundary conditions would be $\widehat v(y_j)=D\widehat v(y_j)=0$, $j=1,2$. Their compatibility selects the eigenvalues; they need not be imposed here.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

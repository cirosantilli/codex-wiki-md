<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [beam splitter](../../../../../../beam-splitter.md) relation and the cavity output equation give

$$
b_0=\beta b_{
m in}-\alpha(\sqrt\gamma\,a+b_0),
\qquad (1+\alpha)b_0=\beta b_{
m in}-\alpha\sqrt\gamma\,a.
$$

For $\alpha\ne-1$, solve this scalar algebraic relation and substitute back:

$$
\boxed{b_0=\frac\beta{1+\alpha}b_{
m in}-\frac{\alpha\sqrt\gamma}{1+\alpha}a,\qquad
b_1=\frac\beta{1+\alpha}b_{
m in}+\frac{\sqrt\gamma}{1+\alpha}a.}
$$

The cavity equation becomes

$$
\boxed{\dot a=\frac{\gamma(\alpha-1)}{2(1+\alpha)}a-\frac{\beta\sqrt\gamma}{1+\alpha}b_{
m in}.}
$$

Finally, use the other beam-splitter output and $\alpha^2+\beta^2=1$:

$$
b_2=\alpha b_{
m in}+\beta b_1
=\left(\alpha+\frac{\beta^2}{1+\alpha}\right)b_{
m in}
+\frac{\beta\sqrt\gamma}{1+\alpha}a
=\boxed{b_{
m in}+\frac{\beta\sqrt\gamma}{1+\alpha}a}.
$$

These derivations retain the printed input $b_{
m in}$ in both beam-splitter equations; the converted TeX changes one of these subscripts. Define $\gamma_{
m eff}=\gamma(1-\alpha)/(1+\alpha)$ and $c=\beta\sqrt\gamma/(1+\alpha)$, so $\dot a=-\gamma_{
m eff}a/2-cb_{
m in}$ and $b_2=b_{
m in}+ca$. In the nondegenerate range $|\alpha|<1$, $\gamma_{
m eff}>0$ and $c^2=\gamma_{
m eff}$, the expected passive input-output relation. This is [instantaneous coherent cavity feedback through a beam splitter](../../../../../../instantaneous-coherent-cavity-feedback-through-a-beam-splitter.md); it uses the zero-delay interconnection assumed by the equations.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

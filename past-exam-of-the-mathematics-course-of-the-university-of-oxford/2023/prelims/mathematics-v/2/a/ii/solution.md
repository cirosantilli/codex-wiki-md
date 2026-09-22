<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An orientation-preserving [reparametrization](../../../../../../../reparametrization.md) has the form $\widetilde\gamma(s)=\gamma(h(s))$, where $h:[\alpha,\beta]\to[a,b]$ is an increasing, piecewise smooth change of parameter with $h(\alpha)=a$, $h(\beta)=b$. For regular parametrizations one may take $h$ and its inverse continuously differentiable on each piece. The [chain rule](../../../../../../../chain-rule.md) gives $\widetilde\gamma'(s)=\gamma'(h(s))h'(s)$. The [change of variables](../../../../../../../change-of-variables-formula.md) $t=h(s)$ therefore yields

$$
\begin{aligned}
\int_\alpha^\beta\mathbf F(\widetilde\gamma(s))\cdot\widetilde\gamma'(s)\,ds
&=\int_\alpha^\beta\mathbf F(\gamma(h(s)))\cdot\gamma'(h(s))h'(s)\,ds\\
&=\int_a^b\mathbf F(\gamma(t))\cdot\gamma'(t)\,dt.
\end{aligned}
$$

This proves [reparametrization invariance of a vector line integral](../../../../../../../reparametrization-invariance-of-a-vector-line-integral.md). If $h$ is decreasing, the endpoints in the final integral are reversed and the sign changes. Thus the same direction and the same multiplicity of traversal are essential.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)

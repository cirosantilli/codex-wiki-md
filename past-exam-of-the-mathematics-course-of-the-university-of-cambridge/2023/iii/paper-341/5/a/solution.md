<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\Phi_h$ be the one-step map of a numerical method. It is a [time-symmetric numerical method](../../../../../../time-symmetric-numerical-method.md) when reversing the step exactly reverses the update:

$$
\boxed{\Phi_{-h}=\Phi_h^{-1},
\quad\text{equivalently}\quad
\Phi_{-h}\circ\Phi_h=I.}
$$

Let $\varphi_h$ be the exact [flow map](../../../../../../flow-map.md) and suppose the method has order $p$ with a nonzero leading [local truncation error](../../../../../../local-truncation-error.md):

$$
\Phi_h(y)=\varphi_h(y)+h^{p+1}d(y)+O(h^{p+2}).
$$

Inverting this expansion changes the sign of its leading perturbation, so

$$
\Phi_h^{-1}(y)=\varphi_{-h}(y)-h^{p+1}\widetilde d(y)+O(h^{p+2}),
$$

where transport by the exact flow only changes $d$ by $O(h)$ and hence does not affect the leading parity. On the other hand, replacing $h$ by $-h$ in the first expansion gives

$$
\Phi_{-h}(y)=\varphi_{-h}(y)+(-1)^{p+1}h^{p+1}\widetilde d(y)+O(h^{p+2}).
$$

Time symmetry equates these expressions, so $(-1)^{p+1}=-1$. Hence $p+1$ is odd and

$$
\boxed{p\text{ is even}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

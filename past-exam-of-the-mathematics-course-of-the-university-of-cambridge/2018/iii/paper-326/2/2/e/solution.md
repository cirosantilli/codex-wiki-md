<h1 id="2/2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Assume $Ku^\dagger=f$, as in the exact-solution setting used for the preceding [source condition for quadratic regularization](../../../../../../../source-condition-for-quadratic-regularization.md). Let $r=r_{k+1}$, $\eta=f^\delta-f$, and $s=u_\delta^{(k+1)}-u_\delta^{(k)}=-\tau K^*r$. Then $K(u_\delta^{(k+1)}-u^\dagger)=r+\eta$, and expanding the two squared errors gives

$$
\begin{aligned}
\|u_\delta^{(k+1)}-u^\dagger\|^2-\|u_\delta^{(k)}-u^\dagger\|^2
&=2\operatorname{Re}\langle s,u_\delta^{(k+1)}-u^\dagger\rangle-\|s\|^2\\
&=-2\tau\operatorname{Re}\langle r,r+\eta\rangle-\|s\|^2\\
&\leq-2\tau\|r\|(\|r\|-\delta)-\|s\|^2.
\end{aligned}
$$

The [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) supplies the last line. Thus while the residual remains at least the noise bound,

$$
\boxed{\|r_{k+1}\|\geq\delta\ \Longrightarrow\
\|u_\delta^{(k+1)}-u^\dagger\|\leq\|u_\delta^{(k)}-u^\dagger\|.}
$$

**Compatibility of the exact data is essential.** If only $f\in\mathcal D(K^\dagger)$ is retained, let $Kx=(x,0)$, $f=(0,1)$, $f^\delta=(1/2,1)$, $\delta=1/2$ and $\tau=1$. The [minimum-norm least-squares solution](../../../../../../../minimum-norm-least-squares-solution.md) is zero, but the first iterate is $1/4$ and its residual [norm](../../../../../../../norm.md) is $\sqrt{17}/4>\delta$. Its error has increased from zero. Thus the original assertion uses the implicit exact-data assumption from part (c), and is false without it.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2](../../../2.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

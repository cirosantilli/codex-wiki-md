<h1 id="b/8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define $f^\sharp(s)=\overline{f(-s)}$. Interchanging the integrals and substituting variables gives

$$
\langle T_fg_1,g_2\rangle=\langle g_1,T_{f^\sharp}g_2\rangle.
$$

Moreover Cauchy-Schwarz in the inner integral gives

$$
\begin{aligned}
|\langle T_fg_1,g_2\rangle|
&\leq\int_{\mathbb R}|f(s)|\left|\int_{\mathbb R}g_1(t-s)\overline{g_2(t)}dt\right|ds\\
&\leq\|f\|_1\|g_1\|_2\|g_2\|_2.
\end{aligned}
$$

Taking the supremum over unit $g_2$ proves $\|T_fg_1\|_2\leq\|f\|_1\|g_1\|_2$, so $T_f$ is bounded with [norm](../../../../../norm.md) at most $\|f\|_1$, and the adjoint identity is justified.

It remains to ensure necessity is a condition on the [kernel](../../../../../kernel-of-a-linear-map-split.md) itself. If $T_h=0$ for some $h\in L^1$, convolve $h$ with a smooth compactly supported [approximate identity](../../../../../approximate-identity.md) $\eta_\varepsilon\in L^1\cap L^2$. Since $T_h\eta_\varepsilon=0$, all these convolutions vanish. But $h*\eta_\varepsilon\to h$ in $L^1$, by continuity of translations in $L^1$, so $h=0$ almost everywhere. Thus the map from kernels to [convolution](../../../../../convolution.md) operators is [injective](../../../../../injective-function.md). Applying this to $h=f-f^\sharp$ yields the exact criterion

$$
\boxed{T_f=T_f^*\iff f(s)=\overline{f(-s)}\text{ for almost every }s.}
$$

For real-valued kernels this reduces to evenness; real-valuedness by itself is insufficient.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

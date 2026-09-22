<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [logic approximation for gene regulation](../../../../logic-approximation-for-gene-regulation.md), zero basal production and initially vanishing X, Y and Z. Let $K=K_{xy}=K_{xz}=K_{yz}=K_{xx}/2$, $Y_\infty=Z_\infty=\beta_y/\alpha$, and assume the activated Q level exceeds the X activation threshold. The circuit combines a [coherent feed-forward loop](../../../../coherent-feed-forward-loop.md) with [negative autoregulation](../../../../negative-autoregulation.md). While X is below its self-repression threshold it obeys $\dot X=\beta_x-\alpha X$, hence X first crosses $K$ at

$$
t_X=-\frac1\alpha\ln\left(1-\frac{\alpha K}{\beta_x}\right).
$$

Y production begins then. While X remains above $K$, $Y=Y_\infty[1-e^{-\alpha(t-t_X)}]$. The AND gate for Z first becomes active when Y reaches $K$, so

$$
\boxed{T_{\min}=t_X-\frac1\alpha\ln\left(1-\frac{\alpha K}{\beta_y}\right)
\simeq-\frac1\alpha\ln\left(1-\frac{\alpha K}{\beta_y}\right).}
$$

The approximation drops the short X build-up time because $\beta_x\gg\beta_y$. Strictly the input must last longer than this onset time to produce a nonzero amount of Z. This requires $\beta_y/\alpha>K$: at equality the threshold is approached only asymptotically, and below it Z never switches on. No numerical delay follows without the threshold-to-production ratio.

In the strong [negative autoregulation](../../../../negative-autoregulation.md) limit, X is held close to $K_{xx}=2K$; a smooth repression law regularizes the rapid switching of the ideal Boolean rule. After the input disappears at $t_0$, production of X stops and $X\simeq2Ke^{-\alpha(t-t_0)}$. It takes $(\ln2)/\alpha$ for X to fall below $K$. Until then Y remains at $Y_\infty>K$ and the Z AND gate stays on, so Z stays at $Z_\infty$. After that Z decays by dilution, taking another $(\ln2)/\alpha$ to halve. Therefore

$$
\boxed{t_{Z,1/2}-t_0\simeq\frac{2\ln2}{\alpha}.}
$$

More generally replace the first $\ln2$ by $\ln[X(t_0)/K]$. This distinguishes disappearance of the external ligand from disappearance of the persistent X [transcription factor](../../../../transcription-factor.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

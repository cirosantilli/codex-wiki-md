<h1 id="section-d/d12/solution">Solution</h1>

↑ **Parent:** [D12](../d12.md)

Define $s_i=\sin[2\pi(t_i-T)/P+\pi]$ and use the independent quoted Gaussian errors $\sigma=10\,\mathrm{m\,s^{-1}}$, with period and [exoplanet transit](../../../../../exoplanet-transit.md) epoch fixed. The model is linear in $K,V_0$ despite its sinusoidal [time](../../../../../time-in-physics.md) dependence. Minimize $\chi^2=\sum_i(V_i-Ks_i-V_0)^2/\sigma^2$. With $N=5$ the [normal equations](../../../../../normal-equation.md) are

$$
\begin{pmatrix}\sum s_i^2&\sum s_i\\\sum s_i&N\end{pmatrix}
\begin{pmatrix}K\\V_0\end{pmatrix}
=\begin{pmatrix}\sum s_iV_i\\\sum V_i\end{pmatrix}.
$$

Using $\sum s_i=-0.741472$ and $\sum s_i^2=2.824633$, the solution is

$$
\boxed{K=59.26\,\mathrm{m\,s^{-1}},\qquad
V_0=-15348.41\,\mathrm{m\,s^{-1}}.}
$$

The residuals in observation order are $(3.67,11.01,2.74,-7.90,-9.51)\,\mathrm{m\,s^{-1}}$. Therefore $\chi^2_{\min}=2.950$ for $5-2=3$ [degrees of freedom](../../../../../degree-of-freedom.md), giving reduced $\chi^2=0.983$. The upper-tail [probability](../../../../../probability.md) is about $0.40$: **the fit is consistent with the stated errors**, although five points do not establish a unique physical explanation.

For known errors the [covariance matrix](../../../../../covariance-matrix.md) is $\sigma^2(X^TX)^{-1}$. Equivalently, profiling out the fitted offset gives

$$
\sigma_K^2=\frac{\sigma^2}{\sum_i(s_i-\bar s)^2},\qquad
\boxed{\sigma_K=6.07\,\mathrm{m\,s^{-1}}.}
$$

This is the $\Delta\chi^2=1$ one-parameter uncertainty, not the curvature with $V_0$ incorrectly held fixed. Propagating it through the supplied [mass](../../../../../mass.md) relation, and treating its coefficient and $P$ as fixed,

$$
\boxed{m_p=(0.347\pm0.035)\,M_J.}
$$

The symbol $\pm nP$ in the [exoplanet transit](../../../../../exoplanet-transit.md) epoch denotes periodic copies of the same [exoplanet transit](../../../../../exoplanet-transit.md) phase, not an uncertainty [distribution](../../../../../distribution-mathematical-analysis.md) to propagate. No independent error for the empirical [mass](../../../../../mass.md) coefficient was supplied.

Additional independent observations retain positive weight even with twice the error: each has one quarter of the previous per-observation weight. Their information adds to the existing information [matrix](../../../../../matrix.md), so the formal [mass](../../../../../mass.md) uncertainty **decreases for informative additional orbital phases and cannot increase** under this fixed-error model. It can remain unchanged in a degenerate phase configuration that supplies no further [amplitude](../../../../../wave-amplitude.md) information after fitting the offset. The conclusion assumes the same correct model and independent errors, not a new fitted error rescaling or unmodelled systematic effects.

<a id="section-d/d12/image-original-plot-of-the-fitted-orbital-radial-velocity-variation-and-residuals-observed-numbers-used-without-reproducing-the-source-table"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2014/paper-1-radial-velocity.png)

**[Figure 4](#section-d/d12/image-original-plot-of-the-fitted-orbital-radial-velocity-variation-and-residuals-observed-numbers-used-without-reproducing-the-source-table). Original plot of the fitted orbital radial-velocity variation and residuals; observed numbers used without reproducing the source table**.

## ↑ Ancestors (14)

1. [D12](../d12.md)
2. [Section D](../../section-d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

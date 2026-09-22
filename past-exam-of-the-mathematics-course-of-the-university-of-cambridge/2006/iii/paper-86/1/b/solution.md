<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the initial [Half-range Fourier transform](../../../../../../half-range-fourier-transform.md) $Q(k)=\int_0^\infty e^{-ikx}q_0(x)\,dx$, and, for each available [boundary trace](../../../../../../boundary-trace-of-a-function.md), its [finite-time spectral boundary transform](../../../../../../finite-time-spectral-boundary-transform.md)

$$
F_j(k,t)=\int_0^t e^{ik^3s}f_j(s)\,ds.
$$

Temporarily let $f_j=\partial_x^jq(0,t)$ also denote the missing trace. Three [integrations by parts](../../../../../../integration-by-parts.md) in $x$ give

$$
\int_0^\infty e^{-ikx}q_{xxx}\,dx=-f_2-ikf_1+k^2f_0-ik^3\widehat q.
$$

Consequently the [backward-sign Airy half-line global relation](../../../../../../backward-sign-airy-half-line-global-relation.md) is

$$
\partial_t\widehat q+ik^3\widehat q=k^2f_0-ikf_1-f_2,\qquad
e^{ik^3t}\widehat q(k,t)=Q(k)+k^2F_0(k,t)-ikF_1(k,t)-F_2(k,t).
$$

The spatial transform is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) below the real axis, while each finite-time $F_j$ is an [entire function](../../../../../../entire-function.md). Moreover, $F_j(\alpha k,t)=F_j(\alpha^2k,t)=F_j(k,t)$ because $\alpha^3=1$.

Suppose the missing [derivative](../../../../../../derivative.md) has order $j$, and put $r=2-j$. Its contribution to the right-hand side is $a_jk^rF_j$, where $a_0=1$, $a_1=-i$, $a_2=-1$. Apply the inversion from the preceding part at time $t$ and select

$$
c_1=-\alpha^{-2r},\qquad c_2=-\alpha^{-r}.
$$

The rotated coefficients of that missing trace now equal minus its real-line coefficient. Its entire contribution is therefore

$$
\frac{a_j}{2\pi}\left(\int_{\mathbb R}-\int_{\partial E}-\int_{\partial D}\right)
e^{ikx-ik^3t}k^rF_j(k,t)\,dk.
$$

The real-axis pieces cancel. What remains is the boundary of the middle upper sector, outward on $\arg k=\pi/3$ and inward on $\arg k=2\pi/3$. In this sector $\operatorname{Im}k^3\leq0$, and

$$
e^{-ik^3t}F_j(k,t)=\int_0^t e^{-ik^3(t-s)}f_j(s)\,ds
$$

is bounded by $\int_0^t|f_j(s)|\,ds$. The factor $e^{ikx}$ decays exponentially throughout the closing arc, overcoming $k^r$. There are no poles. Thus the [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md) proves the [cubic-dispersion elimination of one missing boundary trace](../../../../../../cubic-dispersion-elimination-of-one-missing-boundary-trace.md) and removes every occurrence of the unknown $f_j$.

For a compact explicit answer, use only the two prescribed traces to form $S(k,t)=Q(k)+H(k,t)$. The three choices are

$$
\begin{array}{c|c|c|c}
\text{prescribed traces}&H(k,t)&c_1&c_2\\ \hline
f_0,f_1&k^2F_0-ikF_1&-1&-1\\
f_0,f_2&k^2F_0-F_2&-\alpha&-\alpha^2\\
f_1,f_2&-ikF_1-F_2&-\alpha^2&-\alpha
\end{array}
$$

For each row the solution is

$$
\boxed{\begin{aligned}
q(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-ik^3t}S(k,t)\,dk
&+\frac{c_1}{2\pi}\int_{\partial E}e^{ikx-ik^3t}S(\alpha^2k,t)\,dk\\
&+\frac{c_2}{2\pi}\int_{\partial D}e^{ikx-ik^3t}S(\alpha k,t)\,dk.
\end{aligned}}
$$

All quantities in this formula are transforms of the given data. On the [contour](../../../../../../complex-integration-contour.md) rays $k^3$ is real, so the time exponential is oscillatory; the [integrals](../../../../../../integral.md) use the usual limiting interpretation of [Fourier inversion](../../../../../../fourier-inversion-theorem.md). The decay estimate used for elimination belongs to the middle sector, not to $D$ or $E$, where $e^{-ik^3(t-s)}$ can grow.

At $t=0$, $F_j=0$ and the preceding inversion recovers $q_0$. The spectral exponential satisfies the [Airy equation](../../../../../../airy-equation.md) with the required minus sign. Differentiating the finite-time amplitudes produces only [derivatives](../../../../../../derivative.md) of the [Dirac delta](../../../../../../dirac-delta-function.md) supported at $x=0$ and zero rotated closed-[contour](../../../../../../complex-integration-contour.md) contributions, so the interior equation also holds. Finally, two solutions with the same data have $Q=H=0$ for their difference, so this representation gives zero: **each of the three prescribed pairs determines the solution uniquely in the smooth decaying class**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 86](../../../paper-86-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

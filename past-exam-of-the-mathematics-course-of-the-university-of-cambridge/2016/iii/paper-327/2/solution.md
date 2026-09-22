<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat\varphi(\xi)=\int e^{-ix\cdot\xi}\varphi(x)\,dx$, with inverse factor $(2\pi)^{-n}$. The [Paley–Wiener–Schwartz theorem](../../../../../paley-wiener-schwartz-theorem.md) can be stated with sharp convex support: for a nonempty [compact convex set](../../../../../compact-convex-set.md) $K\subset\mathbb R^n$, let its [support function](../../../../../support-function.md) be $H_K(\eta)=\sup_{x\in K}x\cdot\eta$. Then **$F$ is the [Fourier transform](../../../../../fourier-transform.md) of a unique [distribution](../../../../../distribution-mathematical-analysis.md) supported in $K$ if and only if it is entire and**

$$
\boxed{|F(z)|\leq C(1+|z|)^M e^{H_K(\operatorname{Im}z)}\quad(z\in\mathbb C^n)}
$$

for some $C$ and nonnegative integer $M$. For $K=\overline B_R$, this is the familiar bound $C(1+|z|)^M e^{R|\operatorname{Im}z|}$. Allowing some $R$ characterizes all [compactly supported distributions](../../../../../compactly-supported-distribution.md). Here the extension of the [Fourier transform](../../../../../fourier-transform.md) is $F(z)=\langle u,e^{-ix\cdot z}\rangle$, interpreted with a cutoff equal to one near the [support of a distribution](../../../../../support-of-a-distribution.md).

First suppose $\operatorname{supp}u\subset K$. Fix one [smooth cutoff function](../../../../../smooth-cutoff-function.md) equal to one near $K$. Pairing the resulting compactly supported exponential with $u$ shows that $F$ is an [entire function](../../../../../entire-function.md): differentiation with respect to $z_j$ inserts $-ix_j$, and the power series converges in the test-function [seminorms](../../../../../seminorm.md) uniformly on compact subsets of $\mathbb C^n$.

To keep the exponential type exactly $H_K$, rather than that of a fixed larger neighborhood, use a [shrinking-cutoff exponential-type estimate](../../../../../shrinking-cutoff-exponential-type-estimate.md). There are cutoffs $\chi_\varepsilon$ equal to one on $K+\varepsilon B_1$, supported in $K+3\varepsilon\overline B_1$, and satisfying $|\partial^\alpha\chi_\varepsilon|\leq C_\alpha\varepsilon^{-|\alpha|}$ for $0<\varepsilon\leq1$. One construction convolves the indicator of $K+2\varepsilon B_1$ with a unit-mass [mollifier](../../../../../mollifier.md) supported in $\varepsilon B_1$. Continuity of $u$ on a fixed compact neighborhood gives a finite [order of a distribution](../../../../../order-of-a-distribution.md) $q$ there. By the product rule,

$$
|F(z)|=|\langle u,\chi_\varepsilon e^{-ix\cdot z}\rangle|
\leq C\varepsilon^{-q}(1+|z|)^q
\exp\big(H_K(\operatorname{Im}z)+3\varepsilon|\operatorname{Im}z|\big).
$$

Taking $\varepsilon=(1+|z|)^{-1}$ proves the required bound with $M=2q$, since the extra exponential factor is at most $e^3$. The value of the pairing is independent of the chosen cutoff because all cutoffs agree near $\operatorname{supp}u$. Thus the forward direction has the exact asserted [support function](../../../../../support-function.md), without an unproved estimate on derivatives restricted only to $K$.

Conversely, suppose the entire $F$ has the stated bound. Its restriction to real frequency has polynomial growth, so define a [tempered distribution](../../../../../tempered-distribution.md) $u$ by

$$
\langle u,\varphi\rangle=(2\pi)^{-n}\int_{\mathbb R^n}F(\xi)\widehat\varphi(-\xi)\,d\xi,
\qquad\varphi\in\mathcal S(\mathbb R^n).
$$

The [Schwartz space](../../../../../schwartz-space.md) decay makes this integral absolutely convergent and continuous; by [Fourier inversion](../../../../../fourier-inversion-theorem.md), $\widehat u=F$ on real frequency. It remains to prove the support assertion by [mollifier regularization for contour recovery of support](../../../../../mollifier-regularization-for-contour-recovery-of-support.md).

Choose a nonnegative unit-mass [mollifier](../../../../../mollifier.md) $\rho$ supported in $B_1$, and set

$$
F_\varepsilon(z)=F(z)\widehat\rho(\varepsilon z),\qquad
h_\varepsilon(x)=(2\pi)^{-n}\int_{\mathbb R^n}e^{ix\cdot\xi}F_\varepsilon(\xi)\,d\xi.
$$

On real frequency, $F_\varepsilon$ decays faster than any polynomial after enough applications of [integration by parts](../../../../../integration-by-parts.md) to $\widehat\rho$; hence $h_\varepsilon$ is smooth, by [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md). More generally, for every integer $L$ there is $C_{\varepsilon,L}$ such that

$$
|\widehat\rho(\varepsilon(\xi+i\eta))|
\leq C_{\varepsilon,L}(1+|\xi|)^{-L}(1+|\eta|)^L e^{\varepsilon|\eta|}.
$$

To obtain this estimate, write the transform of $\rho_\varepsilon$ as the real-frequency transform of $e^{x\cdot\eta}\rho_\varepsilon(x)$ and integrate by parts; each derivative introduces at most one factor of $|\eta|$.

Fix a unit vector $v$ and take $L>M+n+1$. A [contour-shift proof of the Paley–Wiener–Schwartz theorem](../../../../../contour-shift-proof-of-the-paley-wiener-schwartz-theorem.md) moves the inverse-transform contour to $\mathbb R^n+itv$:

$$
h_\varepsilon(x)=(2\pi)^{-n}\int_{\mathbb R^n}e^{ix\cdot(\xi+itv)}F_\varepsilon(\xi+itv)\,d\xi.
$$

Here is a justification of the shift. Rotate coordinates so $v$ is the first coordinate direction, apply the [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) on a rectangle in the first complex variable, and integrate over the other real variables. For fixed $t$, the vertical sides at real part $\pm A$ have an integrated bound proportional to $A^{M-L+n-1}$, and hence vanish as $A\to\infty$. The same decay bounds give absolute convergence on the horizontal sides. No contour shift of an unregularized polynomially growing integral is needed.

Positive homogeneity of the [support function](../../../../../support-function.md) now gives

$$
|h_\varepsilon(x)|\leq C_{\varepsilon,L}(1+t)^{M+L}
\exp\big(-t[x\cdot v-H_K(v)-\varepsilon]\big).
$$

If $x\notin K+\varepsilon\overline B_1$, the [Hahn-Banach separation theorem](../../../../../hahn-banach-separation-theorem.md) supplies a unit vector $v$ with $x\cdot v>H_K(v)+\varepsilon$. Letting $t\to\infty$ proves $h_\varepsilon(x)=0$. Therefore $h_\varepsilon\in C_c^\infty$ and $\operatorname{supp}h_\varepsilon\subset K+\varepsilon\overline B_1$.

Since $\widehat\rho(\varepsilon\xi)\to1$ and its modulus is at most one on real frequency, the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) in the formula for $\langle u,\varphi\rangle$ gives $h_\varepsilon\to u$ as [tempered distributions](../../../../../tempered-distribution.md), and thus as [distributions](../../../../../distribution-mathematical-analysis.md). A [test function](../../../../../test-function.md) supported outside $K$ has positive distance from $K$, so its pairing with $h_\varepsilon$ is zero for all sufficiently small $\varepsilon$. This proves $\operatorname{supp}u\subset K$. The [Fourier transform of a compactly supported distribution](../../../../../fourier-transform-of-a-compactly-supported-distribution.md) constructed in the forward direction equals $F$ on $\mathbb R^n$; applying the one-variable [identity theorem](../../../../../identity-theorem.md) successively in each coordinate extends the equality to $\mathbb C^n$. Injectivity of the [Fourier transform of a tempered distribution](../../../../../fourier-transform-of-a-tempered-distribution.md) proves uniqueness and completes both directions.

For the independence application, put $g_m(z)=e^{iz\cdot y_m}f_m(z)$ and $r_m=1/(m+1)$. The ball version of the [Paley–Wiener–Schwartz theorem](../../../../../paley-wiener-schwartz-theorem.md) supplies a nonzero [distribution](../../../../../distribution-mathematical-analysis.md) $v_m$ supported in $\overline B_{r_m}(0)$ with $\widehat v_m=g_m$. By the [Translation property of the Fourier transform](../../../../../translation-property-of-the-fourier-transform.md),

$$
f_m(z)=e^{-iz\cdot y_m}\widehat v_m(z)=\widehat w_m(z),\qquad
w_m=\tau_{y_m}v_m,\qquad
\operatorname{supp}w_m\subset\overline B_{r_m}(y_m),
$$

where $\langle\tau_y v,\varphi\rangle=\langle v,\varphi(\,\cdot+y)\rangle$. Distinct integer points are at least distance one apart. For distinct positive indices $j,k$, the largest possible radius sum is $1/2+1/3=5/6<1$. Thus these closed balls, and hence the [distribution supports](../../../../../support-of-a-distribution.md), are pairwise disjoint.

If $\sum_{m=1}^N c_mf_m=0$, injectivity of the [Fourier transform](../../../../../fourier-transform.md) gives $\sum_m c_mw_m=0$. For each $j$, choose a [smooth cutoff function](../../../../../smooth-cutoff-function.md) equal to one near its ball and zero near all other balls. Multiplying the distributional identity by this cutoff isolates $c_jw_j=0$. Since $f_j$ is not identically zero, $w_j\ne0$, so $c_j=0$. Consequently **$f_1,\ldots,f_N$ are linearly independent over $\mathbb C$**. This [Fourier independence from disjoint distribution supports](../../../../../fourier-independence-from-disjoint-distribution-supports.md) uses the quantitative exponential types to establish support separation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 327](../../paper-327-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

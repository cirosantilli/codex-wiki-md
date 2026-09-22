<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $d=U'(0)>0$, $h=U'''(0)$, $p=\phi_0(0)\ne0$, and $q=\phi_0'(0)$. At a regular neutral [Rayleigh equation for inviscid shear flow](../../../../../rayleigh-equation-for-inviscid-shear-flow.md) mode, multiply the equation by $U-c_0$ and evaluate it at the [critical layer in a shear flow](../../../../../critical-layer-in-a-shear-flow.md). The term multiplying $\phi_0''-k_0^2\phi_0$ vanishes, leaving $U''(0)p=0$. Therefore $U''(0)=0$. If this condition failed, the coefficient $U''/(U-c_0)$ would have a simple pole and a nonzero $p$ would force a logarithmically singular slope instead of a regular [eigenfunction](../../../../../eigenfunction.md).

**There is a sign error in the printed first-order equation.** Direct expansion of the original [Rayleigh equation for inviscid shear flow](../../../../../rayleigh-equation-for-inviscid-shear-flow.md) gives

$$
L_0\phi_1=H\phi_0,\qquad L_0=\frac{d^2}{dy^2}-k_0^2-\frac{U''}{U-c_0},\qquad H=2k_0k_1+\frac{c_1U''}{(U-c_0)^2}.
$$

The coefficient on the left must have a minus sign. Indeed, $1/(U-c)=1/(U-c_0)+\varepsilon c_1/(U-c_0)^2+\cdots$, and moving both first-order parameter corrections to the right gives exactly this equation. The plus sign printed there is incompatible with the original equation and its neutral [eigenfunction](../../../../../eigenfunction.md). The later matching and integral formulas follow from the corrected equation. The PDF also has $y^3h/6$ in the [Taylor expansion](../../../../../taylor-expansion.md) of $U$, and $U'''(0)$ in the requested logarithmic coefficient; these are mistranscribed in the converted TeX.

Near zero, $U-c_0=dy+hy^3/6+\cdots$ and $U''=hy+O(y^2)$. Thus $U''/(U-c_0)\to h/d$, whereas $U''/(U-c_0)^2=h/(d^2y)+O(1)$. The singular part of the first-order equation is

$$
\phi_1''\sim\frac{c_1hp}{d^2y}.
$$

Integrating twice on either side gives

$$
\phi_1(y)=a+\beta_\pm y\log|y|+b_\pm y+\cdots,\qquad \boxed{\beta_+=\beta_-=\beta=\frac{c_1hp}{d^2}.}
$$

The constant $a$ is common because the inner solution is continuous. The coefficient necessarily also contains $p$: rescaling the neutral [eigenfunction](../../../../../eigenfunction.md) rescales its correction. One may choose the normalization $p=1$ if a formula only in terms of the flow derivatives and $c_1$ is wanted.

The [outer expansion](../../../../../outer-expansion.md) of $1/(U-c)$ fails when $|dy|$ is comparable with $\varepsilon|c_1|$. Therefore the [distinguished limit](../../../../../distinguished-limit.md) is

$$
\boxed{y=\varepsilon\eta,\qquad\ell=1.}
$$

In this [inner variable](../../../../../inner-variable.md), the original equation becomes

$$
\Phi_{\eta\eta}=\varepsilon^2\left(k^2+\frac{U''(\varepsilon\eta)}{U(\varepsilon\eta)-c}\right)\Phi.
$$

At orders one and $\varepsilon$, its right side is zero. Matching the [outer expansion](../../../../../outer-expansion.md) therefore selects $\Phi_0=p$ and $\Phi_1=q\eta+a$. At order $\varepsilon^2\log\varepsilon$, $\theta_2''=0$. The outer term $\varepsilon\beta y\log|y|$ becomes $\varepsilon^2\beta\eta(\log\varepsilon+\log|\eta|)$, so the required [switchback term](../../../../../switchback-term.md) is $\theta_2=\beta\eta$. At order $\varepsilon^2$,

$$
\Phi_2''=p k_0^2+\frac{ph\eta}{d\eta-c_1}.
$$

Integrating, or using the supplied hint, gives

$$
\boxed{\Phi_2=\frac p2\left(k_0^2+\frac hd\right)\eta^2+\frac{phc_1}{d^3}\left[(d\eta-c_1)\log(d\eta-c_1)-(d\eta-c_1)\right]+B\eta+C.}
$$

The constants $B,C$ are homogeneous matching freedoms; they do not affect the slope jump. The quadratic term agrees with $\phi_0''(0)=p(k_0^2+h/d)$, another check on the sign of $L_0$.

For $\operatorname{Im}c_1>0$, $d\eta-c_1$ runs below the real axis. Choose the continuous [branch of the complex logarithm](../../../../../branch-of-the-complex-logarithm.md) there. At positive infinity its argument tends to zero; at negative infinity it tends to $-\pi$. Thus the linear parts of the two large-$|\eta|$ expansions of $\Phi_2$ are

$$
\begin{aligned}
\eta\to+\infty:\quad&\beta\eta\log|\eta|+\bigl[B+\beta(\log d-1)\bigr]\eta,\\
\eta\to-\infty:\quad&\beta\eta\log|\eta|+\bigl[B+\beta(\log d-1)-i\pi\beta\bigr]\eta.
\end{aligned}
$$

These expressions omit the already matched common quadratic term and terms only logarithmic or constant in $\eta$. Matching the linear coefficients to $b_\pm$ proves the [neutral-mode critical-layer matching](../../../../../neutral-mode-critical-layer-matching.md) relation

$$
\boxed{b_+-b_-=i\pi\beta=\frac{i\pi c_1U'''(0)\phi_0(0)}{U'(0)^2}.}
$$

The sign comes from passing below the pole; taking $\operatorname{Im}c_1<0$ would reverse it.

Finally use the [Wronskian](../../../../../wronskian.md) $W=\phi_1\phi_0'-\phi_0\phi_1'$. Since $L_0\phi_0=0$ and $L_0\phi_1=H\phi_0$, subtraction gives $W'=-H\phi_0^2$. The wall [boundary conditions](../../../../../boundary-condition.md) give $W(a)=W(b)=0$, so

$$
\left(\int_a^{-\delta}+\int_\delta^b\right)H\phi_0^2\,dy=W(\delta)-W(-\delta).
$$

This is the requested excised-interval identity. As $\delta\downarrow0$, the equal logarithmic slope terms cancel and

$$
W(\delta)-W(-\delta)\longrightarrow-p(b_+-b_-)=-\frac{i\pi c_1hp^2}{d^2}.
$$

The remaining real singular integral is interpreted as a [Cauchy principal value](../../../../../cauchy-principal-value.md), consistent with excision on both sides of the [critical layer in a shear flow](../../../../../critical-layer-in-a-shear-flow.md). Define

$$
I=\int_a^b\phi_0^2dy,\qquad J=\operatorname{PV}\int_a^b\frac{U''\phi_0^2}{(U-c_0)^2}dy,\qquad M=\frac{hp^2}{d^2}.
$$

Then the [neutral Rayleigh-mode dispersion correction](../../../../../neutral-rayleigh-mode-dispersion-correction.md) is

$$
\boxed{2k_0k_1I=-c_1(J+i\pi M),\qquad c_1=-\frac{2k_0k_1I}{J+i\pi M},}
$$

where the last form assumes a nonzero denominator. For real $k_1$, $\operatorname{Im}c_1=2k_0k_1I\pi M/(J^2+\pi^2M^2)$, so the assumed growing branch must have the corresponding sign. If $h=0$, the displayed logarithmic coefficient and jump vanish; further degeneracy can require higher-order analysis. No nonzero growth rate follows from that degenerate first-order calculation alone.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

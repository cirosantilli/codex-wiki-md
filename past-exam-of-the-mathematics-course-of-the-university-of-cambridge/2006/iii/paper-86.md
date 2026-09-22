# Paper 86

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper86.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper86.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)

## 1

↑ **Parent:** [Paper 86](paper-86.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Extend $q$ by zero to the negative half-line. Its ordinary [Fourier transform](../../../analysis.md#fourier-transform) is then exactly the [Half-range Fourier transform](../../../analysis.md#half-range-fourier-transform) $\widehat q(k)$. The [Fourier inversion theorem](../../../fourier-analysis.md#fourier-inversion-theorem) gives the real-line term for $x>0$; no endpoint convention at $x=0$ is needed.

It remains to show that each extra [contour](../../../complex-analysis.md#complex-integration-contour) contributes zero, independently of its coefficient. For $\operatorname{Im}k<0$, the [integral](../../../calculus.md#integral) defining $\widehat q$ is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point). With $\alpha=e^{2\pi i/3}$, multiplication by $\alpha^2$ rotates the sector $E$ into $-2\pi/3\leq\arg(\alpha^2k)\leq-\pi/3$, and multiplication by $\alpha$ rotates $D$ into $-2\pi/3\leq\arg(\alpha k)\leq-\pi/3$. Thus the two rotated transforms are [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) on their respective upper sectors.

Orient the [contours](../../../complex-analysis.md#complex-integration-contour) as in the PDF: $\partial E$ runs from infinity on the $\pi/3$ ray into zero and then out along the positive real axis; $\partial D$ runs from negative real infinity into zero and then out along the $2\pi/3$ ray. Both have their sector on their left. Smooth decay and [integration by parts](../../../calculus.md#integration-by-parts) give $\widehat q(k)=O(1/k)$ in closed lower-half-plane sectors. The factor $e^{ikx}$ decays in the [upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) for $x>0$. Close each sector by a large arc; the arc [integral](../../../calculus.md#integral) vanishes by [Jordan lemma](../../../complex-analysis.md#jordan-s-lemma), including its short portion near the real axis. The [Cauchy integral theorem](../../../complex-analysis.md#cauchy-s-integral-theorem) therefore gives the [rotated null contours for half-range Fourier inversion](../../../analysis.md#rotated-null-contours-for-half-range-fourier-inversion):

$$
\boxed{\int_{\partial E}e^{ikx}\widehat q(\alpha^2k)\,dk=0,\qquad
\int_{\partial D}e^{ikx}\widehat q(\alpha k)\,dk=0\quad(x>0).}
$$

Adding arbitrary constant multiples of these two zero [integrals](../../../calculus.md#integral) to ordinary [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) proves the asserted inversion formula. **The constants $c_1,c_2$ are arbitrary in this part**; selecting them later is what removes an unknown [boundary trace](../../../differential-equation.md#boundary-trace-of-a-function).

<a id="1/a/image-the-rotated-inversion-sectors-and-the-middle-sector-that-eliminates-an-unknown-boundary-transform"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-86-cubic-contours.png)

**[Figure 1](#1/a/image-the-rotated-inversion-sectors-and-the-middle-sector-that-eliminates-an-unknown-boundary-transform). The rotated inversion sectors and the middle sector that eliminates an unknown boundary transform**.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Define the initial [Half-range Fourier transform](../../../analysis.md#half-range-fourier-transform) $Q(k)=\int_0^\infty e^{-ikx}q_0(x)\,dx$, and, for each available [boundary trace](../../../differential-equation.md#boundary-trace-of-a-function), its [finite-time spectral boundary transform](../../../differential-equation.md#finite-time-spectral-boundary-transform)

$$
F_j(k,t)=\int_0^t e^{ik^3s}f_j(s)\,ds.
$$

Temporarily let $f_j=\partial_x^jq(0,t)$ also denote the missing trace. Three [integrations by parts](../../../calculus.md#integration-by-parts) in $x$ give

$$
\int_0^\infty e^{-ikx}q_{xxx}\,dx=-f_2-ikf_1+k^2f_0-ik^3\widehat q.
$$

Consequently the [backward-sign Airy half-line global relation](../../../integrable-systems.md#backward-sign-airy-half-line-global-relation) is

$$
\partial_t\widehat q+ik^3\widehat q=k^2f_0-ikf_1-f_2,\qquad
e^{ik^3t}\widehat q(k,t)=Q(k)+k^2F_0(k,t)-ikF_1(k,t)-F_2(k,t).
$$

The spatial transform is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) below the real axis, while each finite-time $F_j$ is an [entire function](../../../complex-analysis.md#entire-function). Moreover, $F_j(\alpha k,t)=F_j(\alpha^2k,t)=F_j(k,t)$ because $\alpha^3=1$.

Suppose the missing [derivative](../../../calculus.md#derivative) has order $j$, and put $r=2-j$. Its contribution to the right-hand side is $a_jk^rF_j$, where $a_0=1$, $a_1=-i$, $a_2=-1$. Apply the inversion from the preceding part at time $t$ and select

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

is bounded by $\int_0^t|f_j(s)|\,ds$. The factor $e^{ikx}$ decays exponentially throughout the closing arc, overcoming $k^r$. There are no poles. Thus the [Cauchy integral theorem](../../../complex-analysis.md#cauchy-s-integral-theorem) proves the [cubic-dispersion elimination of one missing boundary trace](../../../differential-equation.md#cubic-dispersion-elimination-of-one-missing-boundary-trace) and removes every occurrence of the unknown $f_j$.

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

All quantities in this formula are transforms of the given data. On the [contour](../../../complex-analysis.md#complex-integration-contour) rays $k^3$ is real, so the time exponential is oscillatory; the [integrals](../../../calculus.md#integral) use the usual limiting interpretation of [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem). The decay estimate used for elimination belongs to the middle sector, not to $D$ or $E$, where $e^{-ik^3(t-s)}$ can grow.

At $t=0$, $F_j=0$ and the preceding inversion recovers $q_0$. The spectral exponential satisfies the [Airy equation](../../../integrable-systems.md#airy-equation) with the required minus sign. Differentiating the finite-time amplitudes produces only [derivatives](../../../calculus.md#derivative) of the [Dirac delta](../../../distribution-theory.md#dirac-delta-function) supported at $x=0$ and zero rotated closed-[contour](../../../complex-analysis.md#complex-integration-contour) contributions, so the interior equation also holds. Finally, two solutions with the same data have $Q=H=0$ for their difference, so this representation gives zero: **each of the three prescribed pairs determines the solution uniquely in the smooth decaying class**.

## 2

↑ **Parent:** [Paper 86](paper-86.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use the [Wirtinger derivative](../../../analysis.md#wirtinger-derivatives) $f=q_z=(q_x-iq_y)/2$. Since $q$ satisfies the [Laplace equation](../../../partial-differential-equation.md#laplace-equation), $\partial_{\bar z}f=\Delta q/4=0$, so $f$ is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point). The differential relation is understood as a [one-form](../../../differential-form.md#one-form) identity:

$$
d(\mu e^{-ikz})=e^{-ikz}f(z)\,dz.
$$

The differential $dz$ is needed on its right-hand side. Because this form is closed, its [integral](../../../calculus.md#integral) is independent of path within the semistrip.

Three spectral primitives are obtained by integrating from the two finite corners and from the infinite end:

$$
\mu_0=e^{ikz}\int_0^ze^{-ikw}f(w)\,dw,\qquad
\mu_l=e^{ikz}\int_{il}^ze^{-ikw}f(w)\,dw,\qquad
\mu_\infty=-e^{ikz}\int_z^{\infty+i\,\operatorname{Im}z}e^{-ikw}f(w)\,dw.
$$

The last [integral](../../../calculus.md#integral) is taken horizontally and defines the infinite-end primitive for $\operatorname{Im}k<0$. Their differences are $e^{ikz}$ times the three boundary spectral [functions](../../../function.md). Using counterclockwise boundary orientation, define

$$
\rho_L(k)=\int_{il}^0e^{-ikw}f(w)\,dw,\qquad
\rho_B(k)=\int_0^\infty e^{-ikx}f(x)\,dx,\qquad
\rho_T(k)=-e^{kl}\int_0^\infty e^{-ikx}f(x+il)\,dx.
$$

Then $\mu_0-\mu_\infty=e^{ikz}\rho_B$, $\mu_\infty-\mu_l=e^{ikz}\rho_T$, and $\mu_l-\mu_0=e^{ikz}\rho_L$. Their sum gives the [global relation](../../../differential-equation.md#global-relation-for-a-linear-boundary-value-problem) $\rho_L+\rho_B+\rho_T=0$ for $\operatorname{Im}k\leq0$.

To express these spectra in boundary data, write $g_0(x)=q(x,0)$, $g_l(x)=q(x,l)$, $h(y)=q(0,y)$, $n_0(x)=q_y(x,0)$, $n_l(x)=q_y(x,l)$, and $v(y)=q_x(0,y)$. Direct substitution into $f$ gives

$$
\begin{aligned}
\rho_B(k)&=\frac12\int_0^\infty e^{-ikx}[g_0'(x)-in_0(x)]\,dx,\\
\rho_T(k)&=-\frac{e^{kl}}2\int_0^\infty e^{-ikx}[g_l'(x)-in_l(x)]\,dx,\\
\rho_L(k)&=-\frac12\int_0^le^{ky}[h'(y)+iv(y)]\,dy.
\end{aligned}
$$

These are transforms of tangential [derivatives](../../../calculus.md#derivative) of [Dirichlet boundary data](../../../differential-equation.md#dirichlet-boundary-data) and the corresponding [Neumann boundary data](../../../differential-equation.md#neumann-boundary-data). The outward [derivatives](../../../calculus.md#derivative) are $-n_0$ at the bottom, $n_l$ at the top, and $-v$ at the left.

The [boundary spectral representation of a holomorphic function on a semistrip](../../../differential-equation.md#boundary-spectral-representation-of-a-holomorphic-function-on-a-semistrip) is

$$
\boxed{q_z(z)=\frac1{2\pi}\left[
\int_0^{i\infty}e^{ikz}\rho_L(k)\,dk
+\int_0^\infty e^{ikz}\rho_B(k)\,dk
+\int_0^{-\infty}e^{ikz}\rho_T(k)\,dk\right].}
$$

All three $k$-rays are oriented outward from zero. To verify the spectral inversion, use

$$
\int_0^{e^{i\theta}\infty}e^{ik(z-w)}\,dk=\frac{i}{z-w}
$$

whenever the exponential decays. The positive real ray works for the bottom, the negative real ray for the top, and the positive imaginary ray for the left. Substitution of the boundary spectra therefore turns the boxed formula into $(2\pi i)^{-1}\int_{\partial\Omega}f(w)/(w-z)\,dw=f(z)$ by the [Cauchy integral formula](../../../analysis.md#cauchy-integral-formula). This also fixes all orientation signs.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $G_0(k),G_l(k)$ denote the [Half-range Fourier transforms](../../../analysis.md#half-range-fourier-transform) of $g_0,g_l$, and let $N_0(k),N_l(k)$ denote those of the upward [derivatives](../../../calculus.md#derivative) $n_0,n_l$. Also set

$$
H(k)=\int_0^le^{ky}h(y)\,dy,\qquad
W(k)=\int_0^le^{ky}v(y)\,dy.
$$

Integrate the tangential [derivatives](../../../calculus.md#derivative) in the three spectral [functions](../../../function.md) by parts. For example, $\int_0^\infty e^{-ikx}g_0'=-h(0)+ikG_0$, and $\int_0^le^{ky}h'=e^{kl}h(l)-h(0)-kH$. All corner values cancel in $\rho_L+\rho_B+\rho_T=0$. The result is the [semistrip Laplace spectral global relation](../../../differential-equation.md#semistrip-laplace-spectral-global-relation)

$$
e^{kl}N_l(k)-N_0(k)+k[G_0(k)-e^{kl}G_l(k)]-W(k)-ikH(k)=0.
$$

For $\kappa>0$, use the [sine transforms](../../../analysis.md#fourier-sine-transform)

$$
G_j^s(\kappa)=\int_0^\infty\sin(\kappa x)g_j(x)\,dx,\qquad
S_j(\kappa)=\int_0^\infty\sin(\kappa x)n_j(x)\,dx.
$$

Reality of $q$ makes $W(\kappa)$ and $W(-\kappa)$ real, so taking imaginary parts removes the unknown left-side [normal derivative](../../../differential-geometry.md#normal-derivative). At $k=\kappa$ and $k=-\kappa$ the two consequences of the [global relation](../../../differential-equation.md#global-relation-for-a-linear-boundary-value-problem) are

$$
\begin{aligned}
e^{\kappa l}S_l-S_0
&=\kappa[e^{\kappa l}G_l^s-G_0^s-H(\kappa)],\\
e^{-\kappa l}S_l-S_0
&=\kappa[G_0^s-e^{-\kappa l}G_l^s-H(-\kappa)].
\end{aligned}
$$

Subtracting these equations and then substituting back gives the [semistrip Dirichlet-to-Neumann sine transforms](../../../differential-equation.md#semistrip-dirichlet-to-neumann-sine-transforms) entirely in terms of the prescribed [Dirichlet boundary data](../../../differential-equation.md#dirichlet-boundary-data):

$$
\boxed{S_0(\kappa)=\frac{\kappa}{\sinh(\kappa l)}
\left[-\cosh(\kappa l)G_0^s(\kappa)+G_l^s(\kappa)
+\int_0^l\sinh(\kappa(l-y))h(y)\,dy\right],}
$$



$$
\boxed{S_l(\kappa)=\frac{\kappa}{\sinh(\kappa l)}
\left[-G_0^s(\kappa)+\cosh(\kappa l)G_l^s(\kappa)
-\int_0^l\sinh(\kappa y)h(y)\,dy\right].}
$$

These are the requested transforms of $q_y$ itself. The bottom outward [Neumann boundary data](../../../differential-equation.md#neumann-boundary-data) have the opposite sign. The apparent division at $\kappa=0$ is handled by a continuous limit whenever the corresponding moments exist; there is no singularity for any $\kappa>0$.

## 3

↑ **Parent:** [Paper 86](paper-86.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $s_j=\sin\beta_j$, $c_j=\cos\beta_j$. Inverting the two orthogonal [derivative](../../../calculus.md#derivative) systems gives, on the vertical axis,

$$
q_x(0,y)=-s_1h_1(y)-c_1j_1(y),\qquad
q_y(0,y)=c_1h_1(y)-s_1j_1(y),
$$

and, on the horizontal axis,

$$
q_x(x,0)=c_2h_2(x)+s_2j_2(x),\qquad
q_y(x,0)=-s_2h_2(x)+c_2j_2(x).
$$

Using the [Wirtinger derivative](../../../analysis.md#wirtinger-derivatives) $q_z=(q_x-iq_y)/2$, these become

$$
q_z(iy)=-\frac{e^{-i\beta_1}}2[j_1(y)+ih_1(y)],\qquad
q_z(x)=\frac{e^{i\beta_2}}2[h_2(x)-ij_2(x)].
$$

Define the appropriate boundary transforms by

$$
\begin{aligned}
H_1(k)&=\int_0^\infty e^{ky}h_1(y)\,dy,&J_1(k)&=\int_0^\infty e^{ky}j_1(y)\,dy,\\
H_2(k)&=\int_0^\infty e^{-ikx}h_2(x)\,dx,&J_2(k)&=\int_0^\infty e^{-ikx}j_2(x)\,dx.
\end{aligned}
$$

The first pair is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) for $\operatorname{Re}k<0$; the second pair consists of [Half-range Fourier transforms](../../../analysis.md#half-range-fourier-transform), [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) for $\operatorname{Im}k<0$. Parametrizing the vertical boundary by $z=iy$ gives $dz=i\,dy$, which must be retained. Substitution yields the [quarter-plane oblique boundary spectral functions](../../../differential-equation.md#quarter-plane-oblique-boundary-spectral-functions):

$$
\boxed{\widehat q_1(k)=\frac{e^{-i\beta_1}}2[H_1(k)-iJ_1(k)],\qquad
\widehat q_2(k)=-\frac{e^{i\beta_2}}2[H_2(k)-iJ_2(k)].}
$$

Their signs follow from the stated clockwise boundary orientations: upward on the left and inward on the bottom.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Since $q$ is [harmonic](../../../partial-differential-equation.md#harmonic-function), $q_z$ is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) and the [one-form](../../../differential-form.md#one-form) $e^{-ikz}q_z\,dz$ is closed. Closing the physical quadrant at infinity gives the [global relation](../../../differential-equation.md#global-relation-for-a-linear-boundary-value-problem)

$$
\widehat q_1(k)+\widehat q_2(k)=0\qquad
(\operatorname{Re}k<0,\ \operatorname{Im}k<0).
$$

In this third spectral quadrant the exponential decays on both boundary axes. Set $\gamma=\beta_1+\beta_2$. The relation becomes

$$
H_1(k)-iJ_1(k)=e^{i\gamma}[H_2(k)-iJ_2(k)].
$$

All four boundary [functions](../../../function.md) are real. Consequently their transforms obey

$$
\overline{H_1(\bar k)}=H_1(k),\qquad
\overline{H_2(-\bar k)}=H_2(k),
$$

and the same identities for $J_1,J_2$. [Complex conjugation](../../../complex-analysis.md#complex-conjugation) of the [global relation](../../../differential-equation.md#global-relation-for-a-linear-boundary-value-problem) therefore gives its upper-left consequence

$$
H_1(k)+iJ_1(k)=e^{-i\gamma}[H_2(-k)+iJ_2(-k)]
\qquad(\operatorname{Re}k<0,\ \operatorname{Im}k>0).
$$

Introduce just one unknown [function](../../../function.md),

$$
\boxed{\Phi(k)=H_2(-k)-iJ_2(-k)
=\int_0^\infty e^{ikx}[h_2(x)-ij_2(x)]\,dx,\qquad\operatorname{Im}k>0.}
$$

It is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) in the [upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis). Under the transform-admissible decay assumptions, $|\Phi(k)|\leq\int_0^\infty(|h_2|+|j_2|)\,dx$, so it is bounded there.

For $k$ on the positive real ray, use both consequences of the [global relation](../../../differential-equation.md#global-relation-for-a-linear-boundary-value-problem) at $-k$. Adding them removes $J_1(-k)$ and gives

$$
H_2(k)+iJ_2(k)=2e^{i\gamma}H_1(-k)-e^{2i\gamma}\Phi(k).
$$

For $k$ on the positive imaginary ray, use the upper-left relation and $H_2(-k)+iJ_2(-k)=2H_2(-k)-\Phi(k)$. The resulting [single-function spectral elimination for a rational-angle quadrant](../../../differential-equation.md#single-function-spectral-elimination-for-a-rational-angle-quadrant) is

$$
\boxed{\begin{aligned}
\widehat q_2(k)&=-e^{i\beta_2}[H_2(k)-e^{i\gamma}H_1(-k)]
-\frac{e^{i\beta_2+2i\gamma}}2\Phi(k),\qquad k>0,\\
\widehat q_1(k)&=e^{-i\beta_1}[H_1(k)-e^{-i\gamma}H_2(-k)]
+\frac{e^{-i\beta_1-i\gamma}}2\Phi(k),\qquad k\in i\mathbb R_+.
\end{aligned}}
$$

Boundary limits from the appropriate transform domains are understood. Every remaining unknown boundary [derivative](../../../calculus.md#derivative) is contained in the one bounded upper-half-plane [function](../../../function.md) $\Phi$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

First resolve the [orientation sign in quadrant harmonic spectral inversion](../../../analysis.md#orientation-sign-in-quadrant-harmonic-spectral-inversion). The printed spectral definitions traverse the physical boundary clockwise, whereas both reconstruction rays run outward from zero. Integrating first in $k$ gives the kernel $i/(z-w)$. The resulting clockwise [Cauchy integral](../../../complex-analysis.md#cauchy-transform) is the negative of the desired [holomorphic function](../../../complex-analysis.md#holomorphic-function). Thus, with exactly the spectral definitions used above, the consistent reconstruction is

$$
q_z(z)=-\frac1{2\pi}\left[\int_0^\infty e^{ikz}\widehat q_2(k)\,dk+
\int_0^{i\infty}e^{ikz}\widehat q_1(k)\,dk\right].
$$

The printed plus sign would reconstruct $-q_z$. For a concrete nonzero example, $q(z)=-2\operatorname{Re}[(1+i)/(z+1+i)]$ is real, [harmonic](../../../partial-differential-equation.md#harmonic-function), smooth on the closed quadrant and decays along both axes. With $\beta_1=\beta_2=0$, it has $h_1(0)=h_2(0)=1$ and $q_z=(1+i)/(z+1+i)^2$. The printed orientation returns the negative of this [derivative](../../../calculus.md#derivative), so the issue persists even under the stated corner condition.

Let $a=\tfrac12e^{-i\beta_1-i\gamma}$. In the expressions from the preceding part, the coefficient of $\Phi$ on the imaginary ray is $a$, and the coefficient on the real ray is $-a e^{4i\gamma}$. For each of the three allowed sums, $e^{4i\gamma}=1$. The unknown part is therefore proportional to

$$
\int_0^{i\infty}e^{ikz}\Phi(k)\,dk-\int_0^\infty e^{ikz}\Phi(k)\,dk=0.
$$

Indeed, close the first spectral quadrant. For $z=x+iy$ with $x,y>0$, $|e^{ikz}|=e^{-(x\operatorname{Im}k+y\operatorname{Re}k)}$, so the large-arc contribution vanishes for bounded $\Phi$. The [Cauchy integral theorem](../../../complex-analysis.md#cauchy-s-integral-theorem) proves the equality and eliminates the single unknown [function](../../../function.md).

Substituting only the known pieces leaves

$$
q_z(z)=\frac1{2\pi}\left[
e^{i\beta_2}\int_0^\infty e^{ikz}H_2(k)\,dk
-e^{i\beta_2+i\gamma}\int_0^\infty e^{ikz}H_1(-k)\,dk
-e^{-i\beta_1}\int_0^{i\infty}e^{ikz}H_1(k)\,dk
+e^{-i\beta_1-i\gamma}\int_0^{i\infty}e^{ikz}H_2(-k)\,dk
\right].
$$

This already determines the answer from $h_1,h_2$ alone. Evaluating the elementary ray kernels gives the more direct [rational-angle oblique derivative problem on a quadrant](../../../differential-equation.md#rational-angle-oblique-derivative-problem-on-a-quadrant) formula

$$
\boxed{\begin{aligned}
q_z(z)=\frac{i}{2\pi}\bigg[
&e^{i\beta_2}\int_0^\infty\frac{h_2(x)}{z-x}\,dx
+e^{-i\beta_1-i\gamma}\int_0^\infty\frac{h_2(x)}{z+x}\,dx\\
&-e^{-i\beta_1}\int_0^\infty\frac{h_1(y)}{z-iy}\,dy
-e^{i\beta_2+i\gamma}\int_0^\infty\frac{h_1(y)}{z+iy}\,dy
\bigg].
\end{aligned}}
$$

No denominator vanishes for an interior point of the first quadrant.

For explicit formulas in the three cases, define

$$
I_2(z)=\int_0^\infty\frac{h_2(x)}{z^2-x^2}\,dx,\qquad
I_1(z)=\int_0^\infty\frac{h_1(y)}{z^2+y^2}\,dy,
$$



$$
K_2(z)=\int_0^\infty\frac{x h_2(x)}{z^2-x^2}\,dx,\qquad
K_1(z)=\int_0^\infty\frac{y h_1(y)}{z^2+y^2}\,dy.
$$

Combining the paired fractions and using $\beta_2=\gamma-\beta_1$ yields

$$
\boxed{q_z(z)=\frac{e^{-i\beta_1}}{\pi}
\begin{cases}
iz[I_2(z)-I_1(z)],&\gamma=0,\\
K_1(z)-K_2(z),&\gamma=\pi/2,\\
-iz[I_2(z)+I_1(z)],&\gamma=\pi.
\end{cases}}
$$

There is also a necessary [corner compatibility for collinear oblique derivative data](../../../differential-equation.md#corner-compatibility-for-collinear-oblique-derivative-data). When $\gamma=\pi/2$, the two prescribed [derivative](../../../calculus.md#derivative) directions are opposites, so a continuous corner [gradient](../../../calculus.md#gradient) requires $h_2(0)=-h_1(0)$. Together with the stipulated equality, this forces **$h_1(0)=h_2(0)=0$ in that case**. Existence was assumed, so admissible data must satisfy this additional consequence. Smoothness at the corner and decay at infinity also exclude the [homogeneous corner ambiguity in a quadrant Laplace problem](../../../differential-equation.md#homogeneous-corner-ambiguity-in-a-quadrant-laplace-problem); no extra singular or growing term is permitted in the boxed reconstruction.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)

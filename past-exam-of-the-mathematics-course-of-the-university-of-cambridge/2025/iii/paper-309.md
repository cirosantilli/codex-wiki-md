# Paper 309

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_309.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_309.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

In the [spherical coordinate system](../../../calculus.md#spherical-coordinate-system), $|d\mathbf x|^2=dr^2+r^2d\Omega_2^2$ and $\mathbf x\mathbin\cdot d\mathbf x=r\,dr$. Hence

$$
|d\mathbf x|^2-\frac{(\mathbf x\mathbin\cdot d\mathbf x)^2}{1+r^2}
=\left(1-\frac{r^2}{1+r^2}\right)dr^2+r^2d\Omega_2^2
=\frac{dr^2}{1+r^2}+r^2d\Omega_2^2.
$$

Thus the [static coordinates on anti-de Sitter spacetime](../../../general-relativity.md#static-coordinates-on-anti-de-sitter-spacetime) have

$$
\boxed{w(r)=1+r^2},
$$

which is positive for every $r\geq0$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Affinely parametrized [geodesics](../../../riemannian-geometry.md#geodesic) are the critical curves of the [geodesic Lagrangian](../../../riemannian-geometry.md#geodesic-lagrangian)

$$
L=\frac12\left[-w\dot t^2+\frac{\dot r^2}{w}
+r^2\dot\theta^2+r^2\sin^2\theta\,\dot\phi^2\right].
$$

For $w=1+r^2$ and $w'=2r$, the nonzero [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol), up to symmetry in the lower indices, are

$$
\Gamma^t{}_{tr}=\frac{w'}{2w}=\frac r w,
\quad
\Gamma^r{}_{tt}=\frac{ww'}2=rw,
\quad
\Gamma^r{}_{rr}=-\frac{w'}{2w}=-\frac r w,
$$



$$
\Gamma^r{}_{\theta\theta}=-rw,
\quad
\Gamma^r{}_{\phi\phi}=-rw\sin^2\theta,
\quad
\Gamma^\theta{}_{r\theta}=\Gamma^\phi{}_{r\phi}=\frac1r,
$$



$$
\Gamma^\theta{}_{\phi\phi}=-\sin\theta\cos\theta,
\qquad
\Gamma^\phi{}_{\theta\phi}=\cot\theta.
$$

They follow either from the Euler-Lagrange equations or directly from the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) formula.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The angular Euler-Lagrange equations are homogeneous in $\dot\theta$ and $\dot\phi$. Therefore initial data with both angular velocities zero give the unique solution with constant $\theta$ and $\phi$, so a radial geodesic remains radial.

Time-translation symmetry supplies the [geodesic conserved quantity from a Killing vector](../../../general-relativity.md#geodesic-conserved-quantity-from-a-killing-vector)

$$
e=w\dot t.
$$

Metric compatibility makes the squared tangent norm another constant,

$$
k=g(\dot\gamma,\dot\gamma)
=-w\dot t^2+\frac{\dot r^2}{w}
=\boxed{-\frac{e^2}{1+r^2}+\frac{\dot r^2}{1+r^2}}.
$$

For a proper-time parametrized timelike geodesic $k=-1$, for a null geodesic $k=0$, and for a unit-speed spacelike geodesic $k=1$. The constant $e$ is the conserved energy per unit mass associated with the static Killing vector $\partial_t$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Use proper time $s$, so $k=-1$. The first integral becomes

$$
\dot r^2=e^2-1-r^2=A^2-r^2,
\qquad A=\sqrt{e^2-1}.
$$

For an outward geodesic starting at the origin,

$$
r(s)=A\sin s
$$

until it next reaches $r=0$. This occurs at

$$
\boxed{T=\pi}.
$$

**Thus every [radial timelike geodesic in anti-de Sitter spacetime](../../../general-relativity.md#radial-timelike-geodesic-in-anti-de-sitter-spacetime) through the origin returns after the same proper time; restoring anti-de Sitter radius $a$ gives $T=\pi a$.**

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

For a radial [null geodesic](../../../special-relativity.md#null-geodesic), $k=0$ gives $\dot r^2=e^2$. Choose the affine parameter so that $r(0)=0$ and the outgoing branch has $\dot r=e>0$. Then

$$
r(\lambda)=e\lambda,
\qquad
\dot t=\frac e{1+r^2}.
$$

Using $dr/d\lambda=e$,

$$
t(\lambda)=\int_0^{r(\lambda)}\frac{dr}{1+r^2}
=\arctan r(\lambda).
$$

Consequently $r\to\infty$ while

$$
\boxed{t\longrightarrow\tau=\frac\pi2}.
$$

The conformal boundary is infinitely far away in affine parameter but is reached in finite static coordinate time.

## 2

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

Fix the convention

$$
(\nabla_c\nabla_d-\nabla_d\nabla_c)X^a
=R^a{}_{bcd}X^b.
$$

Although a single covariant derivative of a vector is tensorial, the second derivative contains connection-dependent terms. Their antisymmetric difference cancels every second derivative of a coordinate change. More intrinsically, the map

$$
R(U,V)X=\nabla_U\nabla_VX-\nabla_V\nabla_UX-\nabla_{[U,V]}X
$$

is $C^\infty(M)$-linear in each of $U,V,X$, so it defines the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor).

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Apply the definition to a coordinate-basis vector, use $[\partial_c,\partial_d]=0$, and collect the coefficient of $X^b$. This gives

$$
R^a{}_{bcd}
=\partial_c\Gamma^a{}_{db}-\partial_d\Gamma^a{}_{cb}
+\Gamma^a{}_{ce}\Gamma^e{}_{db}
-\Gamma^a{}_{de}\Gamma^e{}_{cb},
$$

up to the overall sign fixed in part i. The right side therefore transforms as a tensor even though its individual Christoffel-symbol terms do not. This identifies the displayed coordinate expression $K^a{}_{bcd}$ with $R^a{}_{bcd}$ after matching the paper's index and sign conventions.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

At an arbitrary point choose [normal coordinates](../../../general-relativity.md#normal-coordinates), so $\Gamma^a{}_{bc}=0$ there. Torsion freedom and commuting partial derivatives immediately give the algebraic [first Bianchi identity](../../../general-relativity.md#first-bianchi-identity)

$$
R^a{}_{[bcd]}=0.
$$

Differentiating the coordinate curvature formula at that point and cyclically antisymmetrizing gives the differential identity

$$
\nabla_{[e}R^a{}_{|b|cd]}=0.
$$

Both equations are tensorial, so validity in normal coordinates at every point proves them in every coordinate system.

Contract the differential identity on its first and third curvature indices and use the algebraic symmetries of the Riemann tensor. One obtains the [contracted Bianchi identity](../../../general-relativity.md#contracted-bianchi-identity)

$$
\boxed{\nabla_aR^a{}_b-\frac12\nabla_bR=0}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The left side of the stated identity must inherit $R_{abcd}=-R_{abdc}$. Exchange $c$ and $d$, reduce all curvature products using pair antisymmetry and the first Bianchi identity, and compare with the negative of the original expression. The unmatched mixed products cancel precisely for

$$
\boxed{\alpha=2}.
$$

This is the coefficient appearing in the [Penrose wave equation](../../../general-relativity.md#penrose-wave-equation) with the curvature convention of part a.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

The vacuum [Einstein field equations](../../../general-relativity.md#einstein-field-equations) imply $R_{ab}=0$ and hence $R=0$. Every term in the supplied general identity involving the Ricci tensor or its covariant derivatives therefore vanishes. Substituting $\alpha=2$ leaves

$$
\boxed{
\nabla^e\nabla_eR_{abcd}
+2R_a{}^e{}_c{}^fR_{bdef}
-2R_a{}^e{}_d{}^fR_{becf}
+R_{abef}R_{cd}{}^{ef}=0
}.
$$

This nonlinear, gauge-independent curvature equation is the [Penrose wave equation](../../../general-relativity.md#penrose-wave-equation).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

At $\epsilon=0$ the metric is the constant [Minkowski metric](../../../special-relativity.md#minkowski-metric), whose Christoffel symbols and curvature vanish, so

$$
R^{(0)}_{\mu\nu\rho\sigma}=0.
$$

Insert $R=\epsilon R^{(1)}+O(\epsilon^2)$ into the [Penrose wave equation](../../../general-relativity.md#penrose-wave-equation). Every curvature-square term is $O(\epsilon^2)$, while the covariant wave operator reduces at first order to the flat [d'Alembert operator](../../../wave-equation.md#d-alembert-operator). Thus

$$
\boxed{\partial^\alpha\partial_\alpha
R^{(1)}_{\mu\nu\rho\sigma}=0}.
$$

The [linearized Riemann curvature operator](../../../general-relativity.md#linearized-riemann-curvature-operator) is unchanged by $h_{\mu\nu}\mapsto h_{\mu\nu}+\partial_\mu\xi_\nu+\partial_\nu\xi_\mu$, because the resulting third derivatives cancel pairwise. The equation therefore requires no gauge choice for $h_{\mu\nu}$.

## 3

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Write $g_{\mu\nu}=\eta_{\mu\nu}+\epsilon h_{\mu\nu}$ and retain first-order terms. The quadratic Christoffel products in the supplied Ricci formula drop out. The wave-coordinate condition becomes the [Lorenz gauge in linearized gravity](../../../general-relativity.md#lorenz-gauge-in-linearized-gravity)

$$
\partial^\mu\bar h_{\mu\nu}=0,
\qquad
\bar h_{\mu\nu}=h_{\mu\nu}-\frac12\eta_{\mu\nu}h.
$$

The [linearized Ricci tensor and scalar](../../../general-relativity.md#linearized-ricci-tensor-and-scalar) then satisfy

$$
G^{(1)}_{\mu\nu}=-\frac12\mathop{\Box}\bar h_{\mu\nu}.
$$

Substitution into $G_{\mu\nu}=8\pi T_{\mu\nu}$ gives

$$
\boxed{\mathop{\Box}\bar h_{\mu\nu}=-16\pi T_{\mu\nu}},
\qquad
\boxed{\partial^\mu\bar h_{\mu\nu}=0}.
$$

If the paper denotes the trace-reversed variable itself by $h_{\mu\nu}$ in its displayed equation, this is exactly that convention.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Under $h'_{\mu\nu}=h_{\mu\nu}+\partial_\mu\xi_\nu+\partial_\nu\xi_\mu$, trace reversal gives

$$
\bar h'_{\mu\nu}=\bar h_{\mu\nu}
+\partial_\mu\xi_\nu+\partial_\nu\xi_\mu
-\eta_{\mu\nu}\partial_\rho\xi^\rho.
$$

Taking a divergence yields

$$
\partial^\mu\bar h'_{\mu\nu}
=\partial^\mu\bar h_{\mu\nu}+\mathop{\Box}\xi_\nu.
$$

Applying $\Box$ to the transformed field likewise produces only derivatives of $\Box\xi$. Therefore $\Box\xi^\mu=0$ preserves both the gauge condition and the sourced wave equation. These are the [residual gauge transformations](../../../general-relativity.md#residual-gauge-symmetry-of-linearized-gravity).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

Let $s=k_\rho x^\rho$. In vacuum,

$$
\mathop{\Box}\bar h_{\mu\nu}=k^2H''_{\mu\nu}(s),
\qquad
\partial^\mu\bar h_{\mu\nu}=k^\mu H'_{\mu\nu}(s).
$$

A nonzero localized profile cannot have $H''=0$, because an affine function does not decay at both ends. Hence

$$
\boxed{k^\mu k_\mu=0},
\qquad
\boxed{k^\mu H'_{\mu\nu}=0}.
$$

Decay removes the integration constant, so the second condition is equivalently $k^\mu H_{\mu\nu}=0$. Thus a nontrivial [plane gravitational wave in linearized gravity](../../../general-relativity.md#plane-gravitational-wave-in-linearized-gravity) has a null wavevector and transverse amplitude.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

A spatial rotation and rescaling put the future null vector in the form $k^\mu=(1,0,0,1)$, so the profile depends on $z-t$. Transversality gives four linear relations among the ten symmetric components. The four residual gauge functions satisfying $\Box\xi^\mu=0$ remove the time and longitudinal components; the remaining trace can be removed by the residual transformation indicated in the question. The resulting [transverse-traceless gauge](../../../general-relativity.md#transverse-traceless-gauge) is

$$
h_{\mu\nu}=
\begin{pmatrix}
0&0&0&0\\
0&f_+&f_\times&0\\
0&f_\times&-f_+&0\\
0&0&0&0
\end{pmatrix}(z-t).
$$

The two arbitrary functions are the plus and cross [gravitational-wave polarizations](../../../general-relativity.md#gravitational-wave-polarization). They are the two physical degrees of freedom left after the four gauge conditions and four residual coordinate freedoms are removed.

## 4

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For any differential form $\omega$, [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) gives

$$
\mathcal L_X\omega=d(\iota_X\omega)+\iota_X(d\omega).
$$

Using $d^2=0$,

$$
d\mathcal L_X\omega=d\iota_Xd\omega
=\mathcal L_Xd\omega.
$$

**Thus the [Lie derivative](../../../differential-form.md#lie-derivative-of-a-differential-form) commutes with the [exterior derivative](../../../differential-form.md#exterior-derivative) on every differential form.**

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Because the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) preserves the spacetime volume form, only derivatives of $X$ remain in $\mathcal L_XT$. Lower the raised indices in $T_{ab}{}^{cd}=\epsilon_{ab}{}^{cd}$, contract successively with the supplied products of two Levi-Civita tensors, and separate $\nabla_aX_b$ into antisymmetric, trace and symmetric trace-free parts. The antisymmetric part cancels automatically, while $\mathcal L_XT=0$ is equivalent to vanishing of the symmetric trace-free part:

$$
\nabla_{(a}X_{b)}-\frac14g_{ab}\nabla_cX^c=0.
$$

Therefore

$$
\boxed{\nabla_aX_b+\nabla_bX_a
=\frac12g_{ab}\nabla_cX^c},
$$

so $\boxed{\alpha=1/2}$. This is the four-dimensional [Conformal Killing equation](../../../general-relativity.md#conformal-killing-equation), and $X$ is a [Conformal Killing vector field](../../../general-relativity.md#conformal-killing-vector-field).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The first vacuum [Maxwell equations](../../../electromagnetism.md#maxwell-equations) equation is preserved for every vector field because part a gives

$$
d\widetilde F=d\mathcal L_XF=\mathcal L_X(dF)=0.
$$

On two-forms in four dimensions, the mixed volume tensor $T_{ab}{}^{cd}$ represents twice the [Hodge star operator](../../../differential-form.md#hodge-star-operator). Part b therefore says that a conformal Killing field commutes with the Hodge star:

$$
\mathcal L_X(\star F)=\star\mathcal L_XF.
$$

It follows that

$$
d(\star\widetilde F)
=d\mathcal L_X(\star F)
=\mathcal L_Xd(\star F)=0.
$$

**Hence $\widetilde F=\mathcal L_XF$ satisfies both vacuum Maxwell equations whenever $F$ does.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)

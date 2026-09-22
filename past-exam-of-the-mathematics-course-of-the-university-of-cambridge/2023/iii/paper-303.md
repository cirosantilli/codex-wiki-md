# Paper 303

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_303.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_303.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
    - [iii](#3/c/iii)
      - [Solution](#3/c/iii/solution)
    - [iv](#3/c/iv)
      - [Solution](#3/c/iv/solution)

## 1

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

[Landau theory](../../../critical-phenomenon.md#landau-theory) treats the [order parameter](../../../critical-phenomenon.md#order-parameter) as spatially uniform and expands the free-energy density in powers allowed by its symmetries. The [Landau-Ginzburg theory](../../../critical-phenomenon.md#landau-ginzburg-theory) promotes it to a field $\phi(\mathbf x)$ and adds gradient terms such as $|\nabla\phi|^2$. It therefore describes spatial fluctuations, interfaces, defects, and [correlation lengths](../../../critical-phenomenon.md#correlation-length), while reducing to Landau theory for uniform fields.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

For a real field, $\phi_{-\mathbf k}=\phi_{\mathbf k}^*$. The stated [Fourier transform](../../../analysis.md#fourier-transform) gives

$$
\nabla\phi(\mathbf x)=\int\frac{d^dk}{(2\pi)^d}\,i\mathbf k e^{i\mathbf k\cdot\mathbf x}\phi_{\mathbf k}.
$$

Using

$$
\int d^dx\,e^{i(\mathbf k+\mathbf q)\cdot\mathbf x}
=(2\pi)^d\delta^{(d)}(\mathbf k+\mathbf q)
$$

in both quadratic terms yields

$$
\boxed{F[\phi]
=\frac12\int\frac{d^dk}{(2\pi)^d}
(\gamma k^2+\mu^2)|\phi_{\mathbf k}|^2.}
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Write $A(k,T)=\gamma k^2+\mu^2(T)$ and use units with $k_B=1$. The [Gaussian functional integral](../../../quantum-field-theory.md#gaussian-functional-integral) gives the fluctuation free-energy density, up to terms linear in $T$ that do not affect the heat capacity,

$$
f(T)=\frac T2\int\frac{d^dk}{(2\pi)^d}
\log\frac{A(k,T)}T.
$$

Since the heat capacity per volume is $c=-T\,d^2f/dT^2$,

$$
c=\frac12\int\frac{d^dk}{(2\pi)^d}
\left[1-\frac{2T\dot\mu^2+T^2\ddot\mu^2}{\gamma k^2+\mu^2}
+\frac{T^2(\dot\mu^2)^2}{(\gamma k^2+\mu^2)^2}
\right],
$$

where a dot denotes $d/dT$. Thus

$$
g(T)=2T\frac{d\mu^2}{dT}+T^2\frac{d^2\mu^2}{dT^2},
\qquad
h(T)=T^2\left(\frac{d\mu^2}{dT}\right)^2.
$$

For $\mu^2=a(T-T_c)$, these reduce to $g(T)=2aT$ and $h(T)=a^2T^2$.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The most singular contribution as $\mu^2\downarrow0$ is

$$
\int\frac{d^dk}{(2\pi)^d}\frac1{(\gamma k^2+\mu^2)^2}.
$$

Rescaling $\mathbf k=(\mu/\sqrt\gamma)\mathbf q$ shows that its singular part is proportional to

$$
(\mu^2)^{d/2-2}.
$$

Because $\mu^2\propto T-T_c$, the [heat-capacity critical exponent](../../../critical-phenomenon.md#heat-capacity-critical-exponent) is

$$
\alpha=2-\frac d2=\frac{4-d}{2},
$$

for $d<4$. The term with one propagator is less singular. At $d=4$ the power is replaced by a logarithmic singularity, identifying four as the [upper critical dimension](../../../critical-phenomenon.md#upper-critical-dimension) of this Gaussian heat-capacity correction.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The stationary points obey

$$
f'(m)=m(2a_2+3a_3m+4a_4m^2)=0.
$$

Nonzero stationary points exist when

$$
9a_3^2-32a_2a_4\geq0,
$$

so they first appear at the ordered-phase [spinodal point](../../../critical-phenomenon.md#spinodal-point) $a_2=9a_3^2/(32a_4)$. The disordered state $m=0$ is locally stable for $a_2>0$ and loses that stability at $a_2=0$.

The actual phase boundary is found by requiring a nonzero stationary point $m_*$ to have the same free energy as $m=0$. Solving $f'(m_*)=0$ and $f(m_*)=0$ gives

$$
m_*=-\frac{a_3}{2a_4},
\qquad
a_2=\frac{a_3^2}{4a_4}.
$$

The disordered state is the global minimum for $a_2>a_3^2/(4a_4)$, the ordered state is the global minimum for $a_2<a_3^2/(4a_4)$, and they coexist at equality.

Since $a_3\ne0$, the order parameter jumps from zero to $-a_3/(2a_4)$ at coexistence. Hence this model has no [continuous phase transition](../../../critical-phenomenon.md#continuous-phase-transition) as the phases exchange stability, but it does have a [first-order phase transition](../../../thermodynamics.md#first-order-phase-transition) at the displayed positive value of $a_2$.

## 2

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A momentum-shell [renormalization group](../../../critical-phenomenon.md#renormalization-group) step has three parts:

1. Split the field into slow modes $\phi^-$ with $|k|<\Lambda/\zeta$ and fast modes $\phi^+$ with $\Lambda/\zeta<|k|<\Lambda$, then integrate out $\phi^+$ to obtain a [Wilsonian effective action](../../../perturbative-quantum-field-theory.md#wilsonian-effective-action) for $\phi^-$.  
2. Rescale momenta by $k'=\zeta k$, equivalently coordinates by $x'=x/\zeta$, so the reduced cutoff returns from $\Lambda/\zeta$ to $\Lambda$.  
3. Rescale the field, at the Gaussian fixed point by $\phi'(x')=\zeta^{(d-2)/2}\phi^-(x)$, so the coefficient of $(\nabla\phi)^2/2$ retains its chosen normalization.

The resulting functional has the original cutoff but changed coefficients. Iterating the operation gives a [renormalization-group flow](../../../critical-phenomenon.md#renormalization-group-flow) on masses and interaction couplings.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

At the Gaussian fixed point, the [engineering dimension](../../../critical-phenomenon.md#engineering-dimension) of the field is

$$
[\phi]=\frac{d-2}{2}.
$$

The operator $\phi^n(\nabla^2\phi)^m$ contains $n+m$ fields and $2m$ derivatives. Since its integral must be dimensionless,

$$
[g_{n,m}]
=d-\frac{(n+m)(d-2)}2-2m.
$$

It is marginal when this vanishes, namely

$$
d=\frac{2(n-m)}{n+m-2},
$$

when $n+m\ne2$. Since $n,m$ are positive, the exceptional case is $n=m=1$: $\phi\nabla^2\phi$ has a dimensionless coupling in every $d$ and differs from the kinetic term by integration by parts. If the displayed formula gives no positive $d$, there is no positive spatial dimension in which that operator is naively marginal.

At an interacting fixed point, field and composite operators acquire [anomalous dimensions](../../../critical-phenomenon.md#anomalous-dimension), and operators with the same symmetries can mix under renormalization. Their full [scaling dimensions](../../../string-theory.md#scaling-dimension) can therefore differ from these naive engineering dimensions.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

Use two external slow-field legs and internal fast-mode propagators. Through the requested orders, the connected mass-correction topologies are:

- order $g_0$: one quartic vertex with one fast tadpole;
- order $g_0^2$: two quartic vertices joined either by three fast lines, or by two fast lines with a fast tadpole on the vertex carrying no external legs;
- order $\lambda_0$: one sextic vertex with two fast tadpole loops;
- order $\lambda_0g_0$: a sextic and a quartic vertex joined by two fast lines, with the remaining fast legs closed into tadpoles in the two possible external-leg placements; joined by four fast lines with two external legs on the sextic vertex; or joined by three fast lines with one sextic tadpole and one external leg on each vertex.

A nominal one-line bridge at order $\lambda_0g_0$ vanishes in a sharp momentum-shell scheme at small external momentum because that line would have to carry momentum outside the fast shell. These descriptions specify the same diagrams without depending on a particular drawing convention for vertices and external legs.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

Write

$$
I_j=\int_{\Lambda/\zeta<|k|<\Lambda}
\frac{d^dk}{(2\pi)^d}\,G_0(k)^j,
\qquad
G_0(k)=\frac1{k^2+\mu_0^2},
$$

and, for the three-line topology,

$$
J_3=\int_+\frac{d^dk\,d^dq}{(2\pi)^{2d}}
G_0(k)G_0(q)G_0(k+q),
$$

and define the four-line integral

$$
J_4=\int_+\frac{d^dk\,d^dq\,d^d\ell}{(2\pi)^{3d}}
G_0(k)G_0(q)G_0(\ell)G_0(k+q+\ell),
$$

with every propagator momentum restricted to the fast shell.

The first cumulant contains

$$
\lambda_0\binom62\langle(\phi^+)^4\rangle_+(\phi^-)^2
=45\lambda_0 I_1^2(\phi^-)^2.
$$

Since the quadratic free energy is $\frac12\mu^2(\phi^-)^2$, this gives

$$
\delta\mu^2\big|_{\lambda_0}=90\lambda_0I_1^2.
$$

The mixed term in the second cumulant is

$$
-\left(\langle V_6V_4\rangle_+
-\langle V_6\rangle_+\langle V_4\rangle_+\right).
$$

Wick contraction with the printed normalization $V_6=\lambda_0\int\phi^6$ and $V_4=g_0\int\phi^4$ gives, at zero external momentum,

$$
\delta\mu^2\big|_{\lambda_0g_0}
=-2\lambda_0g_0
\left(1620I_1^2I_2+1440I_1J_3+360J_4\right).
$$

The coefficients respectively combine the two placements of both external legs in the two-line topology, the three-line topology with one external leg on each vertex, and the four-line topology. Couplings normalized as $g_0\phi^4/4!$ and $\lambda_0\phi^6/6!$ absorb the corresponding factorials, which is why formulas in that convention have much smaller numerical coefficients.

## 3

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a uniform field with $r^2=\boldsymbol\phi\mathbin\cdot\boldsymbol\phi$, the potential is

$$
V(r)=\frac12\mu^2r^2+gr^4.
$$

For $T>T_c$, one has $\mu^2>0$, so $\boldsymbol\phi_0=0$. The Hessian has $N$ positive equal eigenvalues, and all $N$ modes are gapped. The full $O(N)$ symmetry is unbroken.

For $T<T_c$, one has $\mu^2<0$, and

$$
|\boldsymbol\phi_0|^2=-\frac{\mu^2}{4g}.
$$

The vacuum manifold is $S^{N-1}$. Choosing one point breaks $O(N)$ spontaneously to $O(N-1)$. The radial fluctuation has squared mass $-2\mu^2$, while the $N-1$ tangent directions are gapless [Nambu-Goldstone bosons](../../../critical-phenomenon.md#goldstone-boson), one for each broken continuous generator modulo the unbroken subgroup.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For the $O(2)$ model write

$$
\boldsymbol\phi=(v+\rho)(\cos\theta,\sin\theta),
\qquad
v^2=-\frac{\mu^2}{4g}.
$$

At long distances the massive radial field $\rho$ can be neglected, leaving the [Goldstone-mode effective free energy](../../../critical-phenomenon.md#goldstone-mode-effective-free-energy)

$$
F_\theta=\frac{\gamma v^2}{2}\int d^dx\,(\nabla\theta)^2.
$$

Therefore

$$
\langle\theta(\mathbf x)\theta(\mathbf y)\rangle
=\frac1{\gamma v^2}\int\frac{d^dk}{(2\pi)^d}
\frac{e^{-i\mathbf k\cdot(\mathbf x-\mathbf y)}}{k^2}.
$$

The mode is massless, so its [correlation length](../../../critical-phenomenon.md#correlation-length) is infinite. For $d>2$ its large-distance Green function is

$$
\langle\theta(\mathbf x)\theta(\mathbf y)\rangle
\sim\frac{\Gamma(d/2-1)}{4\pi^{d/2}\gamma v^2}\,r^{2-d}.
$$

For $d=2$ it is $-(2\pi\gamma v^2)^{-1}\log(r/a)$ up to an infrared-dependent constant, and in $d=1$ it is $-|r|/(2\gamma v^2)$ up to such a constant.

The invariant diagnostic is the [phase-difference variance](../../../critical-phenomenon.md#phase-difference-variance)

$$
\langle[\theta(\mathbf r)-\theta(0)]^2\rangle
=\frac2{\gamma v^2}\int\frac{d^dk}{(2\pi)^d}
\frac{1-\cos(\mathbf k\cdot\mathbf r)}{k^2}.
$$

It diverges linearly in $d=1$ and logarithmically in $d=2$, destroying true long-range order, but approaches a finite infrared limit for $d=3,4$. Thus the continuous-symmetry ordered phase exists for $d=3,4$ and not for $d=1,2$, in agreement with the [Mermin-Wagner theorem](../../../critical-phenomenon.md#mermin-wagner-theorem). The lower critical dimension is $d_{\mathrm{lc}}=2$; the two-dimensional $O(2)$ model can instead show [quasi-long-range order below a BKT transition](../../../critical-phenomenon.md#berezinskii-kosterlitz-thouless-transition).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For generic $\mu^2\ne\lambda^2$, the symmetry is $O(1)\times O(2)$: an independent sign flip of $\phi_1$ and orthogonal transformations of $(\phi_2,\phi_3)$. When $\mu^2=\lambda^2$, it is enhanced to $O(3)$.

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

If $\mu^2,\lambda^2>0$, the unique ground state is $\boldsymbol\phi_0=0$. The full $O(1)\times O(2)$ symmetry remains unbroken and every mode is gapped.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

If $\mu^2<0$ and $\lambda^2>0$, the minima are

$$
\boldsymbol\phi_0=(\pm v_1,0,0),
\qquad
v_1^2=-\frac{\mu^2}{4g}.
$$

The discrete $O(1)\cong\mathbb Z_2$ symmetry is spontaneously broken, while $O(2)$ remains intact. There is no Goldstone mode because only a discrete symmetry is broken.

<h4 id="3/c/iii">iii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/c/iii)

If $\mu^2>0$ and $\lambda^2<0$, the minima are

$$
\phi_{01}=0,
\qquad
\phi_{02}^2+\phi_{03}^2=-\frac{\lambda^2}{4g}.
$$

The $O(1)$ factor remains unbroken, while $O(2)$ is spontaneously broken to the $O(1)$ subgroup that fixes a chosen point on the circle. The one-dimensional vacuum circle gives one Goldstone mode.

<h4 id="3/c/iv">iv</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/c/iv)

If $\mu^2=\lambda^2<0$, the enhanced $O(3)$-symmetric potential has the sphere of minima

$$
|\boldsymbol\phi_0|^2=-\frac{\mu^2}{4g}.
$$

Choosing a ground state breaks $O(3)$ to $O(2)$. The vacuum manifold $O(3)/O(2)\simeq S^2$ has dimension two, so there are two Goldstone modes.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)

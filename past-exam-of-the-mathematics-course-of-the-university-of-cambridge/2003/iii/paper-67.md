# Paper 67

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper67.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper67.pdf)

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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
- [6](#6)
  - [Solution](#6/solution)
- [7](#7)
  - [Solution](#7/solution)

## 1

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Introduce one stage $k=f(t_n+h/2,Y)$ with $Y=y_n+hk/2$, and update $y_{n+1}=y_n+hk$. This is the [implicit midpoint rule](../../../numerical-analysis.md#implicit-midpoint-rule) as a one-stage [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method), with [Butcher tableau](../../../numerical-analysis.md#butcher-tableau)

$$
\begin{array}{c|c}1/2&1/2\\\hline&1\end{array}.
$$

For a smooth vector field, write $\Delta=y_{n+1}-y_n$. Expanding its stage equation gives

$$
\Delta=hf(t_n,y_n)+\frac{h^2}{2}\bigl(f_t+f_yf\bigr)(t_n,y_n)+O(h^3),
$$

which matches the exact [Taylor expansion](../../../calculus.md#taylor-expansion) through degree two. The method therefore has order at least two. On the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation) $y'=\lambda y$, its [stability function](../../../numerical-analysis.md#stability-function) is

$$
R(z)=\frac{1+z/2}{1-z/2}=1+z+\frac{z^2}{2}+\frac{z^3}{4}+O(z^4),\qquad z=h\lambda.
$$

The third coefficient differs from the exponential's $1/6$, so the order is exactly two.

There is no pole in $\operatorname{Re}z\leq0$, and

$$
|1-z/2|^2-|1+z/2|^2=-2\operatorname{Re}z\geq0.
$$

Thus $|R(z)|\leq1$ throughout the closed left half-plane:

$$
\boxed{\text{one-stage implicit Runge-Kutta; order }2;\quad\text{A-stable}.}
$$

This conclusion is [A-stability](../../../numerical-analysis.md#a-stability), not strong damping of arbitrarily stiff modes: $R(z)\to-1$ along the negative real axis.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $Q(y)=y^TSy$. In the usual pointwise meaning of an [ODE invariant](../../../differential-equation.md#first-integral-of-an-ordinary-differential-equation), differentiation along an exact solution through an arbitrary state gives

$$
\frac d{dt}Q(y(t))=2y^TSf(t,y)=0.
$$

For a nonautonomous equation this identity must hold at the stage time as well as at the initial time. It follows directly from invariance for solutions started at any time and state, or from the stated initial-time invariance when the exact flow onto the stage-time domain is invertible. This is the first-integral condition used below.

Put $Y=(y_n+y_{n+1})/2$ and $t_*=t_n+h/2$. Since $S$ is symmetric,

$$
Q(y_{n+1})-Q(y_n)
=(y_{n+1}+y_n)^TS(y_{n+1}-y_n)
=2hY^TSf(t_*,Y)=0.
$$

Induction over all well-defined implicit steps gives

$$
\boxed{y_n^TSy_n=y_0^TSy_0.}
$$

No positive-definiteness assumption on $S$ was used. Nor is uniqueness of the stage essential to this algebraic identity: any stage solution satisfying the method and the pointwise invariant condition preserves $Q$. This is the one-stage case of [Runge-Kutta conservation of quadratic invariants](../../../numerical-analysis.md#runge-kutta-conservation-of-quadratic-invariants).

## 2

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use the coefficient $2-\alpha$ in the numerator, as verified in the PDF; the converted TeX lost its $-\alpha$. Multiplying the method by $2+\alpha$ gives the [characteristic polynomials of a linear multistep method](../../../numerical-analysis.md#characteristic-polynomials-of-a-linear-multistep-method)

$$
\rho(\zeta)=(2+\alpha)\zeta^2-4\zeta+(2-\alpha),\qquad
\sigma(\zeta)=\zeta^2+2\alpha\zeta-1.
$$

For every admissible real $\alpha$, $\rho(1)=0$ and $\rho'(1)=2\alpha=\sigma(1)$, giving [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method). Factorization gives

$$
\rho(\zeta)=(\zeta-1)\bigl((2+\alpha)\zeta-(2-\alpha)\bigr).
$$

The second root is $r=(2-\alpha)/(2+\alpha)$. The [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) requires $|r|\leq1$ and forbids a repeated root at one. For real $\alpha\ne-2$,

$$
|r|\leq1\iff(2-\alpha)^2\leq(2+\alpha)^2\iff\alpha\geq0.
$$

At $\alpha=0$ both roots equal one, violating [zero-stability](../../../numerical-analysis.md#zero-stability). For $\alpha>0$ the second root lies strictly inside the unit disk. The [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem) therefore gives

$$
\boxed{\text{convergence exactly for }\alpha>0.}
$$

To find the order rather than only consistency, expand the exact-solution residual through the generating function:

$$
\rho(e^z)-z\sigma(e^z)
=\frac\alpha3z^3+\left(\frac\alpha3-\frac16\right)z^4+O(z^5).
$$

Thus its unnormalized [local truncation error](../../../numerical-analysis.md#local-truncation-error) begins with $(\alpha/3)h^3y^{(3)}$ when $\alpha>0$, and the global method order is exactly two for every convergent parameter. For comparison, $\alpha=0$ has formal order three but is not convergent because of its double unit root:

$$
\boxed{p=2\quad\text{for every }\alpha>0.}
$$

These orders assume a smooth solution, the usual local Lipschitz condition and starting approximations of the required accuracy.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Only $\alpha>0$ needs consideration, by the preceding [zero-stability](../../../numerical-analysis.md#zero-stability) analysis. On the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation), all roots of the [amplification polynomial](../../../numerical-analysis.md#amplification-polynomial-of-a-multistep-method)

$$
P_z(\zeta)=\rho(\zeta)-z\sigma(\zeta)
$$

must satisfy the unit-disk root condition if the method is [A-stable](../../../numerical-analysis.md#a-stability). Evaluate it at $\zeta=-1$:

$$
P_z(-1)=8+2\alpha z.
$$

Take a real negative $z<-4/\alpha$. Then $P_z(-1)<0$, whereas the leading coefficient $2+\alpha-z$ is positive and $P_z(\zeta)\to+\infty$ as $\zeta\to-\infty$. The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) gives a real root strictly below $-1$. Its numerical mode grows in modulus, contradicting [absolute stability](../../../numerical-analysis.md#linear-stability-domain) at this negative test parameter. Consequently

$$
\boxed{\text{no parameter gives both convergence and A-stability}.}
$$

This proof detects an unstable root directly; the second-order value alone would not exclude [A-stability](../../../numerical-analysis.md#a-stability). Equivalently the limiting derivative polynomial has an exterior root $-\alpha-\sqrt{1+\alpha^2}$, explaining the instability for large negative $z$.

## 3

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

There is a genuine indexing defect in the printed PDF: its new value is at $m+1$, while every old-time coefficient is centered at $m$. On a fixed grid the literal residual contains

$$
\frac{u(x+\delta,t+k)-u(x,t)}k-L_\delta u(x,t)
=\frac\delta k u_x+O(1)+O(k)+O(\delta^2),\qquad k=\mu\delta^2.
$$

For a general solution the leading term is $u_x/(\mu\delta)$, so this is not a consistent diffusion discretization. It also leaves one new interior value unspecified while imposing a generally incompatible update on a prescribed boundary value. The calculation that follows is for the intended same-node update $U_m^{n+1}=U_m^n+kL_\delta U_m^n$; that correction is necessary, not an unnoticed transcription change.

For the [midpoint flux stencil for one-dimensional diffusion](../../../finite-difference.md#midpoint-flux-stencil-for-one-dimensional-diffusion), define

$$
L_\delta u(x)=\frac{a(x-\delta/2)[u(x-\delta)-u(x)]+a(x+\delta/2)[u(x+\delta)-u(x)]}{\delta^2}.
$$

Assume sufficient smoothness of $a$ and the solution for the displayed remainders. Multiplying the centered [Taylor expansions](../../../calculus.md#taylor-expansion) of $a$ and $u$ gives

$$
L_\delta u=(au_x)_x+\delta^2\left(\frac{a u_{xxxx}}{12}+\frac{a'u_{xxx}}6+\frac{a''u_{xx}}8+\frac{a^{(3)}u_x}{24}\right)+O(\delta^4).
$$

The first time difference is $(u(t+k)-u(t))/k=u_t+ku_{tt}/2+O(k^2)$. After using the [diffusion equation](../../../diffusion-equation.md), the [normalized local truncation error](../../../numerical-analysis.md#normalized-local-truncation-error) is

$$
\tau_m^n=\frac{k}{2}u_{tt}-\delta^2\left(\frac{a u_{xxxx}}{12}+\frac{a'u_{xxx}}6+\frac{a''u_{xx}}8+\frac{a^{(3)}u_x}{24}\right)+O(k^2+\delta^4).
$$

Therefore, for the corrected update,

$$
\boxed{\tau=O(k+\delta^2),\qquad d=k\tau=O(k^2+k\delta^2).}
$$

The first is the residual divided by the time step; the second is the unnormalized one-step defect. At fixed $\mu=k/\delta^2$ they are respectively $O(\delta^2)$ and $O(\delta^4)$. A rate based on derivatives is not justified for a merely bounded nonsmooth $a$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use the corrected same-node method identified above, with $\delta=1/M$, interior indices $1,\ldots,M-1$ and zero endpoint values. Its spatial [matrix](../../../vector-space.md#matrix) $L_\delta$ is real symmetric. Summation by parts gives, for a vector extended by zero at the endpoints,

$$
-v^TL_\delta v=\delta^{-2}\sum_{j=0}^{M-1}a_{j+1/2}(v_{j+1}-v_j)^2.
$$

Hence $-L_\delta$ is positive definite, and $\sum_j(v_{j+1}-v_j)^2\leq4\sum_jv_j^2$ bounds its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) by $4a_+/\delta^2$. The [Forward Euler method](../../../numerical-analysis.md#euler-method) has amplification [matrix](../../../vector-space.md#matrix) $I+kL_\delta$. Its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) lie in $[1-4\mu a_+,1]$, so their moduli are at most one when

$$
\boxed{0<\mu\leq\frac1{2a_+}.}
$$

Symmetry makes this a contraction in the mesh-weighted [discrete L2 norm](../../../functional-analysis.md#discrete-l2-norm), uniformly over all grids and all coefficient samples satisfying the bounds. There is also a [maximum norm](../../../functional-analysis.md#supremum-norm) proof: the update weights are $\mu a_{m-1/2}$, $1-\mu(a_{m-1/2}+a_{m+1/2})$, and $\mu a_{m+1/2}$. They are nonnegative and sum to one, giving a contraction after the boundary values are included.

This mesh-independent bound is sharp. For $a\equiv a_+$, the spatial eigenvectors are $\sin(j\pi m/M)$ and their amplification factors are

$$
1-4\mu a_+\sin^2\frac{j\pi}{2M},\qquad j=1,\ldots,M-1.
$$

If $\mu>1/(2a_+)$, sufficiently fine grids have a highest-frequency factor below $-1$, giving exponential growth in the step number.

On one fixed grid, rather than uniformly under refinement, the sharp universal [stability of a numerical method](../../../numerical-analysis.md#stability-of-a-numerical-method) bound in the [discrete L2 norm](../../../functional-analysis.md#discrete-l2-norm) is slightly larger:

$$
\mu\leq\frac1{2a_+\cos^2(\pi/(2M))}.
$$

Indeed the quadratic form above is bounded by $a_+$ times the constant-coefficient difference form, whose largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is $4\cos^2(\pi/(2M))/\delta^2$; equality is realized by the constant coefficient. Its limit as $M\to\infty$ is the boxed bound. No such fixed-grid [matrix](../../../vector-space.md#matrix) conclusion repairs the ill-defined shifted-boundary update in the literal printed formula.

## 4

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Put $\nu=k/\delta$ and use the [discrete Fourier transform](../../../numerical-analysis.md#discrete-fourier-transform) on the infinite grid. A spatial [Fourier mode](../../../fourier-analysis.md#fourier-mode) $e^{i(j\theta+\ell\phi)}$ has time coefficient satisfying

$$
v_{n+1}=2is\,v_n+v_{n-1},\qquad s=\nu(\sin\theta+\sin\phi).
$$

Its [amplification polynomial of a multilevel finite difference scheme](../../../finite-difference.md#amplification-polynomial-of-a-multilevel-finite-difference-scheme) is $\zeta^2-2is\zeta-1$, with roots

$$
\zeta_\pm=is\pm\sqrt{1-s^2}.
$$

For $|s|<1$ they are distinct and have modulus one. Since $|s|\leq2\nu$, a fixed $0<\nu<1/2$ bounds their separation below by $2\sqrt{1-4\nu^2}$. Solving for the two mode amplitudes therefore bounds every power of the two-level [companion matrix](../../../linear-operator-theory.md#companion-matrix) uniformly in frequency and step number. [Parseval identity](../../../fourier-analysis.md#parseval-identity) transfers this bound to the [discrete L2 norm](../../../functional-analysis.md#discrete-l2-norm).

If $\nu>1/2$, an open set of frequencies around $(\pi/2,\pi/2)$ has $|s|>1$ and a root of modulus greater than one. Fourier data supported there grow exponentially. At $\nu=1/2$, the central frequency has the double root $i$, and the recurrence admits $v_n=(A+Bn)i^n$. Thus the root moduli being one do not suffice: a nontrivial [Jordan block](../../../linear-operator-theory.md#jordan-block) makes the two-level powers grow linearly. Although this exact frequency has measure zero on the infinite grid, the [matrices](../../../vector-space.md#matrix) depend continuously on frequency. For every step count, a neighborhood has powers nearly as large, so their essential supremum is still unbounded. Wave packets in those neighborhoods rule out a uniform [stability of a numerical method](../../../numerical-analysis.md#stability-of-a-numerical-method) estimate in the [discrete L2 norm](../../../functional-analysis.md#discrete-l2-norm).

For arbitrary perturbations in both starting levels the sharp positive range is therefore

$$
\boxed{0<\Delta t/\Delta x<1/2.}
$$

The zero-step limiting recurrence is bounded but does not advance time. A specially filtered startup can suppress a repeated-root mode; that restriction does not establish stability of the full two-level scheme. This is the [two-dimensional leapfrog stability threshold](../../../finite-difference.md#two-dimensional-leapfrog-stability-threshold).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Divide the recurrence by $2k$ and substitute a smooth exact solution. Centered [Taylor expansions](../../../calculus.md#taylor-expansion) in time and space give

$$
\frac{u(t+k)-u(t-k)}{2k}-\frac{u(x+\delta,y)-u(x-\delta,y)+u(x,y+\delta)-u(x,y-\delta)}{2\delta}
=\frac{k^2}{6}u_{ttt}-\frac{\delta^2}{6}(u_{xxx}+u_{yyy})+O(k^4+\delta^4).
$$

Thus the [leapfrog advection scheme](../../../finite-difference.md#leapfrog-advection-scheme) is consistent with normalized residual $O(k^2+\delta^2)$. Its unnormalized defect is $O(k^3+k\delta^2)$. For a fixed $0<\nu<1/2$, the uniform two-level bound proved above and accumulation over $O(1/k)$ steps yield, for a sufficiently smooth solution,

$$
\max_{nk\leq T}\|e^n\|_{2,\delta}\leq C_{T,\nu}\bigl(\|e^0\|_{2,\delta}+\|e^1\|_{2,\delta}+k^2+\delta^2\bigr).
$$

Both starting levels must be supplied consistently; errors of order $k^2+\delta^2$ give second-order convergence. For general [square-integrable functions](../../../measure-theory.md#square-integrable-function) as initial data, point sampling is not defined on equivalence classes. Use cell averages or another bounded grid projection, together with a bounded consistent startup. Approximate the initial data by smooth functions, apply the smooth-data convergence estimate, and use the uniform numerical and exact translation bounds to pass to the [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) limit. This is the content of [Lax equivalence theorem](../../../finite-difference.md#lax-equivalence-theorem) in the present setting.

At $\nu>1/2$ the growing [Fourier mode](../../../fourier-analysis.md#fourier-mode) prevents general convergence. At the endpoint, initial data supported in increasingly narrow neighborhoods of the double root can have a second-level error of norm $O(k)$ but a final error of order one after $O(1/k)$ steps. These are vanishing starting errors, so the endpoint fails general two-level convergence as well. Consequently

$$
\boxed{0<\Delta t/\Delta x<1/2}
$$

is also the general convergence range, with a consistent stable initialization. Claims for a particular specially chosen endpoint startup would be a different, restricted assertion.

## 5

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Assume $n\geq3$ and use periodic indices for the [Jacobi method](../../../numerical-analysis.md#jacobi-method). At iteration $r$, it is

$$
\boxed{x_j^{(r+1)}=\tfrac12\bigl(x_{j-1}^{(r)}+x_{j+1}^{(r)}-b_j\bigr),\qquad x_0=x_n,\quad x_{n+1}=x_1.}
$$

All values on its right side belong to the old iterate. For lexicographic [Gauss-Seidel iteration](../../../numerical-analysis.md#gauss-seidel-method), compute in the order $1,\ldots,n$ and use a newly available coordinate immediately:

$$
\begin{aligned}
x_1^{(r+1)}&=\tfrac12(x_2^{(r)}+x_n^{(r)}-b_1),\\
x_j^{(r+1)}&=\tfrac12(x_{j-1}^{(r+1)}+x_{j+1}^{(r)}-b_j),\quad 2\leq j\leq n-1,\\
x_n^{(r+1)}&=\tfrac12(x_1^{(r+1)}+x_{n-1}^{(r+1)}-b_n).
\end{aligned}
$$

The wrap-around term in the last row uses the new $x_1$, while the wrap-around term in the first row uses the old $x_n$. This is important for the actual [iteration matrix](../../../numerical-analysis.md#iteration-matrix) and its convergence behavior.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The [circulant matrix](../../../linear-algebra.md#circulant-matrix) is singular, so the meaning of convergence needs care. If $C$ is the cyclic shift, $A=C+C^{-1}-2I$ has Fourier [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $-4\sin^2(\pi j/n)$. Its [null space](../../../linear-algebra.md#kernel-of-a-linear-map) consists of constants. Therefore $Ax=b$ is solvable exactly when $\sum_jb_j=0$, and any solution is determined only up to a constant. Neither iteration can converge to a unique solution for arbitrary right-hand sides.

For a compatible $b$, fix one solution $x_*$ and examine the error. The [iteration matrix](../../../numerical-analysis.md#iteration-matrix) of the [Jacobi method](../../../numerical-analysis.md#jacobi-method) is $(C+C^{-1})/2$, with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\cos(2\pi j/n)$. The constant mode has [eigenvalue](../../../linear-operator-theory.md#eigenvalue) one. For odd $n$ all other [eigenvalues](../../../linear-operator-theory.md#eigenvalue) have modulus less than one, so the iterates converge to $x_*+c\mathbf1$, with the constant selected by the initial mean. For even $n$, the alternating vector has [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $-1$, producing an undamped oscillation. With $b=0$ and alternating initial vector this is an explicit nonconvergent example. For even $n$ convergence occurs only when that error component vanishes. When $\sum b_j\ne0$, the mean instead drifts by $-(\sum b_j)/(2n)$ at each step, so Jacobi cannot converge.

For [Gauss-Seidel iteration](../../../numerical-analysis.md#gauss-seidel-method), put $K=-A=D+L+U$, so $K$ is positive semidefinite with diagonal two. The homogeneous error iteration is $e^+=Be$, $B=-(D+L)^{-1}U$. Updating a coordinate exactly minimizes $E(e)=e^TKe/2$ in that coordinate; completing the square gives an energy decrement $|\Delta e_j|^2$. Summing within a sweep gives

$$
E(e)-E(Be)=\sum_{j=1}^n|\Delta e_j|^2\geq0.
$$

The same identity holds for the Hermitian energy of complex vectors. If $Be=\lambda e$ and $e$ is nonconstant, its energy is positive, so $|\lambda|\leq1$. Equality forces every update to be zero, whence $Ke=0$ and $e$ is constant, a contradiction. Thus all nonconstant eigenmodes have modulus strictly below one.

The [eigenvalue](../../../linear-operator-theory.md#eigenvalue) one has only the constant [eigenspace](../../../linear-operator-theory.md#eigenspace). To exclude a generalized eigenvector at one, observe that

$$
w=(D+L)^T\mathbf1=(0,1,\ldots,1,2)^T,\qquad w^TB=w^T,\quad w^T\mathbf1=n.
$$

If $(B-I)v=\mathbf1$, multiplication by $w^T$ would give $0=n$. Hence the constant [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is algebraically simple, and

$$
B^r\longrightarrow\mathbf1w^T/n.
$$

For compatible $b$, Gauss-Seidel therefore converges from every start to some solution, for either parity of $n$. Its limit differs from $x_*$ by $\mathbf1w^T(x^{(0)}-x_*)/n$. For an incompatible $b$, the affine update gives $w^Tx^{(r+1)}-w^Tx^{(r)}=-\sum_jb_j$, so the iterates again cannot converge.

Thus [semiconvergence of cyclic Poisson iterations](../../../numerical-analysis.md#semiconvergence-of-cyclic-poisson-iterations) gives the precise answer:

$$
\boxed{\begin{array}{l}
\sum b_j\ne0:\ \text{neither iteration converges};\\
\sum b_j=0:\ \text{Gauss-Seidel converges to a solution for all }n;\\
\text{Jacobi converges from every start iff }n\text{ is odd}.
\end{array}}
$$

Both have spectral radius one on the unrestricted space, so neither meets the strict stationary-iteration criterion for a unique limit independent of the starting constant. A spectral radius of one alone is not a proof that Gauss-Seidel's compatible iterates fail to converge. A normalization or projection removing the constant mode makes this distinction explicit.

## 6

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Consider $-\Delta u=f$ on a rectangle, with prescribed [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition), and assume initially that the solution is smooth up to the boundary. A [finite difference method](../../../finite-difference.md#finite-difference-method) chooses grid values as unknowns, approximates the differential operator by a local stencil, incorporates the boundary data, and solves the resulting sparse [linear system](../../../linear-algebra.md#system-of-linear-equations). Accuracy of a stencil by itself is insufficient: one also needs a well-posed discrete problem, a stability estimate uniform under refinement, and a sufficiently accurate algebraic solve.

For a square grid of spacing $h$, centered second differences give the [five-point Laplacian](../../../finite-difference.md#five-point-laplacian)

$$
D_5U_{ij}=\frac{U_{i+1,j}+U_{i-1,j}+U_{i,j+1}+U_{i,j-1}-4U_{ij}}{h^2}.
$$

Expanding each opposite pair in a [Taylor series](../../../calculus.md#taylor-series) gives

$$
D_5u=\Delta u+\frac{h^2}{12}(u_{xxxx}+u_{yyyy})+O(h^4).
$$

Thus the standard equation $-D_5U=f$ has second-order normalized [local truncation error](../../../numerical-analysis.md#local-truncation-error). Known boundary values move to the right-hand side; they are not iterated as independent unknowns. Nonrectangular geometry requires a consistent boundary approximation rather than silently retaining a full interior stencil outside the domain.

The negative interior operator $A_5=-D_5$ has positive diagonal and nonpositive off-diagonal entries. For a grid vector extended by zero on the boundary,

$$
v^TA_5v=h^{-2}\sum_{\text{grid edges}}(v_i-v_j)^2>0\quad(v\ne0).
$$

The edge sum includes links to the fixed boundary. Connectivity makes the [matrix](../../../vector-space.md#matrix) positive definite, proving uniqueness and providing an energy structure. The same sign pattern gives a [discrete maximum principle](../../../finite-difference.md#discrete-maximum-principle): at a negative interior minimum, $A_5v$ is nonpositive. If $A_5v\geq0$ and the boundary is nonnegative, equality can only persist by propagating that minimum through all neighbors to the boundary, a contradiction. Therefore $v\geq0$.

On the unit square, the barrier $b(x,y)=[x(1-x)+y(1-y)]/4$ satisfies $A_5b=1$ exactly. If $e$ has zero boundary values and $A_5e=r$, apply the maximum principle to $\|r\|_\infty b\pm e$ to obtain

$$
\|e\|_\infty\leq\tfrac18\|r\|_\infty.
$$

The bound is independent of $h$, so the $O(h^2)$ consistency error gives an $O(h^2)$ nodal error. It also separates the algebraic residual from the discretization error: solving the [linear system](../../../linear-algebra.md#system-of-linear-equations) much less accurately than $h^2$ would spoil the spatial accuracy.

A direct higher-order design is possible. In one coordinate,

$$
u_{xx}(x)\approx\frac{-u(x+2h)+16u(x+h)-30u(x)+16u(x-h)-u(x-2h)}{12h^2}
$$

has fourth-order accuracy. Adding the corresponding formula in the other coordinate gives a wider stencil. Its advantages must be balanced against boundary closures, more distant couplings, and the possible loss of monotonicity. Higher order does not automatically imply a stable or geometrically convenient scheme.

The [Mehrstellen method](../../../finite-difference.md#mehrstellen-method) takes a different route: it uses the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) to eliminate leading truncation derivatives while keeping a compact unknown stencil. Define the [nine-point finite-difference stencil](../../../finite-difference.md#nine-point-finite-difference-stencil)

$$
D_9U=\frac{4\sum_{\mathrm{axial}}U+\sum_{\mathrm{diagonal}}U-20U_{ij}}{6h^2}.
$$

Here each sum has four terms. Equivalently $D_9=D_5+(h^2/6)\delta_{xx}\delta_{yy}$. Expanding gives

$$
D_9u=\Delta u+\frac{h^2}{12}(u_{xxxx}+2u_{xxyy}+u_{yyyy})+O(h^4)
=\Delta u+\frac{h^2}{12}\Delta^2u+O(h^4).
$$

The uncorrected nine-point operator is only second order for a general function. But $-\Delta u=f$ implies $\Delta^2u=-\Delta f$. Moving this known leading defect to the source and approximating its Laplacian with $D_5$ gives

$$
\boxed{-D_9U=f+\frac{h^2}{12}D_5f,\qquad\text{fourth-order normalized residual}.}
$$

Indeed $D_5f=\Delta f+O(h^2)$, and multiplication by $h^2$ makes that replacement's error fourth order. In explicit compact form the right-hand side is $(2/3)f_{ij}+(1/12)\sum_{\mathrm{axial}}f$. Only known source samples, not additional distant solution unknowns, enter this correction. The corresponding unscaled stencil residual is $O(h^6)$. If $f=0$, the leading term already vanishes, which explains [harmonic superconvergence of the nine-point stencil](../../../finite-difference.md#harmonic-superconvergence-of-the-nine-point-stencil).

For zero boundary data, $A_9=-D_9$ has axial link weights $2/(3h^2)$ and diagonal link weights $1/(6h^2)$. Their energy sum proves positive definiteness, and their sign pattern again proves the [discrete maximum principle](../../../finite-difference.md#discrete-maximum-principle). The same quadratic barrier is exact for $A_9$, so

$$
\|e\|_\infty\leq\tfrac18\|A_9e\|_\infty.
$$

For smooth solutions and accurately imposed boundary values this proves fourth-order nodal convergence of the corrected scheme. Singular corners, rough sources or low-order boundary treatment can reduce the observed rate; a formal interior expansion is not a global regularity theorem.

More generally, compact high-order schemes choose a solution stencil and a source stencil together, match their [Taylor expansions](../../../calculus.md#taylor-expansion), and use differentiated forms of the PDE to remove derivatives that would otherwise need a wide solution stencil. Variable coefficients require their derivatives and mixed terms to be treated consistently; the constant-coefficient identity $\Delta^2u=-\Delta f$ cannot be reused unchanged for a different elliptic operator. On irregular meshes, conservation and consistent fluxes may be more useful starting points than a symmetric Cartesian formula.

Finally, discretization and solution cost are coupled. The five-point Dirichlet [matrix](../../../vector-space.md#matrix) has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) proportional to sums of squared sine frequencies, so its smallest [eigenvalue](../../../linear-operator-theory.md#eigenvalue) stays of order one while its largest is $O(h^{-2})$. Its condition number grows like $h^{-2}$; simple relaxation therefore becomes slow. Sparse direct elimination, [Conjugate gradient method](../../../numerical-analysis.md#conjugate-gradient-method) with appropriate [matrix preconditioning](../../../numerical-analysis.md#matrix-preconditioning), and the [multigrid method](../../../numerical-analysis.md#multigrid-method) are alternatives. A sound design combines local accuracy, boundary fidelity, mesh-independent stability, and an algebraic solver whose residual is small enough for the intended error tolerance.

## 7

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

The [multigrid method](../../../numerical-analysis.md#multigrid-method) addresses a characteristic failure of single-grid relaxation: its cheapest updates rapidly remove oscillatory error but barely change smooth error. For example, the one-dimensional [Poisson equation](../../../partial-differential-equation.md#poisson-equation) [matrix](../../../vector-space.md#matrix) has diagonal $2/h^2$. The [weighted Jacobi method](../../../numerical-analysis.md#weighted-jacobi-method) with weight $\omega$ has Fourier error factor

$$
s_\omega(\theta)=1-\omega(1-\cos\theta)=1-2\omega\sin^2(\theta/2).
$$

At low physical frequency, $\theta=O(h)$ and this factor is $1-O(h^2)$, requiring $O(h^{-2})$ sweeps for a fixed error reduction. With $\omega=2/3$, high grid frequencies $\pi/2\leq|\theta|\leq\pi$ are multiplied by at most $1/3$ in modulus. Smooth error on a fine mesh is well represented on a coarser mesh, where it is relatively more oscillatory and hence cheaper to remove. These two complementary mechanisms motivate smoothing and [coarse-grid correction](../../../numerical-analysis.md#coarse-grid-correction).

Write the discrete problem as $A_hu_h=f_h$. For an approximation $v_h$, the residual is $r_h=f_h-A_hv_h$ and the error $e_h=u_h-v_h$ satisfies $A_he_h=r_h$. It is this error equation that is transferred to a coarse grid; restricting the approximate solution alone would not solve the missing error. With prolongation $P$ and restriction $R$, solve

$$
A_He_H=Rr_h,\qquad v_h\leftarrow v_h+Pe_H.
$$

For nested Cartesian grids with $H=2h$, linear interpolation copies a coarse value at a coincident fine node and averages the two nearest coarse values at an intermediate node. Its two-dimensional counterpart is bilinear interpolation. [Full-weighting restriction](../../../numerical-analysis.md#full-weighting-restriction) uses weights $(1,2,1)/4$ in one dimension and

$$
\frac1{16}\begin{pmatrix}1&2&1\\2&4&2\\1&2&1\end{pmatrix}
$$

in two dimensions. With these choices $R=2^{-d}P^T$ in ordinary coordinate inner products. A [Galerkin coarse-grid operator](../../../numerical-analysis.md#galerkin-coarse-grid-operator) is $A_H=RA_hP$; alternatively one can rediscretize the PDE on the coarse mesh when that choice remains compatible with the transfers.

For a symmetric positive-definite fine operator and $R=cP^T$, the exact correction [matrix](../../../vector-space.md#matrix) is

$$
C_h=I-P(RA_hP)^{-1}RA_h.
$$

It satisfies $C_hP=0$ and $P^TA_hC_h=0$. Thus it removes the coarse-space component of the error and is an orthogonal projection in the energy inner product. With pre- and post-smoothing [matrices](../../../vector-space.md#matrix) $S_{\mathrm{pre}},S_{\mathrm{post}}$, the exact two-grid error [matrix](../../../vector-space.md#matrix) is $S_{\mathrm{post}}C_hS_{\mathrm{pre}}$. Effective smoothing on the complementary space and accurate coarse representation of smooth error are both needed for contraction.

A concrete harmonic calculation makes the mechanism quantitative. On the one-dimensional constant-coefficient problem, couple the two harmonics $\theta$ and $\theta+\pi$, put $s=\sin^2(\theta/2)$ and $c=1-s$, and use the above transfers. Linear interpolation has harmonic weights $(c,s)^T$, while the fine operator has diagonal symbol $4\operatorname{diag}(s,c)/h^2$. Therefore its Galerkin correction on this pair is

$$
C=\begin{pmatrix}s&-c\\-s&c\end{pmatrix}.
$$

One pre- and one post-sweep of [weighted Jacobi](../../../numerical-analysis.md#weighted-jacobi-method) with $\omega=2/3$ gives $E=SCS$, $S=\operatorname{diag}(1-4s/3,1-4c/3)$. This rank-one [matrix](../../../vector-space.md#matrix) has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) zero and

$$
s(1-4s/3)^2+c(1-4c/3)^2=\frac19.
$$

The [two-grid Poisson factor with weighted Jacobi](../../../numerical-analysis.md#two-grid-poisson-factor-with-weighted-jacobi) is therefore mesh-independent in this model. A periodic constant nullspace must first be removed; a Dirichlet problem has no such nullspace. This is evidence for the design, not a claim that the same factor applies to every PDE or every smoother.

The [geometric multigrid V-cycle](../../../numerical-analysis.md#geometric-multigrid-v-cycle) replaces the exact coarse solve by one recursively defined coarse cycle. A complete implementation on level $\ell$ proceeds as follows:

- On the coarsest level, solve $A_\ell v_\ell=f_\ell$ directly and return.
- Otherwise perform a fixed number $\nu_1$ of pre-smoothing sweeps, for example $v_\ell\leftarrow v_\ell+\omega D_\ell^{-1}(f_\ell-A_\ell v_\ell)$.
- Compute the current residual $r_\ell=f_\ell-A_\ell v_\ell$ and restrict it: $f_{\ell-1}=R_\ell r_\ell$.
- Initialize the coarse error approximation at zero and apply one V-cycle to $A_{\ell-1}e_{\ell-1}=f_{\ell-1}$.
- Prolong and add the correction: $v_\ell\leftarrow v_\ell+P_\ell e_{\ell-1}$.
- Perform $\nu_2$ post-smoothing sweeps and return the improved approximation.

Boundary values of the solution are imposed on the fine level; the error equation has homogeneous boundary conditions when those values were already imposed exactly. Residuals must be computed after pre-smoothing, not before. The zero initialization on each recursive error solve makes the cycle an error correction rather than an accidental addition of an old coarse solution. For an energy-symmetric cycle usable in [Conjugate gradient method](../../../numerical-analysis.md#conjugate-gradient-method), choose compatible adjoint transfers and symmetric smoothing, such as forward Gauss-Seidel before correction and its backward sweep afterward.

With bounded stencil size and fixed sweep counts, a sweep, residual calculation or transfer costs $O(N_\ell)$. Uniform coarsening gives $N_{\ell-1}\approx2^{-d}N_\ell$, so

$$
\boxed{W(N)=O(N)+W(N/2^d)=O(N),\qquad\text{storage }O(N).}
$$

If the full V-cycle has an error reduction factor $q<1$ independent of mesh size, reducing an arbitrary initial algebraic error by a factor $\varepsilon$ takes $O(\log(1/\varepsilon))$ cycles and $O(N\log(1/\varepsilon))$ work. Linear work per cycle alone does not prove the mesh-independent factor; it rests on the smoothing and approximation properties just illustrated. [Full multigrid](../../../numerical-analysis.md#full-multigrid) starts on a coarse mesh, interpolates its solution to each successive finer mesh, and uses a few cycles per level. When the interpolation accuracy and cycle contraction match the discretization error, this reaches discretization-level accuracy in $O(N)$ work.

Performance depends on the operator. Strong anisotropy can leave error oscillatory in one direction but weakly penalized by the differential operator, defeating point smoothing; line or plane relaxation and selective coarsening address this. Large coefficient jumps demand compatible coarse spaces. Nonrectangular meshes motivate algebraic rather than purely geometric coarsening. Nonlinear problems use a full-approximation formulation instead of the linear residual correction verbatim. Singular Neumann or periodic operators need right-hand-side compatibility and consistent nullspace treatment on every level. Multigrid is fast because its components address different error scales, not because coarsening alone guarantees a good solver.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)

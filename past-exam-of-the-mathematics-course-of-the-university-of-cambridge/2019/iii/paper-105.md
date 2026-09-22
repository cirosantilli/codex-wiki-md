# Paper 105

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_105.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_105.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $u_Q=|Q|^{-1}\int_Qu$. Since $u-u_Q$ has [arithmetic mean](../../../arithmetic.md#arithmetic-mean) zero,

$$
\|u\|_{L^2(Q)}^2=|Q|u_Q^2+\|u-u_Q\|_{L^2(Q)}^2,
$$

and the pairwise-difference identity gives

$$
\|u-u_Q\|_{L^2(Q)}^2
=\frac1{2|Q|}\int_Q\int_Q|u(x)-u(y)|^2\,dx\,dy.
$$

First take $u$ [smooth](../../../analysis.md#smooth-function). Join $x$ to $y$ by changing one coordinate at a time and apply the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality):

$$
|u(x)-u(y)|^2
\leq n\sum_{i=1}^n
|u(x_1,\ldots,x_i,y_{i+1},\ldots,y_n)-u(x_1,\ldots,x_{i-1},y_i,\ldots,y_n)|^2.
$$

For a one-dimensional slice $v$, the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) yields

$$
|v(s)-v(t)|^2\leq |s-t|\int_{\min(s,t)}^{\max(s,t)}|v'(r)|^2\,dr
\leq L\int_0^L|v'(r)|^2\,dr.
$$

Integrating the $i$th summand over $x,y\in Q$ therefore gives at most $L^{n+2}\|D_i u\|_{L^2(Q)}^2$. Hence

$$
\|u-u_Q\|_{L^2(Q)}^2\leq\frac n2L^2\|Du\|_{L^2(Q)}^2.
$$

The [density of smooth functions in a Sobolev space](../../../sobolev-space.md#density-of-smooth-functions-in-a-sobolev-space) extends the estimate to every $u\in H^1(\mathbb R^n)$. Thus

$$
\boxed{\|u\|_{L^2(Q)}^2\leq |Q|u_Q^2+\frac n2L^2\|Du\|_{L^2(Q)}^2.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

With the standard [Sobolev space](../../../sobolev-space.md) inner product, $u_i\rightharpoonup u$ weakly in $H^1(U)$ means

$$
\int_U\bigl(u_i v+Du_i\mathbin\cdot Dv\bigr)
\longrightarrow
\int_U\bigl(uv+Du\mathbin\cdot Dv\bigr)
$$

for every $v\in H^1(U)$. Equivalently, every [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) on $H^1(U)$ takes convergent values on the sequence.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The [Sobolev space](../../../sobolev-space.md) $H^1(U)$ is a separable [Hilbert space](../../../hilbert-space.md). A bounded sequence therefore has a weakly convergent subsequence by the [weak subsequence of a bounded Hilbert-space sequence](../../../hilbert-space.md#weak-subsequence-of-a-bounded-hilbert-space-sequence); write $u_{i_j}\rightharpoonup u$ in $H^1(U)$. Since $U$ is bounded with smooth boundary, the [Rellich-Kondrachov compactness theorem](../../../sobolev-space.md#rellich-kondrachov-theorem) says that $H^1(U)\hookrightarrow L^2(U)$ is compact. Passing to a further subsequence gives

$$
\boxed{u_{i_j}\longrightarrow u\quad\text{strongly in }L^2(U).}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

Suppose the claimed [Poincare-Wirtinger inequality](../../../sobolev-space.md#poincare-wirtinger-inequality) were false. There would be $u_k\in H^1(U)$ such that, after setting

$$
v_k=\frac{u_k-(u_k)_U}{\|u_k-(u_k)_U\|_{L^2(U)}},
$$

we have $(v_k)_U=0$, $\|v_k\|_2=1$, and $\|Dv_k\|_2\to0$. The sequence is bounded in $H^1(U)$, so part 1(b)(ii) supplies a subsequence converging strongly in $L^2(U)$ and weakly in $H^1(U)$ to some $v$.

The weak [gradient](../../../calculus.md#gradient) of $v$ is zero. Because $U$ is [connected](../../../geometry-and-topology.md#connected-space), $v$ is a [constant function](../../../function.md#constant-function); its mean is zero, so $v=0$. Strong convergence would then give $\|v_k\|_2\to0$, contradicting $\|v_k\|_2=1$. Therefore

$$
\boxed{\|u-u_U\|_{L^2(U)}\leq C_1\|Du\|_{L^2(U)}.}
$$

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

If the [Poincare inequality with a boundary trace](../../../sobolev-space.md#poincare-inequality-with-a-boundary-trace) failed, after normalization there would be $u_k\in H^1(U)$ with

$$
\|u_k\|_{L^2(U)}=1,
\qquad
\|Du_k\|_{L^2(U)}+\|u_k\|_{L^2(\partial U)}\longrightarrow0.
$$

As in part 1(c)(i), a subsequence converges strongly in $L^2(U)$ and weakly in $H^1(U)$ to a [constant function](../../../function.md#constant-function) $u$. The [Sobolev trace theorem](../../../sobolev-space.md#sobolev-trace-theorem) is a bounded linear map, so the traces converge weakly while their norms tend to zero; hence the trace of $u$ is zero. A constant with zero trace is zero, contradicting $\|u\|_2=1$. Consequently

$$
\boxed{\|u\|_{L^2(U)}\leq C_2\left(\|Du\|_{L^2(U)}+\|u\|_{L^2(\partial U)}\right).}
$$

## 2

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) states that if $H$ is a real [Hilbert space](../../../hilbert-space.md), $B:H\times H\to\mathbb R$ is a [bounded bilinear form](../../../linear-algebra.md#bounded-bilinear-form), and there is an $\alpha>0$ such that

$$
B(v,v)\geq\alpha\|v\|_H^2
\qquad(v\in H),
$$

then for every bounded linear functional $F\in H'$ there is a unique $u\in H$ satisfying

$$
B(u,v)=F(v)
\qquad(v\in H).
$$

Moreover, $\boxed{\|u\|_H\leq\alpha^{-1}\|F\|_{H'}}$. Symmetry of $B$ is not required.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) is built into the first component's space, while the [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition) is natural. Thus a [weak solution](../../../partial-differential-equation.md#weak-solution) is a pair

$$
(u,w)\in H_0^1(U)\times H^1(U)
$$

such that for every $(v,z)\in H_0^1(U)\times H^1(U)$,

$$
\int_U(Du\mathbin\cdot Dv+uv+wv)=\int_Ufv,
$$



$$
\int_U(Dw\mathbin\cdot Dz+wz-3uz)=\int_Ugz.
$$

If $u,w$ are $C^2$ up to the boundary, taking compactly supported [test functions](../../../distribution-theory.md#test-function) and applying the [fundamental lemma of the calculus of variations](../../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) gives both differential equations pointwise in $U$. Membership of $H_0^1(U)$ gives $u=0$ on $\partial U$. Applying [integration by parts](../../../calculus.md#integration-by-parts) to the second identity and using its differential equation leaves

$$
\int_{\partial U}\frac{\partial w}{\partial\nu}z=0
$$

for every smooth boundary trace $z$. Hence $\partial w/\partial\nu=0$ on $\partial U$, so the equations and both boundary conditions hold classically.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

On the product [Hilbert space](../../../hilbert-space.md) $H=H_0^1(U)\times H^1(U)$ define

$$
B((u,w),(v,z))
=\int_U\bigl(Du\mathbin\cdot Dv+uv+wv+Dw\mathbin\cdot Dz+wz-3uz\bigr)
$$

and

$$
F(v,z)=\int_U(fv+gz).
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) makes $B$ and $F$ bounded. On the diagonal,

$$
B((u,w),(u,w))
=\|Du\|_2^2+\|Dw\|_2^2+\|u-w\|_2^2.
$$

The [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) controls $\|u\|_2$ by $\|Du\|_2$, and

$$
\|w\|_2\leq\|w-u\|_2+\|u\|_2.
$$

The displayed diagonal value therefore controls the full product $H^1$ norm, so $B$ is [coercive](../../../linear-algebra.md#coercive-bilinear-form). The [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) now gives exactly one pair $(u,w)\in H$ satisfying the weak identities. Hence **a unique weak solution exists for every $f,g\in L^2(U)$**.

## 3

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The function $f$ is [real analytic](../../../analysis.md#real-analytic-function) at $y$ if there is a [neighborhood](../../../topology.md#neighbourhood-mathematics) of $y$ on which its multivariable [Taylor series](../../../calculus.md#taylor-series)

$$
\boxed{f(x)=\sum_{\alpha\in\mathbb N^n}
\frac{D^\alpha f(y)}{\alpha!}(x-y)^\alpha}
$$

converges to $f(x)$. Here $\alpha$ is a [multi-index](../../../distribution-theory.md#multi-index-notation); equivalently, $f$ agrees locally with a convergent real [power series](../../../real-analysis.md#power-series) centred at $y$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Locally write the real analytic [hypersurface](../../../differential-geometry.md#hypersurface) as $\Sigma=\{F=0\}$ with $dF\ne0$. The [conormal bundle](../../../symplectic-geometry.md#conormal-bundle) is spanned by $dF$. The surface is a [characteristic hypersurface](../../../partial-differential-equation.md#characteristic-hypersurface) at $p$ precisely when the [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) vanishes on that conormal:

$$
\boxed{\sum_{i,j=1}^n a_{ij}(p)F_{x_i}(p)F_{x_j}(p)=0.}
$$

Only the matrix $(a_{ij}+a_{ji})/2$, which is a [symmetric matrix](../../../linear-algebra.md#symmetric-matrix), contributes to this expression.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

One prescribes analytic [Cauchy data](../../../partial-differential-equation.md#cauchy-data): the value of $u$ and one first derivative transverse to $\Sigma$, for example

$$
u|_\Sigma=\phi,
\qquad
\partial_\nu u|_\Sigma=\psi,
$$

where $\phi$ and $\psi$ are real analytic on $\Sigma$. Being a [non-characteristic hypersurface](../../../partial-differential-equation.md#non-characteristic-hypersurface) allows the equation to solve for the second derivative in the transverse direction. The [Cauchy-Kovalevskaya theorem](../../../partial-differential-equation.md#cauchy-kovalevskaya-theorem) then gives **one and only one local real analytic solution near $p$**.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Expanding the equation gives

$$
u_{xx}-(1-y^2)^2u_{yy}+4y(1-y^2)u_y=0,
$$

so its [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) is

$$
p(y,\xi)=\xi_x^2-(1-y^2)^2\xi_y^2.
$$

If a [characteristic curve](../../../partial-differential-equation.md#characteristic-curve) is locally a graph $y=y(x)$, its conormal is proportional to $(-y',1)$. The characteristic equation is therefore

$$
(y')^2-(1-y^2)^2=0,
\qquad
\frac{dy}{dx}=\pm(1-y^2).
$$

On each region separated by $y=\pm1$, separation of variables gives

$$
\frac12\log\left|\frac{1+y}{1-y}\right|=\pm x+C.
$$

Thus all the characteristic curves are

$$
\boxed{
\begin{cases}
y=\tanh(\pm x+C),&|y|<1,\\
y=\coth(\pm x+C),&|y|>1,\\
y=1\text{ or }y=-1.&
\end{cases}}
$$

The inner curves approach the horizontal characteristics $y=\pm1$ as $x\to\pm\infty$; the outer hyperbolic-cotangent branches have vertical asymptotes and also approach $y=\pm1$. This describes the requested sketch.

The initial line $x=0$ has conormal $(1,0)$, and $p(y,1,0)=1$, so it is a [non-characteristic hypersurface](../../../partial-differential-equation.md#non-characteristic-hypersurface) at every point. Since the coefficients and prescribed data are real analytic, the [Cauchy-Kovalevskaya theorem](../../../partial-differential-equation.md#cauchy-kovalevskaya-theorem) gives a unique real analytic solution in a neighborhood of each point of $\{x=0\}$, hence in a neighborhood of that line.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Put $a(y)=(1-y^2)^2$. Multiply $u_{xx}=\partial_y(au_y)$ by $2u_x$ and integrate over $-1<y<1$. An [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\begin{aligned}
\frac d{dx}\int_{-1}^1u_x^2\,dy
&=2\bigl[au_xu_y\bigr]_{-1}^1-2\int_{-1}^1a u_{xy}u_y\,dy\\
&=-\frac d{dx}\int_{-1}^1a u_y^2\,dy,
\end{aligned}
$$

because $a(1)=a(-1)=0$. Therefore the [energy estimate](../../../partial-differential-equation.md#energy-estimate) is in fact the conservation law

$$
\boxed{\frac d{dx}\int_{-1}^1\left(u_x^2+(1-y^2)^2u_y^2\right)dy=0.}
$$

If $u(0,y)=u_x(0,y)=0$, then differentiating the first identity in $y$ also gives $u_y(0,y)=0$, so the conserved nonnegative energy is zero. Hence $u_x=0$ and $(1-y^2)u_y=0$ throughout the open strip. There $|y|<1$, so both derivatives vanish; connectedness and the initial value now give

$$
\boxed{u(x,y)=0\qquad((x,y)\in\mathbb R\times(-1,1)).}
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Assume $0<\varepsilon<1$ and set

$$
a=1-\varepsilon,
\qquad
S_\varepsilon=\operatorname{artanh}(a)
=\frac12\log\frac{2-\varepsilon}{\varepsilon}.
$$

The [travel-time coordinate for a one-dimensional variable-speed wave equation](../../../partial-differential-equation.md#travel-time-coordinate-for-a-one-dimensional-variable-speed-wave-equation)

$$
s=\operatorname{artanh}y
$$

sends the initial interval $I_\varepsilon=(-a,a)$ to $(-S_\varepsilon,S_\varepsilon)$. By the [characteristic curves for speed one minus y squared](../../../partial-differential-equation.md#characteristic-curves-for-speed-one-minus-y-squared), the two characteristic coordinates are $s-x$ and $s+x$. The [finite propagation speed](../../../wave-equation.md#finite-propagation-speed) and uniqueness theorem for [hyperbolic partial differential equations](../../../partial-differential-equation.md#hyperbolic-partial-differential-equation) therefore give the maximal characteristic diamond

$$
\boxed{D_\varepsilon
=\left\{(x,y):|x|+|\operatorname{artanh}y|<S_\varepsilon\right\}.}
$$

Equivalently,

$$
D_\varepsilon
=\left\{(x,y):|x|<S_\varepsilon,
\ |y|<\tanh(S_\varepsilon-|x|)\right\}.
$$

In the $(x,s)$ plane this is a diamond with vertices $(0,\pm S_\varepsilon)$ and $(\pm S_\varepsilon,0)$; transforming back bends its four sides into the characteristic curves found in part 3(c). Beyond any one of those sides, a point's backward characteristics meet $x=0$ outside $I_\varepsilon$, where no [Cauchy data](../../../partial-differential-equation.md#cauchy-data) were prescribed, so uniqueness cannot be extended farther.

## 4

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Extend $u$ by zero to $\mathbb R^n$; its [compact support](../../../function.md#compact-support) inside the ball makes the extension [smooth](../../../analysis.md#smooth-function). The [Fourier transform of a derivative](../../../fourier-analysis.md#fourier-transform-of-a-derivative) gives

$$
\widehat{L_0u}(\xi)=-(A\xi\mathbin\cdot\xi)\widehat u(\xi).
$$

The assumption says that $L_0$ is a [uniformly elliptic operator](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator), so

$$
|A\xi\mathbin\cdot\xi|^2\geq\theta^2|\xi|^4.
$$

Moreover,

$$
\sum_{i,j=1}^n|\xi_i\xi_j|^2
=\left(\sum_{i=1}^n\xi_i^2\right)^2
=|\xi|^4.
$$

The [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem) therefore yields

$$
\|L_0u\|_2^2
=\int_{\mathbb R^n}|A\xi\mathbin\cdot\xi|^2|\widehat u|^2\,d\xi
\geq\theta^2\int_{\mathbb R^n}|\xi|^4|\widehat u|^2\,d\xi
=\theta^2\|D^2u\|_2^2.
$$

All integrands vanish outside the original support where appropriate, so

$$
\boxed{\theta\|D^2u\|_{L^2(B_r(x_0))}\leq\|L_0u\|_{L^2(B_r(x_0))}.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Write $Lu=L_0u+(a^{ij}-A^{ij})D_{ij}u$, with repeated indices summed. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) over the $n^2$ coefficient pairs give

$$
\begin{aligned}
\|Lu\|_2
&\geq\|L_0u\|_2-\left\|\sum_{i,j}(a^{ij}-A^{ij})D_{ij}u\right\|_2\\
&\geq\theta\|D^2u\|_2-n\varepsilon\|D^2u\|_2.
\end{aligned}
$$

Choose

$$
\boxed{\varepsilon=\frac{\theta}{2n}.}
$$

Then the strict coefficient bound in the question implies

$$
\boxed{\frac\theta2\|D^2u\|_{L^2(B_r(x_0))}\leq\|Lu\|_{L^2(B_r(x_0))}.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The continuous coefficients are [uniformly continuous](../../../topological-analysis.md#uniform-continuity) on a compact neighborhood of $\overline W$. For every $x_0\in\overline W$, choose a ball $B_r(x_0)\Subset U$ small enough that

$$
\|a^{ij}-a^{ij}(x_0)\|_{L^\infty(B_r(x_0))}<\frac\theta{2n}
$$

for all $i,j$. Part 4(b), with the frozen [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) $A=(a^{ij}(x_0))$, then applies on this ball.

Choose a finite collection of these balls and a smooth [partition of unity](../../../differential-geometry.md#partition-of-unity) $(\eta_k)$ that sums to one near $\overline W$, with each $\eta_k$ supported in its corresponding ball. Applying part 4(b) to $\eta_k u$ gives

$$
\|D^2(\eta_k u)\|_2\leq C\|L(\eta_k u)\|_2.
$$

Since $(a^{ij})$ is symmetric, the [Leibniz rule](../../../calculus.md#leibniz-rule) gives the commutator formula

$$
L(\eta_k u)
=\eta_kLu+2a^{ij}(D_i\eta_k)(D_ju)+a^{ij}(D_{ij}\eta_k)u.
$$

The coefficients and the finitely many derivatives of the [cutoff functions](../../../distribution-theory.md#cutoff-function) are bounded, so

$$
\|L(\eta_k u)\|_2
\leq C\left(\|Lu\|_{L^2(U)}+\|u\|_{H^1(U)}\right).
$$

Finally $u=\sum_k\eta_k u$ near $\overline W$. Summing the finite set of local estimates proves

$$
\boxed{\|D^2u\|_{L^2(W)}
\leq C\left(\|Lu\|_{L^2(U)}+\|u\|_{H^1(U)}\right).}
$$

This is the [coefficient-freezing interior second-derivative estimate](../../../elliptic-boundary-value-problem.md#coefficient-freezing-interior-second-derivative-estimate).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Fix $W\Subset V\Subset U$. The standard local regularization of the maximal [graph norm](../../../functional-analysis.md#graph-norm) domain supplies smooth compactly supported approximants $u_k$ on $V$ such that

$$
u_k\longrightarrow u\quad\text{in }H^1(V),
\qquad
Lu_k\longrightarrow Lu\quad\text{in }L^2(V).
$$

Apply part 4(c), with $V$ as the outer domain, to $u_k-u_m$. It gives

$$
\|D^2(u_k-u_m)\|_{L^2(W)}
\leq C\left(\|L(u_k-u_m)\|_{L^2(V)}
+\|u_k-u_m\|_{H^1(V)}\right)\longrightarrow0.
$$

Thus $(u_k)$ is Cauchy in $H^2(W)$. Its $H^1$ limit is $u$, so $u\in H^2(W)$. Since $W\Subset U$ was arbitrary, the definition of a [Local Sobolev space](../../../sobolev-space.md#local-sobolev-space) gives

$$
\boxed{u\in H^2_{\mathrm{loc}}(U).}
$$

This is the [Interior H2 regularity for continuous nondivergence coefficients](../../../elliptic-boundary-value-problem.md#interior-h2-regularity-for-continuous-nondivergence-coefficients).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)

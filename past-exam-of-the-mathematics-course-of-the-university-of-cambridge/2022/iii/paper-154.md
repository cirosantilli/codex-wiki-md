# Paper 154

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_154.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_154.pdf)

**Table of contents**

- [1](#1)
  - [1](#1/1)
    - [Solution](#1/1/solution)
    - [2](#1/1/2)
      - [Solution](#1/1/2/solution)
    - [3](#1/1/3)
      - [Solution](#1/1/3/solution)
    - [4](#1/1/4)
      - [Solution](#1/1/4/solution)
    - [5](#1/1/5)
      - [Solution](#1/1/5/solution)
- [2](#2)
  - [1](#2/1)
    - [Solution](#2/1/solution)
  - [2](#2/2)
    - [Solution](#2/2/solution)
    - [3](#2/2/3)
      - [Solution](#2/2/3/solution)
    - [4](#2/2/4)
      - [Solution](#2/2/4/solution)
    - [5](#2/2/5)
      - [Solution](#2/2/5/solution)
- [3](#3)
  - [1](#3/1)
    - [Solution](#3/1/solution)
  - [2](#3/2)
    - [Solution](#3/2/solution)
  - [3](#3/3)
    - [Solution](#3/3/solution)
    - [4](#3/3/4)
      - [Solution](#3/3/4/solution)
    - [5](#3/3/5)
      - [Solution](#3/3/5/solution)

## 1

↑ **Parent:** [Paper 154](paper-154.md)

<h3 id="1/1">1</h3>

↑ **Parent:** [1](#1)

<h4 id="1/1/solution">Solution</h4>

↑ **Parent:** [1](#1/1)

Choose a [test function](../../../distribution-theory.md#space-of-test-functions) $\chi$ that equals one on the unit ball and vanishes outside the ball of radius two. Since

$$
\operatorname{div}(x\chi)=d\chi+x\mathbin{\cdot}\nabla\chi,
$$

[integration by parts](../../../calculus.md#integration-by-parts) gives

$$
d\int\chi u^2
=-\int(x\mathbin{\cdot}\nabla\chi)u^2-2\int\chi u\,x\mathbin{\cdot}\nabla u.
$$

The first term on the right is supported where $1\leq|x|\leq2$, where $u^2\leq |x|^\alpha u^2$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and [Young inequality](../../../nonlinear-analysis.md#young-s-inequality-for-products) bound the second term by

$$
2\left|\int\chi u\,x\mathbin{\cdot}\nabla u\right|
\leq\frac d2\int\chi u^2+C\int|\nabla u|^2.
$$

After absorbing the first integral,

$$
\int_{|x|\leq1}|u|^2
\leq C\left(\int|\nabla u|^2+\int|x|^\alpha|u|^2\right)
=C\|u\|_\Sigma^2.
$$

This estimate also proves completeness. Indeed, a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) in $\Sigma$ is Cauchy in $H^1$ locally, while its gradients and the functions $|x|^{\alpha/2}u_n$ converge in $L^2$. The limits agree locally with a function $u$, so $u\in\Sigma$ and $u_n\to u$ in the energy norm. Thus $\Sigma$ is a [Hilbert space](../../../hilbert-space.md); it is the [confining-potential energy space](../../../nonlinear-analysis.md#confining-potential-energy-space) for $V(x)=|x|^\alpha$.

<h4 id="1/1/2">2</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/2/solution">Solution</h5>

↑ **Parent:** [2](#1/1/2)

On the unit ball, part 1 controls the $L^2$ norm. Outside it, $|x|^\alpha\geq1$, so

$$
\int_{|x|>1}|u|^2\leq\int|x|^\alpha|u|^2.
$$

Hence $\|u\|_2\leq C\|u\|_\Sigma$, proving that the [embedding](../../../vector-space.md#linear-map) $\Sigma\hookrightarrow L^2$ is [continuous](../../../calculus.md#continuous-function).

For compactness, let $(u_n)$ be bounded in $\Sigma$. On each ball, it is bounded in $H^1$, so the [Rellich-Kondrachov compactness theorem](../../../sobolev-space.md#rellich-kondrachov-theorem) gives a subsequence convergent in local $L^2$. The tail estimate

$$
\int_{|x|>R}|u_n|^2
\leq R^{-\alpha}\int|x|^\alpha|u_n|^2
$$

is uniform in $n$ and tends to zero as $R\to\infty$. A [diagonal argument](../../../foundations-of-mathematics.md#diagonal-argument) therefore gives convergence in all of $L^2$. This is the [compact embedding of a confining-potential energy space](../../../nonlinear-analysis.md#compact-embedding-of-a-confining-potential-energy-space).

<h4 id="1/1/3">3</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/3/solution">Solution</h5>

↑ **Parent:** [3](#1/1/3)

For fixed $f\in L^2$, the functional

$$
\ell_f(v)=\langle v,f\rangle_{L^2}
$$

is bounded on $\Sigma$ by the continuous embedding from part 2:

$$
|\ell_f(v)|\leq\|v\|_2\|f\|_2\leq C\|v\|_\Sigma\|f\|_2.
$$

The [Riesz representation theorem](../../../hilbert-space.md#riesz-representation-theorem) gives a unique $T(f)\in\Sigma$ such that $\langle v,T(f)\rangle_\Sigma=\ell_f(v)$ for every $v\in\Sigma$. It also gives

$$
\|T(f)\|_\Sigma=\|\ell_f\|_{\Sigma^*}\leq C\|f\|_2,
$$

so the [linear operator](../../../vector-space.md#linear-operator) $T:L^2\to\Sigma$ is bounded.

<h4 id="1/1/4">4</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/4/solution">Solution</h5>

↑ **Parent:** [4](#1/1/4)

As a map into $L^2$, $T$ factors as

$$
L^2\xrightarrow{\,T\,}\Sigma\hookrightarrow L^2.
$$

The first arrow is bounded by part 3 and the second is the compact embedding from part 2; hence $T:L^2\to L^2$ is a [compact operator](../../../compact-operator.md).

Writing $u=T(f)$ in the defining identity gives

$$
\int\nabla v\mathbin{\cdot}\nabla u+\int |x|^\alpha vu=\int vf
\qquad(v\in\Sigma).
$$

In particular this holds for every [test function](../../../distribution-theory.md#space-of-test-functions) $v$, so the definition of a [distributional derivative](../../../distribution-theory.md#distributional-derivative) yields

$$
\boxed{(-\Delta+|x|^\alpha)T(f)=f
\quad\text{in }\mathcal D'(\mathbb R^d).}
$$

<h4 id="1/1/5">5</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/5/solution">Solution</h5>

↑ **Parent:** [5](#1/1/5)

Minimize $\|u\|_\Sigma^2$ subject to $\|u\|_2=1$. A minimizing sequence is bounded in $\Sigma$, and part 2 supplies a subsequence converging strongly in $L^2$ and weakly in $\Sigma$. The constraint survives the strong convergence, while [weak lower semicontinuity](../../../functional-analysis.md#weak-lower-semicontinuity) of the norm shows that the limit $\psi$ attains the minimum. Since $\||\psi|\|_2=\|\psi\|_2$ and $|\nabla|\psi||\leq|\nabla\psi|$ [almost everywhere](../../../measure-theory.md#almost-everywhere), we may take $\psi\geq0$.

The [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) equation is

$$
\int\nabla v\mathbin{\cdot}\nabla\psi+\int|x|^\alpha v\psi
=\lambda\int v\psi
\qquad(v\in\Sigma),
$$

where testing with $v=\psi$ shows that $\lambda=\|\psi\|_\Sigma^2>0$. Thus

$$
(-\Delta+|x|^\alpha)\psi=\lambda\psi
\quad\text{in }\mathcal D'(\mathbb R^d).
$$

This is the [ground-state eigenfunction of a confining Schrödinger operator](../../../nonlinear-analysis.md#ground-state-eigenfunction-of-a-confining-schrodinger-operator).

<h2 id="2">2</h2>

↑ **Parent:** [Paper 154](paper-154.md)

<h3 id="2/1">1</h3>

↑ **Parent:** [2](#2)

<h4 id="2/1/solution">Solution</h4>

↑ **Parent:** [1](#2/1)

Set $p=2+4/d$. For $u_{a,\lambda}(x)=au(\lambda x)$, the [change of variables](../../../calculus.md#change-of-variables-formula) $y=\lambda x$ gives

$$
\|\nabla u_{a,\lambda}\|_2^2
=|a|^2\lambda^{2-d}\|\nabla u\|_2^2,\qquad
\|u_{a,\lambda}\|_2^{4/d}
=|a|^{4/d}\lambda^{-2}\|u\|_2^{4/d},
$$

and

$$
\|u_{a,\lambda}\|_p^p
=|a|^{2+4/d}\lambda^{-d}\|u\|_p^p.
$$

The factors cancel, so the [Weinstein functional](../../../nonlinear-analysis.md#weinstein-functional) satisfies $J(u_{a,\lambda})=J(u)$.

The [Gagliardo-Nirenberg interpolation inequality](../../../sobolev-space.md#gagliardo-nirenberg-interpolation-inequality) gives

$$
\|u\|_p^p\leq C_d\|\nabla u\|_2^2\|u\|_2^{4/d}.
$$

**Consequently $J(u)\geq C_d^{-1}$ for every nonzero $u\in H^1$, and therefore $I>0$.**

<h3 id="2/2">2</h3>

↑ **Parent:** [2](#2)

<h4 id="2/2/solution">Solution</h4>

↑ **Parent:** [2](#2/2)

By the two invariances from part 1, normalize a minimizing sequence $(u_n)$ so that

$$
\|u_n\|_2=\|\nabla u_n\|_2=1.
$$

Replacing $u_n$ by $|u_n|$ and then by its [symmetric decreasing rearrangement](../../../nonlinear-analysis.md#symmetric-decreasing-rearrangement) preserves its $L^2$ and $L^p$ norms and does not increase the gradient norm. A harmless dilation restores the normalization, so we may take the sequence nonnegative, radial, and radially decreasing.

The sequence has a weakly convergent subsequence in $H^1$. Radial compactness and the fixed scale give strong convergence in $L^p$; in particular the limit is nonzero because $\|u_n\|_p^p\to I^{-1}$. [Weak lower semicontinuity](../../../functional-analysis.md#weak-lower-semicontinuity) of the $L^2$ and gradient norms then shows that the limit attains the infimum. This is the [existence of a Weinstein-functional minimizer](../../../nonlinear-analysis.md#existence-of-a-weinstein-functional-minimizer).

<h4 id="2/2/3">3</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/3/solution">Solution</h5>

↑ **Parent:** [3](#2/2/3)

Write

$$
A=\|\nabla u\|_2^2,\qquad B=\|u\|_2^2,\qquad C=\|u\|_p^p.
$$

Differentiating $\log J(u+th)$ at $t=0$ for a real [test function](../../../distribution-theory.md#space-of-test-functions) $h$ gives

$$
\frac2A\int\nabla u\mathbin{\cdot}\nabla h
+\frac4{dB}\int uh-\frac pC\int u^{p-1}h=0.
$$

After [integration by parts](../../../calculus.md#integration-by-parts),

$$
\Delta u-\lambda u+\mu u^{1+4/d}=0,
\qquad
\lambda=\frac{2A}{dB}>0,\qquad
\mu=\frac{pA}{2C}>0.
$$

Rescaling the dependent and independent variables reduces this [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) to the ground-state equation for $Q$. The uniqueness of its positive radial solution and the equality cases in rearrangement show that all minimizers are

$$
u(x)=aQ(b(x-x_0)),
\qquad
a\in\mathbb C\setminus\{0\},\quad b>0,\quad x_0\in\mathbb R^d.
$$

This is the [classification of Weinstein-functional minimizers](../../../nonlinear-analysis.md#classification-of-weinstein-functional-minimizers).

<h4 id="2/2/4">4</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/4/solution">Solution</h5>

↑ **Parent:** [4](#2/2/4)

The [Pohozaev identity for the mass-critical NLS ground state](../../../nonlinear-analysis.md#pohozaev-identity-for-the-mass-critical-nls-ground-state) gives

$$
E(Q)=0,\qquad
\|Q\|_p^p=\frac p2\|\nabla Q\|_2^2.
$$

Since $Q$ is a minimizer,

$$
\boxed{I=J(Q)
=\frac{\|\nabla Q\|_2^2\|Q\|_2^{4/d}}{\|Q\|_p^p}
=\frac2p\|Q\|_2^{4/d}
=\frac{2}{2+4/d}\|Q\|_2^{4/d}.}
$$

<h4 id="2/2/5">5</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/5/solution">Solution</h5>

↑ **Parent:** [5](#2/2/5)

The definition of the [infimum](../../../real-analysis.md#infimum) $I$ gives

$$
\|u\|_p^p
\leq I^{-1}\|\nabla u\|_2^2\|u\|_2^{4/d}.
$$

Substituting the value of $I$ from part 4 into the energy yields

$$
\begin{aligned}
E(u)
&=\frac12\|\nabla u\|_2^2-\frac1p\|u\|_p^p\\
&\geq\frac12\|\nabla u\|_2^2
\left[1-\left(\frac{\|u\|_2}{\|Q\|_2}\right)^{4/d}\right].
\end{aligned}
$$

This is [coercivity below the NLS ground-state mass](../../../nonlinear-analysis.md#coercivity-below-the-nls-ground-state-mass).

<h2 id="3">3</h2>

↑ **Parent:** [Paper 154](paper-154.md)

<h3 id="3/1">1</h3>

↑ **Parent:** [3](#3)

<h4 id="3/1/solution">Solution</h4>

↑ **Parent:** [1](#3/1)

Both [Mass conservation for the nonlinear Schrödinger equation](../../../nonlinear-analysis.md#mass-conservation-for-the-nonlinear-schrodinger-equation) and [Energy conservation for the nonlinear Schrödinger equation](../../../nonlinear-analysis.md#energy-conservation-for-the-nonlinear-schrodinger-equation) hold throughout the maximal lifespan. Since $\|u_0\|_2<\|Q\|_2$, the [Sharp Gagliardo-Nirenberg inequality](../../../nonlinear-analysis.md#sharp-gagliardo-nirenberg-inequality) gives the uniform estimate

$$
\frac12\left[1-\left(\frac{\|u_0\|_2}{\|Q\|_2}\right)^{4/d}\right]
\|\nabla u(t)\|_2^2
\leq E(u(t))=E(u_0).
$$

**Thus the gradient norm stays bounded. The [Blowup alternative for the nonlinear Schrödinger equation](../../../nonlinear-analysis.md#blowup-alternative-for-the-nonlinear-schrodinger-equation) rules out a finite endpoint of the lifespan in either time direction, so the solution is global.**

<h3 id="3/2">2</h3>

↑ **Parent:** [3](#3)

<h4 id="3/2/solution">Solution</h4>

↑ **Parent:** [2](#3/2)

For real $h\in\mathcal D(\mathbb R^d)$, differentiation under the integral gives

$$
\left.\frac d{dt}E(Q+th)\right|_{t=0}
=\int\nabla Q\mathbin{\cdot}\nabla h-\int Q^{1+4/d}h.
$$

The ground-state equation $\Delta Q-Q+Q^{1+4/d}=0$ and [integration by parts](../../../calculus.md#integration-by-parts) reduce this to

$$
\left.\frac d{dt}E(Q+th)\right|_{t=0}=-\int Qh.
$$

In particular, along the amplitude direction $h=Q$ the derivative is $-\|Q\|_2^2<0$. Hence $u_0=(1+\delta)Q$ has negative energy for every sufficiently small $\delta>0$, while

$$
\|u_0\|_2=(1+\delta)\|Q\|_2<\|Q\|_2+\epsilon
$$

when $\delta$ is chosen small enough. The ground state has finite variance, so [negative-energy blowup for the mass-critical focusing nonlinear Schrödinger equation](../../../nonlinear-analysis.md#negative-energy-blowup-for-the-mass-critical-focusing-nonlinear-schrodinger-equation) shows that the corresponding solution blows up in finite time.

<h3 id="3/3">3</h3>

↑ **Parent:** [3](#3)

<h4 id="3/3/solution">Solution</h4>

↑ **Parent:** [3](#3/3)

Under the mass-critical spatial scaling

$$
v_n(x)=\lambda_n^{d/2}u(t_n,\lambda_nx),
$$

the $L^2$ norm is invariant and the gradient norm is multiplied by $\lambda_n$. Therefore choose

$$
\lambda_n=\frac{\|\nabla Q\|_2}{\|\nabla u(t_n)\|_2}.
$$

Finite-time blowup and the [Blowup alternative for the nonlinear Schrödinger equation](../../../nonlinear-analysis.md#blowup-alternative-for-the-nonlinear-schrodinger-equation) imply $\|\nabla u(t_n)\|_2\to\infty$, so $\lambda_n\to0$.

The energy has scaling degree two:

$$
E(v_n)=\lambda_n^2E(u(t_n))
=\lambda_n^2E(u_0)\longrightarrow0,
$$

where the second equality uses [Energy conservation for the nonlinear Schrödinger equation](../../../nonlinear-analysis.md#energy-conservation-for-the-nonlinear-schrodinger-equation).

<h4 id="3/3/4">4</h4>

↑ **Parent:** [3](#3/3)

<h5 id="3/3/4/solution">Solution</h5>

↑ **Parent:** [4](#3/3/4)

The [profile decomposition modulo translations](../../../nonlinear-analysis.md#profile-decomposition-modulo-translations) says that every bounded sequence $(w_n)$ in $H^1(\mathbb R^d)$ has, after passage to a subsequence,

$$
w_n=\sum_{j=1}^J\phi^j(\,\cdot-x_n^j)+r_n^J,
$$

where the translation parameters are asymptotically orthogonal,

$$
|x_n^j-x_n^k|\longrightarrow\infty\quad(j\ne k),
$$

the squared $L^2$ and gradient norms decouple,

$$
\|w_n\|_2^2=\sum_{j=1}^J\|\phi^j\|_2^2+\|r_n^J\|_2^2+o_n(1),
$$



$$
\|\nabla w_n\|_2^2
=\sum_{j=1}^J\|\nabla\phi^j\|_2^2+\|\nabla r_n^J\|_2^2+o_n(1),
$$

and the remainder vanishes in every subcritical norm:

$$
\boxed{\lim_{J\to\infty}\limsup_{n\to\infty}
\|r_n^J\|_{L^p}=0
\qquad(2<p<2^*).}
$$

<h4 id="3/3/5">5</h4>

↑ **Parent:** [3](#3/3)

<h5 id="3/3/5/solution">Solution</h5>

↑ **Parent:** [5](#3/3/5)

Part 3 and [Mass conservation for the nonlinear Schrödinger equation](../../../nonlinear-analysis.md#mass-conservation-for-the-nonlinear-schrodinger-equation) give

$$
\|v_n\|_2=\|Q\|_2,\qquad
\|\nabla v_n\|_2=\|\nabla Q\|_2,\qquad
E(v_n)\to0.
$$

The last relation and the energy formula imply

$$
\|v_n\|_{2+4/d}^{2+4/d}
\longrightarrow\frac{2+4/d}{2}\|\nabla Q\|_2^2
=\|Q\|_{2+4/d}^{2+4/d},
$$

where the final equality follows from the [Pohozaev identity for the mass-critical NLS ground state](../../../nonlinear-analysis.md#pohozaev-identity-for-the-mass-critical-nls-ground-state). Thus $(v_n)$ is a minimizing sequence for the [Weinstein functional](../../../nonlinear-analysis.md#weinstein-functional) with the same normalization as $Q$.

Apply the profile decomposition from part 4. The [Sharp Gagliardo-Nirenberg inequality](../../../nonlinear-analysis.md#sharp-gagliardo-nirenberg-inequality) bounds each profile by the product of its gradient energy and its mass to the power $2/d$. Since the total mass is exactly $\|Q\|_2^2$, any split into two nonzero profiles would make the limiting inequality strict. Hence precisely one profile carries all the mass and gradient energy. The norm decouplings then make the remainder converge strongly to zero in $H^1$. For suitable translations $x_n$,

$$
v_n(\,\cdot+x_n)\longrightarrow\phi
\quad\text{strongly in }H^1(\mathbb R^d),
$$

and the [Sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem) gives the required strong convergence in $L^{2+4/d}$. This is the [compactness of a mass-critical minimizing sequence](../../../nonlinear-analysis.md#compactness-of-a-mass-critical-minimizing-sequence).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)

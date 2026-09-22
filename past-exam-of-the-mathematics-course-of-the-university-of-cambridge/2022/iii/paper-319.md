# Paper 319

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_319.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_319.pdf)

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
  - [f](#1/f)
    - [Solution](#1/f/solution)
  - [g](#1/g)
    - [Solution](#1/g/solution)
  - [h](#1/h)
    - [Solution](#1/h/solution)

## 1

↑ **Parent:** [Paper 319](paper-319.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [infinitesimal generator of a semigroup](../../../functional-analysis.md#infinitesimal-generator-of-a-semigroup) is the [linear operator](../../../vector-space.md#linear-operator)

$$
Au=\lim_{h\downarrow0}\frac{U(h)u-u}{h}
$$

with [generator domain](../../../functional-analysis.md#generator-domain)

$$
D(A)=\left\{u\in H:\lim_{h\downarrow0}\frac{U(h)u-u}{h}\text{ exists in }H\right\}.
$$

For example, the [Bochner integral](../../../measure-theory.md#bochner-integral)

$$
u_t=\int_0^tU(s)u\,ds
$$

belongs to $D(A)$ for every $u\in H$ and $t>0$, since $Au_t=U(t)u-u$.

To prove that $A$ is a [closed linear operator](../../../functional-analysis.md#closed-linear-operator), suppose $u_n\in D(A)$, $u_n\to u$, and $Au_n\to v$. For vectors in the [generator domain](../../../functional-analysis.md#generator-domain),

$$
U(t)u_n-u_n=\int_0^tU(s)Au_n\,ds.
$$

Passing to the [limit](../../../calculus.md#limit-of-a-function) in the [Banach space](../../../banach-space.md) gives

$$
U(t)u-u=\int_0^tU(s)v\,ds.
$$

After division by $t$, [strong continuity](../../../functional-analysis.md#strong-continuity) makes the right side converge to $v$ as $t\downarrow0$. Hence $u\in D(A)$ and $Au=v$, so $A$ is closed.

For $\operatorname{Re}z>\omega$, define the [Bochner integral](../../../measure-theory.md#bochner-integral)

$$
R(z)u=\int_0^\infty e^{-zt}U(t)u\,dt.
$$

It converges absolutely because

$$
\|e^{-zt}U(t)u\|\leq Me^{-(\operatorname{Re}z-\omega)t}\|u\|.
$$

Integrating the semigroup difference quotient shows that $R(z)u\in D(A)$ and $(zI-A)R(z)u=u$. The same computation for $u\in D(A)$ gives $R(z)(zI-A)u=u$. Thus the [Laplace-transform formula for a semigroup resolvent](../../../functional-analysis.md#laplace-transform-formula-for-a-semigroup-resolvent) proves

$$
\boxed{\{z\in\mathbb C:\operatorname{Re}z>\omega\}\subseteq\rho(A)},
\qquad
\|R(z)\|\leq\frac{M}{\operatorname{Re}z-\omega}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [Laplace-transform formula for a semigroup resolvent](../../../functional-analysis.md#laplace-transform-formula-for-a-semigroup-resolvent) is locally uniformly convergent in the half-plane $\operatorname{Re}z>\omega$, so it may be differentiated under the [Bochner integral](../../../measure-theory.md#bochner-integral):

$$
\frac{d^n}{dz^n}R(z)u
=(-1)^n\int_0^\infty t^ne^{-tz}U(t)u\,dt.
$$

The [resolvent identity](../../../banach-algebra.md#resolvent-identity) gives $R'(z)=-R(z)^2$ and, by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction),

$$
\frac{d^n}{dz^n}R(z)=(-1)^nn!R(z)^{n+1}.
$$

Therefore

$$
\boxed{n!(zI-A)^{-(n+1)}u
=\int_0^\infty t^ne^{-tz}U(t)u\,dt}.
$$

For real $\lambda>\omega$, the [integral triangle inequality](../../../topological-analysis.md#integral-triangle-inequality) and the [Gamma integral](../../../complex-analysis.md#gamma-integral) give

$$
\begin{aligned}
n!\|(\lambda I-A)^{-(n+1)}u\|
&\leq M\|u\|\int_0^\infty t^ne^{-(\lambda-\omega)t}\,dt\\
&=\frac{Mn!}{(\lambda-\omega)^{n+1}}\|u\|.
\end{aligned}
$$

Consequently

$$
\boxed{\|(\lambda I-A)^{-(n+1)}u\|
\leq\frac{M}{(\lambda-\omega)^{n+1}}\|u\|}.
$$

The exponent $-n+1$ printed in the question is a typographical error: already at $n=0$ it contradicts the first-resolvent bound.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $(u_n)$ be a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) in the [graph norm](../../../functional-analysis.md#graph-norm)

$$
\|u\|_Y=\|u\|+\|Au\|.
$$

Then $(u_n)$ and $(Au_n)$ are [Cauchy sequences](../../../real-analysis.md#cauchy-sequence) in the [Banach space](../../../banach-space.md) $H$, so for some $u,v\in H$,

$$
u_n\to u,
\qquad
Au_n\to v.
$$

Because $A$ is a [closed linear operator](../../../functional-analysis.md#closed-linear-operator), $u\in D(A)$ and $Au=v$. It follows that

$$
\|u_n-u\|_Y=\|u_n-u\|+\|Au_n-Au\|\longrightarrow0.
$$

Thus every [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) converges in $Y=(D(A),\|\cdot\|_Y)$, and

$$
\boxed{Y\text{ is a Banach space}}.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For $y\in D(A)$, the [semigroup property](../../../functional-analysis.md#semigroup-property) gives

$$
\frac{U(h)U(t)y-U(t)y}{h}
=U(t)\frac{U(h)y-y}{h}\longrightarrow U(t)Ay.
$$

Hence $U(t)y\in D(A)$ and

$$
AU(t)y=U(t)Ay.
$$

The [generator domain](../../../functional-analysis.md#generator-domain) is therefore an [invariant subspace](../../../representation-theory.md#invariant-subspace), and the [operator norm](../../../continuous-dual-space.md#operator-norm) bound gives

$$
\begin{aligned}
\|\widetilde U(t)y\|_Y
&=\|U(t)y\|+\|AU(t)y\|\\
&=\|U(t)y\|+\|U(t)Ay\|\\
&\leq Me^{\omega t}\bigl(\|y\|+\|Ay\|\bigr).
\end{aligned}
$$

Thus

$$
\boxed{\|\widetilde U(t)y\|_Y\leq Me^{\omega t}\|y\|_Y}.
$$

Moreover, [strong continuity](../../../functional-analysis.md#strong-continuity) applied separately to $y$ and $Ay$ gives

$$
\|\widetilde U(t)y-y\|_Y
=\|U(t)y-y\|+\|U(t)Ay-Ay\|\longrightarrow0.
$$

Therefore the restrictions form the [semigroup restricted to its generator domain](../../../functional-analysis.md#semigroup-restricted-to-its-generator-domain). Its derivative at zero exists in the [graph norm](../../../functional-analysis.md#graph-norm) exactly when $y\in D(A)$ and $Ay\in D(A)$, namely when $y\in D(A^2)$, and then the derivative is $Ay$. Hence its generator is

$$
\boxed{A|_{D(A^2)},\qquad D(A^2)=\{y\in D(A):Ay\in D(A)\}}.
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The family

$$
\widehat U(t)=e^{-\omega t}U(t)
$$

inherits the identity, [semigroup property](../../../functional-analysis.md#semigroup-property), and [strong continuity](../../../functional-analysis.md#strong-continuity) from $U$, while

$$
\|\widehat U(t)u\|\leq M\|u\|.
$$

Its difference quotient satisfies

$$
\frac{\widehat U(h)u-u}{h}
=e^{-\omega h}\frac{U(h)u-u}{h}
+\frac{e^{-\omega h}-1}{h}u\longrightarrow Au-\omega u
$$

for $u\in D(A)$. Conversely, existence of this limit implies existence of the generator limit for $U$, so $D(\widehat A)=D(A)$ and

$$
\boxed{\widehat A=A-\omega I}.
$$

This is the [exponentially shifted semigroup](../../../functional-analysis.md#exponentially-shifted-semigroup) construction.

The [Hille-Yosida theorem](../../../functional-analysis.md#hille-yosida-theorem) in the uniformly bounded case says that a [linear operator](../../../vector-space.md#linear-operator) $B$ on a [Banach space](../../../banach-space.md) generates a [C0-semigroup](../../../functional-analysis.md#c0-semigroup) with $\|e^{tB}\|\leq M$ if and only if:


- $B$ is a [closed linear operator](../../../functional-analysis.md#closed-linear-operator) whose domain is a [dense subset](../../../topology.md#dense-set) of the [Banach space](../../../banach-space.md);
- $(0,\infty)\subseteq\rho(B)$;
- for every $\lambda>0$ and integer $n\geq1$,


$$
\boxed{\|\lambda^n(\lambda I-B)^{-n}\|\leq M}.
$$

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

A [solution operator for a nonautonomous evolution equation](../../../functional-analysis.md#evolution-family) is an [evolution family](../../../functional-analysis.md#evolution-family) $U(t,s)$ satisfying

$$
U(s,s)=I,
\qquad
U(t,r)U(r,s)=U(t,s),
$$

and, on a suitable common domain $\mathcal D$,

$$
\partial_tU(t,s)u=A(t)U(t,s)u,
\qquad
\partial_sU(t,s)u=-U(t,s)A(s)u.
$$

One applicable nonautonomous generation theorem is the following. Suppose $\mathcal D$ is a dense linear subspace of $H$, each $A(t)$ has domain $\mathcal D$, the family is a [stable family of semigroup generators](../../../functional-analysis.md#stable-family-of-semigroup-generators) with constants $M,0$, and $t\mapsto A(t)$ is continuously differentiable as a map from $[0,T]$ to $\mathcal B(\mathcal D,H)$, where $\mathcal D$ carries one of the uniformly equivalent [graph norms](../../../functional-analysis.md#graph-norm). Then there is a unique [evolution family](../../../functional-analysis.md#evolution-family) such that:

- $(t,s)\mapsto U(t,s)u$ is continuous for every $u\in H$ and $\|U(t,s)\|\leq M$;
- $U(t,s)\mathcal D\subseteq\mathcal D$, with a uniform bound on $U(t,s)$ as an operator on $\mathcal D$;
- for $u\in\mathcal D$, both displayed differential equations hold in $H$.

For the uniform partition $t_j=s+j(t-s)/N$, the [frozen-generator product approximation](../../../functional-analysis.md#frozen-generator-product-approximation) is

$$
U_N(t,s)
=e^{(t_N-t_{N-1})A(t_{N-1})}
\cdots e^{(t_1-t_0)A(t_0)}.
$$

As $N\to\infty$, $U_N(t,s)u\to U(t,s)u$ in the norm of $H$ for every $u\in H$, uniformly for $(t,s)$ in the compact time triangle $0\leq s\leq t\leq T$. This is convergence in the [strong operator topology](../../../functional-analysis.md#strong-operator-topology), rather than convergence in the [operator norm](../../../continuous-dual-space.md#operator-norm).

It remains to verify the second differential equation. The [evolution family](../../../functional-analysis.md#evolution-family) law gives, for $h>0$,

$$
U(t,s+h)u-U(t,s)u
=U(t,s+h)\bigl[u-U(s+h,s)u\bigr].
$$

Divide by $h$. Since $u\in\mathcal D$,

$$
\frac{U(s+h,s)u-u}{h}\longrightarrow A(s)u,
$$

while [strong continuity](../../../functional-analysis.md#strong-continuity) gives $U(t,s+h)A(s)u\to U(t,s)A(s)u$. Therefore

$$
\boxed{\partial_sU(t,s)u=-U(t,s)A(s)u}.
$$

The left derivative follows in the same way, so $s\mapsto U(t,s)u$ is differentiable.

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

Under the [Fourier transform](../../../analysis.md#fourier-transform), the operator $A(t)=\partial_x^3+\phi(t)\partial_x$ is the [Fourier multiplier operator](../../../analysis.md#fourier-multiplier-operator)

$$
\widehat{A(t)u}(\xi)
=i\bigl(\phi(t)\xi-\xi^3\bigr)\widehat u(\xi).
$$

Its symbol is purely imaginary because $\phi$ is real. Consequently $A(t)$ is [skew-adjoint](../../../functional-analysis.md#skew-adjoint-generator) on $L^2(\mathbb R)$ with common domain $H^3(\mathbb R)$ and generates the [strongly continuous unitary group](../../../functional-analysis.md#strongly-continuous-unitary-group)

$$
\widehat{e^{rA(t)}u}(\xi)
=e^{ir(\phi(t)\xi-\xi^3)}\widehat u(\xi).
$$

The [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem) gives $\|e^{rA(t)}u\|_2=\|u\|_2$, so every $A(t)\in\mathcal G(1,0)$. Products of the frozen groups are also unitary; hence this is a [stable family of semigroup generators](../../../functional-analysis.md#stable-family-of-semigroup-generators) with constants $1,0$.

For $u\in H^3(\mathbb R)$,

$$
\|(A(t)-A(s))u\|_2
=|\phi(t)-\phi(s)|\,\|\partial_xu\|_2
\leq|\phi(t)-\phi(s)|\,\|u\|_{H^3}.
$$

Since $\phi\in C^1(\mathbb R)$, the map $t\mapsto A(t)$ is continuously differentiable from $H^3$ to $L^2$. All hypotheses from part f are satisfied, so an [evolution family](../../../functional-analysis.md#evolution-family) exists on every finite interval $[0,T]$.

In this commuting [Fourier multiplier operator](../../../analysis.md#fourier-multiplier-operator) example the solution operator can also be written explicitly:

$$
\boxed{
\widehat{U(t,s)u}(\xi)
=\exp\left(i\left[-(t-s)\xi^3
+\xi\int_s^t\phi(r)\,dr\right]\right)\widehat u(\xi)}.
$$

Its multiplier has absolute value one, directly confirming [strong continuity](../../../functional-analysis.md#strong-continuity), the [evolution family](../../../functional-analysis.md#evolution-family) law, preservation of $H^3$, and the required derivatives. The equation combines the dispersive [Airy equation](../../../integrable-systems.md#airy-equation) with a time-dependent [linear transport equation](../../../partial-differential-equation.md#linear-transport-equation).

<h3 id="1/h">h</h3>

↑ **Parent:** [1](#1)

<h4 id="1/h/solution">Solution</h4>

↑ **Parent:** [H](#1/h)

Let $X=C([0,T];L^2(\mathbb R))$ and define the map suggested by the [variation-of-constants formula](../../../functional-analysis.md#variation-of-constants-formula):

$$
(\Phi u)(t)=U(t,0)u_0+\int_0^tU(t,s)f(s,u(s))\,ds.
$$

The [strong continuity](../../../functional-analysis.md#strong-continuity) of the [evolution family](../../../functional-analysis.md#evolution-family) and the continuity of $f$ imply that $\Phi$ maps $X$ into itself. Because $U(t,s)$ is unitary and $\|f(t,u)\|_2\leq C$,

$$
\|\Phi u(t)\|_2\leq\|u_0\|_2+Ct.
$$

Equip $X$ with the [exponentially weighted supremum norm](../../../functional-analysis.md#exponentially-weighted-supremum-norm)

$$
\|u\|_\alpha=\sup_{0\leq t\leq T}e^{-\alpha t}\|u(t)\|_2.
$$

This equivalent norm makes $X$ a [Banach space](../../../banach-space.md). Using that $f$ is a [globally Lipschitz function](../../../real-analysis.md#globally-lipschitz-function) and that the [unitary operator](../../../vector-space.md#unitary-operator) $U(t,s)$ preserves the norm,

$$
\begin{aligned}
e^{-\alpha t}\|\Phi u(t)-\Phi v(t)\|_2
&\leq L\int_0^te^{-\alpha(t-s)}e^{-\alpha s}\|u(s)-v(s)\|_2\,ds\\
&\leq\frac{L}{\alpha}\|u-v\|_\alpha.
\end{aligned}
$$

Choose $\alpha>L$. Then $\Phi$ is a [contraction mapping](../../../analysis.md#contraction-mapping), so the [Banach fixed-point theorem](../../../analysis.md#contraction-mapping-theorem) gives a unique fixed point $u\in X$. This fixed point is exactly the required [mild solution of an abstract Cauchy problem](../../../functional-analysis.md#mild-solution-of-an-abstract-cauchy-problem):

$$
\boxed{u(t)=U(t,0)u_0+\int_0^tU(t,s)f(s,u(s))\,ds}.
$$

The weighted-norm argument works on the whole prescribed finite interval, so no subdivision of $[0,T]$ is needed.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)

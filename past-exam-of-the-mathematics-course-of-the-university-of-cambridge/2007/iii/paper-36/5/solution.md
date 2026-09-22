<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use $M_0=0$, as implicit in the specified initial value of $Y$. First let $[M]_t=t$. The [Lévy characterization of Brownian motion](../../../../../levy-characterization-of-brownian-motion.md) makes $M$ [Brownian motion](../../../../../brownian-motion-split.md) relative to the given [filtration](../../../../../filtration-probability-theory.md). Set

$$
\varepsilon=\mathbb P(|G|>C+2)>0,\qquad G\sim N(0,1).
$$

On this event at time one, the drift has absolute size at most $C$, while $|Y_0|<1$, so $|Y_1|\ge|M_1|-|Y_0|-C>1$. Continuity forces exit by time one. Therefore

$$
\boxed{\mathbb P(T>1)\le1-\varepsilon.}
$$

The same estimate applies conditionally at each integer time without assuming anything about future drift independence. On $\{T>n\}$, $|Y_n|<1$; if $|M_{n+1}-M_n|>C+2$, the drift bound forces exit by $n+1$. That Brownian increment is independent of $\mathcal F_n$. Hence

$$
\mathbb P(T>n+1\mid\mathcal F_n)\le(1-\varepsilon)\mathbf1_{\{T>n\}},\qquad \mathbb P(T>n)\le(1-\varepsilon)^n.
$$

In particular $T<\infty$ almost surely.

For general $Q$, write $K_t=[M]_t$ and $D_t=\int_0^t A_s\,ds$. Continuity of $Q$ and monotonicity of its integral imply $Q_s\ge0$ at all times outside one null set. The drift condition gives

$$
|D_t-D_s|\le C(K_t-K_s)\qquad(s\le t).
$$

Let $\tau_u=\inf\{t:K_t>u\}$. The divergent clock makes $\tau_u$ finite for every $u$, and its continuity gives $K_{\tau_u}=u$. By the [Dambis-Dubins-Schwarz theorem](../../../../../dambis-dubins-schwarz-theorem.md), $W_u=M_{\tau_u}$ is [Brownian motion](../../../../../brownian-motion-split.md) for $\mathcal G_u=\mathcal F_{\tau_u}$. On intervals where $K$ is constant, both $M$ and $D$ are constant. Thus $d_u=D_{\tau_u}$ is a continuous adapted function of clock time satisfying $|d_v-d_u|\le C(v-u)$. The time-changed process is

$$
\widetilde Y_u=Y_{\tau_u}=Y_0+W_u+d_u.
$$

The unit-clock argument uses only this increment bound on the drift, so its first exit time $S$ obeys $\mathbb P(S>n)\le(1-\varepsilon)^n$. It is finite almost surely, and a corresponding finite ordinary time has $|Y|\ge1$. This proves the [exit with drift controlled by quadratic variation](../../../../../exit-with-drift-controlled-by-quadratic-variation.md) result

$$
\boxed{T<\infty\quad\text{almost surely}.}
$$

This proof needs only a nonnegative measurable bracket density, a continuous divergent integral clock, and the drift increment bound; pointwise continuity of the density is unnecessary. This observation permits the application below with measurable SDE coefficients.

For the multidimensional SDE, put $a_{ij}(x)=\sum_{k=1}^m\sigma_k^i(x)\sigma_k^j(x)$. The [generator of an SDE diffusion](../../../../../generator-of-an-sde-diffusion.md) is

$$
\boxed{Lf(x)=\sum_i b_i(x)\partial_if(x)+\frac12\sum_{i,j}a_{ij}(x)\partial_{ij}f(x).}
$$

For every $f\in C_b^2(\mathbb R^d)$, the [Itô formula](../../../../../ito-s-lemma.md) gives

$$
f(X_t^x)-f(x)-\int_0^tLf(X_s^x)\,ds=\sum_k\int_0^t\nabla f(X_s^x)\cdot\sigma_k(X_s^x)\,dB_s^k.
$$

Bounded derivatives and bounded noise fields make the right side square-integrable on each finite horizon, hence a true [martingale](../../../../../martingale-split.md). This is precisely the defining test-function property of an [L-diffusion](../../../../../diffusion-martingale-problem.md), in the martingale-problem sense.

Now fix $x$ and $\xi\ne0$. Its scalar projection has [martingale](../../../../../martingale-split.md) part $M_t^\xi=\sum_k\int_0^t\langle\xi,\sigma_k(X_s^x)\rangle\,dB_s^k$ and drift $\langle\xi,b(X_s^x)\rangle$. The [uniform ellipticity](../../../../../uniformly-elliptic-operator.md) assumption gives

$$
\frac{d[M^\xi]_t}{dt}=\sum_k\langle\xi,\sigma_k(X_t^x)\rangle^2\ge\lambda|\xi|^2.
$$

Let $B_*=\sup_z|b(z)|$ and take $R>|\langle\xi,x\rangle|$. Rescale the projection by $R$. Its bracket density is at least $\lambda|\xi|^2/R^2$, its absolute drift is at most $B_*|\xi|/R$, and hence that drift is at most $C_R$ times its bracket density, with $C_R=B_*R/(\lambda|\xi|)$. Its clock diverges, so the exit lemma forces it out of $(-1,1)$ in finite time. Equivalently it leaves the slab $|\langle\xi,X_t^x\rangle|<R$. Taking a countable sequence of integer $R$ tending to infinity proves the [projection unboundedness of a uniformly elliptic diffusion](../../../../../projection-unboundedness-of-a-uniformly-elliptic-diffusion.md):

$$
\boxed{\sup_{t\ge0}|\langle\xi,X_t^x\rangle|=\infty\quad\text{almost surely, for each fixed }x,\ \xi\ne0.}
$$

For the final uniqueness result, let $\tau_D=\inf\{t:X_t^x\notin D\}$, with $x\in D$. Since $D$ is bounded, it lies in a finite slab; the preceding finite slab-exit time bounds $\tau_D$ from above. Thus $\tau_D<\infty$ almost surely. Continuity gives $X_{\tau_D}^x\in\partial D$.

Set $h=u-v$. It is bounded, has bounded derivatives, is zero on the boundary, and satisfies $Lh=0$ in $D$. The stopped test-function identity says $h(X_{t\wedge\tau_D}^x)$ is a [martingale](../../../../../martingale-split.md); equivalently it is a bounded [local martingale](../../../../../local-martingale.md), which suffices. Taking expectations and then using bounded convergence as $t\to\infty$ gives

$$
h(x)=\mathbb E_x h(X_{\tau_D})=0.
$$

Therefore the [bounded-domain harmonic uniqueness for a diffusion](../../../../../bounded-domain-harmonic-uniqueness-for-a-diffusion.md) conclusion is

$$
\boxed{u=v\text{ throughout }D.}
$$

In particular the argument supplies the representation $u(x)=\mathbb E_xu(X_{\tau_D})$ and establishes uniqueness without selecting a unique diffusion law.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 36](../../paper-36-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

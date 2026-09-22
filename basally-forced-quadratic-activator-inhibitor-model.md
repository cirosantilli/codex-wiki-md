# Basally forced quadratic activator-inhibitor model

↑ **Parent:** [Reaction–diffusion system](reaction-diffusion-system.md)

A quadratic [activator](activator-in-a-reaction-diffusion-system.md) can have both basal production and activation inhibited by a second species. A normalized example has reaction rates $f(u,v)=1+ru^2/v-u$ and $g(u,v)=q(u^2-v)$, with $r,q>0$ and positive concentrations. At its [spatially homogeneous equilibrium](spatially-homogeneous-equilibrium.md), $v=u^2$, so $u_*=1+r$ and $v_*=(1+r)^2$. Writing $a=(r-1)/(r+1)$, its reaction [Jacobian matrix](jacobian-matrix.md) is $J=\begin{pmatrix}a&-r/(1+r)^2\\2q(1+r)&-q\end{pmatrix}$. Thus $\operatorname{tr}J=a-q$ and $\det J=q>0$, giving linear [asymptotic stability](asymptotic-stability.md) when $q>a$ and instability when $q<a$. Basal production makes $a$ change sign at $r=1$; a positive activation feedback needed for a conventional [Turing instability](turing-instability.md) requires $r>1$.

**Table of contents**

- [Weak focus at the Hopf threshold of a basal activator-inhibitor model](weak-focus-at-the-hopf-threshold-of-a-basal-activator-inhibitor-model.md)
- [Turing threshold of a basally forced quadratic activator-inhibitor model](turing-threshold-of-a-basally-forced-quadratic-activator-inhibitor-model.md)

## ↑ Ancestors (7)

1. [Reaction–diffusion system](reaction-diffusion-system.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-75/1/solution.md)
- [Turing threshold of a basally forced quadratic activator-inhibitor model](turing-threshold-of-a-basally-forced-quadratic-activator-inhibitor-model.md)

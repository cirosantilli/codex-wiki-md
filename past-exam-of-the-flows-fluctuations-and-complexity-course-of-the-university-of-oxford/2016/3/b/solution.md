<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $r>0$, the origin always exists. Its derivative $r-1$ makes it attracting for $0<r<1$ and repelling for $r>1$. Nonzero equilibria solve

$$
r=\frac{\sin x}{x},\qquad |x|\le\frac1r.
$$

They occur in symmetric pairs. On the first positive lobe $0<x<\pi$, the sinc function decreases from one to zero, giving one positive and one negative nonzero equilibrium for $0<r<1$. Both are repelling, since $f'=\sin x/x-\cos x>0$ there. Near $r=1$,

$$
\dot x=(r-1)x+\frac{x^3}{6}+O(x^5),\qquad
x_\pm\simeq\pm\sqrt{6(1-r)}.
$$

The unstable branches meet the stable origin in a [subcritical pitchfork bifurcation](../../../../subcritical-pitchfork-bifurcation.md). At $r=1$ the origin is still nonlinearly repelling because the leading term is $+x^3/6$. For $1<r\le2$ it is the only equilibrium.

For each higher positive-sine lobe $2n\pi<x<(2n+1)\pi$, $n\ge1$, the sinc function has a single positive maximum at $a_n$, where

$$
\boxed{\tan a_n=a_n,\quad 2n\pi<a_n<(2n+\tfrac12)\pi,
\qquad r_n=\frac{\sin a_n}{a_n}=\frac1{\sqrt{1+a_n^2}}.}
$$

If $0<r<r_n$, that lobe has two roots: the smaller positive root is attracting and the larger is repelling, because $f'=-x\,d(\sin x/x)/dx$. Their negative counterparts have the same stability. At $r=r_n$ the pair on each side merges in a [saddle-node bifurcation](../../../../saddle-node-bifurcation.md); the double equilibria are semistable. For $r>r_n$ that lobe contributes none. The first such threshold is about $0.128375$.

For $n\gg1$, put $b_n=(2n+1/2)\pi$; expanding near the sine maximum gives $a_n=b_n-b_n^{-1}+O(b_n^{-3})$ and $r_n\simeq1/b_n$. Away from [bifurcation](../../../../bifurcation.md) values, the exact counting rule for $0<r<1$ and its small-$r$ estimate are

$$
\boxed{N(r)=3+4\#\{n\ge1:r<r_n\},\qquad
N(r)=\frac{2}{\pi r}+O(1)\quad(r\to0^+).}
$$

At a saddle-node threshold, count each merged positive or negative equilibrium once rather than twice. Infinitely many thresholds accumulate at $r=0$, consistent with the infinitely many equilibria in [solution](../a/solution.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the flows, fluctuations and complexity course of the University of Oxford](../../../split.md)
5. [Flows, fluctuations and complexity course of the University of Oxford](../../../../flows-fluctuations-and-complexity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

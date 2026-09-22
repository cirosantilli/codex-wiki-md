<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let attractant reduce signalling activity per methylated [receptor](../../../../receptor-biochemistry.md) by a factor $f\in(0,1)$, so the output is $A=fM$. Before stimulation take $f=1$ and $M=M_0=K_Br/(b-r)$. [Perfect adaptation](../../../../perfect-adaptation.md) requires the final methylated [receptor](../../../../receptor-biochemistry.md) [concentration](../../../../concentration.md) $M'=M_0/f$. With $b'=V'_B[B]$, the new [steady state](../../../../steady-state.md) condition is

$$
r=\frac{b'M'}{K_B+M'},\qquad
\boxed{V'_B=\frac{r}{[B]}\left(1+\frac{fK_B}{M_0}\right)
=V_B\frac{M_0+fK_B}{M_0+K_B}.}
$$

Equivalently $b'=fb+(1-f)r$. Since $f<1$, this reduces demethylation relative to the initial condition. Immediately after binding, activity and tumbling fall. The excess [CheR](../../../../cher.md) flux then increases [receptor methylation](../../../../receptor-methylation.md), compensating the activity loss until $fM'=M_0$. The methylated population must have sufficient remaining capacity to reach $M'$.

Increasing [CheR](../../../../cher.md) [concentration](../../../../concentration.md) raises $r$ and the baseline activity; increasing [CheB](../../../../cheb.md) [concentration](../../../../concentration.md) raises $b$ and lowers it. If the attractant-dependent ratio $c=V'_B/V_B$ remains fixed after such a change, the new pre- and post-step outputs are

$$
A_{\rm before}=\frac{K_Br}{b-r},\qquad
A_{\rm after}=\frac{fK_Br}{cb-r}.
$$

Their equality requires $c=f+(1-f)r/b$. Thus a ratio tuned for one $[R]/[B]$ generally loses [perfect adaptation](../../../../perfect-adaptation.md) when either [enzyme](../../../../enzyme-split.md) level changes independently. For a concrete example, initially $r/b=1/2$ and $f=1/2$ require $c=3/4$; changing $r/b$ to $1/4$ requires $c=5/8$, so keeping $c=3/4$ fails. Proportionally scaling both [enzyme](../../../../enzyme-split.md) levels preserves the ratio and the adaptation condition, while changing response speed. This is fine tuning, rather than [robust perfect adaptation](../../../../robust-perfect-adaptation.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

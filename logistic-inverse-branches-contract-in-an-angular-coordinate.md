# Logistic inverse branches contract in an angular coordinate

↑ **Parent:** [Logistic map](logistic-map.md)

For the real [logistic map](logistic-map.md) $f(x)=\mu x(1-x)$ with $\mu>4$, let $g_L,g_R$ be its two [inverse branches](inverse-branch.md) from $[0,1]$ to the disjoint subintervals on which $0\leq f(x)\leq1$. With the [homeomorphism](homeomorphism.md) $h(u)=\sin^2(\pi u/2)$, these become

$$
G_L(u)=\frac1\pi\arcsin\left(\frac2{\sqrt\mu}\sin\frac{\pi u}{2}\right),\qquad G_R(u)=1-G_L(u).
$$

Direct [differentiation](differentiation.md) gives

$$
|G_{L,R}'(u)|=\frac{\cos(\pi u/2)}{\sqrt\mu\sqrt{1-(4/\mu)\sin^2(\pi u/2)}}\leq\mu^{-1/2},
$$

since $1-(4/\mu)\sin^2v\geq\cos^2v$. Thus length-$n$ [itinerary cylinders](itinerary-cylinder.md) have angular diameter at most $\mu^{-n/2}$, and ordinary diameter at most $(\pi/2)\mu^{-n/2}$ because $|h'|\leq\pi/2$. The [nested interval theorem](nested-interval-theorem.md) then gives exactly one point for each infinite itinerary. This proves the coding by the one-sided [full shift](full-shift.md) even when the ordinary-coordinate [inverse branches](inverse-branch.md) are not contractions.

## ↑ Ancestors (7)

1. [Logistic map](logistic-map.md)
2. [Interval map](interval-map.md)
3. [Discrete dynamical system](discrete-dynamical-system-split.md)
4. [Dynamical systems](dynamical-systems-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-nonlinear-systems-course-of-the-university-of-oxford/2023/3/c/iii/solution.md)

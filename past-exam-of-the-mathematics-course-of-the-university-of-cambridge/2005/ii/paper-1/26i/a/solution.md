<h1 id="26i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $m(t)=E[M_t]$, with finite offspring mean $\rho$. Conditioning on the original cell's first exponential lifetime gives

$$
m(t)=e^{-\mu t}+\int_0^t\mu e^{-\mu s}\rho\,m(t-s)\,ds.
$$

Each of its $k$ offspring starts an independent copy of the process, which explains the factor $\rho$. Changing to $u=t-s$ and differentiating yields $m'=\mu(\rho-1)m$, $m(0)=1$. Hence

$$
\boxed{E[M_t]=e^{\mu(\rho-1)t}.}
$$

Finite-mean truncation and this [integral](../../../../../../integral.md) bound justify finite expectations and exclude explosion in finite time; it is not necessary to assume a bounded offspring count.

For the [probability generating function](../../../../../../probability-generating-function.md), let $P(s)=\sum_{k\ge0}p_ks^k$. Independence of offspring populations gives the conditional generating function $P(\phi_{t-s}(s))$ at a first division time. Thus

$$
\phi_t(s)=se^{-\mu t}+\int_0^t\mu e^{-\mu u}P(\phi_{t-u}(s))\,du,
$$

and differentiation of the changed-variable [integral](../../../../../../integral.md) proves

$$
\boxed{\partial_t\phi_t(s)=\mu\bigl(P(\phi_t(s))-\phi_t(s)\bigr),\qquad\phi_0(s)=s.}
$$

For $0\le s\le1$, the integrand is bounded, so this generating-function argument has the needed convergence even without higher offspring moments.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26I](../../26i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

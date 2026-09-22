<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

Use the first-order [action](../../../../../action.md)

$$
S[q,p]=\int_{t_1}^{t_2}\bigl(p\dot q-H(q,p,t)\bigr)\,dt.
$$

Varying $q$ with fixed endpoints and varying $p$ freely gives

$$
\delta S=\int_{t_1}^{t_2}
\left[(\dot q-H_p)\delta p+(-\dot p-H_q)\delta q\right]dt.
$$

The [principle of stationary action](../../../../../principle-of-stationary-action.md) therefore yields [Hamilton's equations](../../../../../hamilton-s-equations.md)

$$
\dot q=H_p,\qquad\dot p=-H_q.
$$

For $H=p^2+q^{-2}$ these become $\dot q=2p$ and $\dot p=2q^{-3}$. Along their [Hamiltonian flow](../../../../../hamiltonian-flow.md), $H=E$ is conserved and

$$
\frac d{dt}(pq)=\dot p\,q+p\dot q=2q^{-2}+2p^2=2H.
$$

Thus $F=pq-ctH$ is an [integral of motion](../../../../../integral-of-motion.md) exactly when **$c=2$**.

Write its constant value as $F_0$. The surfaces $pq-2tE=F_0$ in extended $(q,p,t)$-space give

$$
pq=F_0+2Et.
$$

Using $Eq^2=p^2q^2+1$,

$$
\boxed{\ q(t)=\pm\sqrt{\frac{(F_0+2Et)^2+1}{E}},
\qquad
p(t)=\frac{F_0+2Et}{q(t)}\ }.
$$

The sign of $q$ is fixed. In [phase space](../../../../../phase-space.md), each energy orbit is one of the two branches

$$
p^2+q^{-2}=E,\qquad
q=\pm(E-p^2)^{-1/2},\qquad |p|<\sqrt E.
$$

Each branch approaches $p=-\sqrt E$ and $p=+\sqrt E$ as $|q|\to\infty$ and turns at $(p,q)=(0,\pm E^{-1/2})$.

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

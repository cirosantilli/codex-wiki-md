<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The Heisenberg update is $ds=U^\dagger sU-s$; the left side of the printed first update relation must be this increment, rather than $s(t)$ itself. For $s=a$, the linear noise term in the supplied stochastic equation is

$$
\sqrt\gamma[a^\dagger\otimes dB-a\otimes dB^\dagger,a]=-\sqrt\gamma\,dB,
$$

by the bosonic [canonical commutation relation](../../../../../../canonical-commutation-relation.md) $[a,a^\dagger]=I$.

The two thermal drift expressions simplify separately to

$$
2a^\dagger a a-aa^\dagger a-a^\dagger a a=-a,\qquad
2aaa^\dagger-aaa^\dagger-aa^\dagger a=a.
$$

The anomalous terms vanish because $[a^\dagger,[a^\dagger,a]]=0$ and $[a,[a,a]]=0$. Hence the factor inside the drift braces is $-(N+1)a+Na=-a$, independent of $N$ and $M$. Therefore

$$
\boxed{da=-\frac\gamma2a\,dt-\sqrt\gamma\,dB_{\mathrm{in}}.}
$$

Equivalently, in the formal white-noise notation of the [cavity-reservoir interaction](../../../../../../cavity-reservoir-interaction.md),

$$
\dot a(t)=-\frac\gamma2a(t)-\sqrt\gamma\,b_{\mathrm{in}}(t).
$$

The dot is a derivative notation for this stochastic differential equation, not a claim that the white-noise field is an ordinary differentiable function.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

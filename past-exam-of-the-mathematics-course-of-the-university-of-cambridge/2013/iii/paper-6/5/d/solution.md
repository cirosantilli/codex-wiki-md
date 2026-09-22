<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Strict positivity throughout [phase space](../../../../../../phase-space.md) is incompatible with [compact support](../../../../../../compact-support.md). The following calculation uses positive smooth rapidly decaying solutions with all displayed [integrals](../../../../../../integral.md) justified; nonnegative cases use the corresponding [entropy](../../../../../../entropy.md) limits where justified.

Write $B=|\mathbb S^2|$ and use integration over $(v,v_*,\sigma)$. The two symmetrized weak collision identities are

$$
\int Q(f,f)\phi(v)\,dv
=\frac1{2B}\int ff_*\bigl(\phi'+\phi_*'-\phi-\phi_*\bigr)\,dv\,dv_*\,d\sigma
$$

and

$$
\int Q(f,f)\phi(v)\,dv
=\frac1{4B}\int(f'f_*'-ff_*)\bigl(\phi+\phi_*-\phi'-\phi_*'\bigr)\,dv\,dv_*\,d\sigma.
$$

They follow from particle interchange and the [angular exchange for elastic collisions](../../../../../../angular-exchange-for-elastic-collisions.md). They are the weak identities needed here; no invalid fixed-angle Jacobian is used.

The [collision invariants](../../../../../../collision-invariant.md) $1$, $v$ and $|v|^2$ obey $\phi'+\phi_*'=\phi+\phi_*$. [Momentum](../../../../../../momentum.md) follows from $v'+v_*'=v+v_*$, and energy from $|v'|^2+|v_*'|^2=|v|^2+|v_*|^2$. Hence

$$
\boxed{\int Q(f,f)\,dv=0,\qquad\int vQ(f,f)\,dv=0,\qquad\int|v|^2Q(f,f)\,dv=0}.
$$

For the [Boltzmann H functional](../../../../../../boltzmann-h-functional.md) $H=\int\!\!\int f\log f\,dx\,dv$, the spatial transport contribution is a boundary [divergence](../../../../../../divergence.md) and the term $\int Q$ is zero. Set $a=f'f_*'$, $b=ff_*>0$. The second weak identity with $\phi=\log f$ gives the [Boltzmann H theorem](../../../../../../h-theorem.md)

$$
\boxed{H'(t)=-\frac1{4B}\int\!\!\int\!\!\int(a-b)\log(a/b)\,dx\,dv\,dv_*\,d\sigma\leq0}.
$$

Indeed this integrand with its negative sign is $b(1-X)\log X$ for $X=a/b>0$, which is nonpositive. The [kinetic H functional](../../../../../../boltzmann-h-functional.md) decreases; the physical [entropy](../../../../../../entropy.md) with opposite sign increases.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

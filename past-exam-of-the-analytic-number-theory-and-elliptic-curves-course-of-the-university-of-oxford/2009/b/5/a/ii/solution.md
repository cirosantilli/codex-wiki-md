<h1 id="b/5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\omega_G=h_G(T)dT$. The pullback through the [formal group](../../../../../../formal-group-law.md) homomorphism is

$$
f^*\omega_G=h_G(f(T))f'(T)dT.
$$

The identity $f(F(X,T))=G(f(X),f(T))$ and the [chain rule](../../../../../../chain-rule.md) show that this pullback is invariant under $F$: translation by $T$ before $f$ becomes translation by $f(T)$ afterward. By part (i) it is a scalar multiple of $\omega_F$. Its coefficient at zero is $h_G(0)f'(0)=f'(0)$, so

$$
\boxed{f^*\omega_G=f'(0)\omega_F.}
$$

Apply this to the multiplication-by-$p$ endomorphism $q(T)=[p](T)$. Since the linear coefficient of $F$ is $X+Y$, repeated addition gives $q'(0)=p$. If $\omega_F=h(T)dT$ with $h(0)=1$, the pullback formula gives

$$
h(q(T))q'(T)=p\,h(T),\qquad
q'(T)\in pR[[T]],
$$

because $h(q(T))$ is a [unit in a ring](../../../../../../unit-in-a-ring.md). Write $q(T)=\sum_{m\geq1}a_mT^m$. Then $ma_m\in pR$ for every $m$. If $p\nmid m$, choose [integers](../../../../../../integer-split.md) $u,v$ with $um+vp=1$. It follows that

$$
a_m=u(ma_m)+vp a_m\in pR.
$$

Choose $b_m\in R$ with $a_m=pb_m$ for those $m$ not divisible by $p$, and define

$$
f(T)=\sum_{p\nmid m}b_mT^m,\qquad
g(T)=\sum_{j\geq1}a_{pj}T^j.
$$

Coefficient comparison now proves

$$
\boxed{[p](T)=pf(T)+g(T^p).}
$$

No cancellation of $p$ was used, so this [prime-multiplication coefficient splitting for formal groups](../../../../../../prime-multiplication-coefficient-splitting-for-formal-groups.md) remains valid when $p$ is a [zero divisor](../../../../../../zero-divisor.md) in $R$.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../../split.md)
7. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)

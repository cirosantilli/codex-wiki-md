<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The quotient.** Evaluation $\mathbb Z[t]\to\mathbb Z[i]$, $t\mapsto i$, is a surjective [ring homomorphism](../../../../ring-homomorphism.md) whose [kernel of a ring homomorphism](../../../../kernel-of-a-ring-homomorphism.md) is $(t^2+1)$. Indeed, division by this [monic polynomial](../../../../monic-polynomial.md) leaves a remainder $a+bt$, and $a+bi=0$ for $a,b\in\mathbb Z$ forces $a=b=0$. Taking the further [quotient ring](../../../../quotient-ring.md) modulo $p$ gives the explicit [isomorphism](../../../../isomorphism.md)

$$
\boxed{\mathbb F_p[t]/(t^2+1)\xrightarrow{\ \sim\ }\mathbb Z[i]/(p),\qquad \overline t\longmapsto\overline i.}
$$

**All fibers, including the generic fiber.** For a point $s\in\operatorname{Spec}\mathbb Z$ with [residue field](../../../../residue-field.md) $\kappa(s)$, its [scheme-theoretic fiber](../../../../scheme-theoretic-fiber.md) is

$$
X_s=\operatorname{Spec}\bigl(\mathbb Z[i]\otimes_{\mathbb Z}\kappa(s)\bigr).
$$

At the [generic point](../../../../generic-point.md) $s=(0)$, the [residue field](../../../../residue-field.md) is $\mathbb Q$, and $t^2+1$ is an [irreducible polynomial](../../../../irreducible-polynomial.md) over $\mathbb Q$, so $X_{(0)}=\operatorname{Spec}\mathbb Q(i)$. For a [closed point](../../../../closed-point.md) $(p)$ the [residue field](../../../../residue-field.md) is $\mathbb F_p$. The permitted criterion for a square root of $-1$ gives three cases. If $p\equiv1\pmod4$, choose $a\in\mathbb F_p$ with $a^2=-1$; the two roots $a,-a$ are distinct, so the [Chinese remainder theorem](../../../../chinese-remainder-theorem.md) gives $\mathbb F_p[t]/(t^2+1)\cong\mathbb F_p\times\mathbb F_p$. If $p\equiv3\pmod4$, the quadratic has no root and is an [irreducible polynomial](../../../../irreducible-polynomial.md), giving the [finite field](../../../../finite-field.md) $\mathbb F_{p^2}$. Finally, in [characteristic](../../../../characteristic-of-a-field.md) two, $t^2+1=(t+1)^2$; setting $\epsilon=t+1$ gives the [dual numbers](../../../../dual-number.md). Thus

$$
\boxed{X_s\cong\begin{cases}
\operatorname{Spec}\mathbb Q(i),&s=(0),\\
\operatorname{Spec}\mathbb F_p\ \amalg\ \operatorname{Spec}\mathbb F_p,&s=(p),\ p\equiv1\pmod4,\\
\operatorname{Spec}\mathbb F_{p^2},&s=(p),\ p\equiv3\pmod4,\\
\operatorname{Spec}\bigl(\mathbb F_2[\epsilon]/(\epsilon^2)\bigr),&s=(2).
\end{cases}}
$$

The split [scheme-theoretic fiber](../../../../scheme-theoretic-fiber.md) has two [closed points](../../../../closed-point.md), represented by $(p,i-a)$ and $(p,i+a)$. The inert [scheme-theoretic fiber](../../../../scheme-theoretic-fiber.md) has one [closed point](../../../../closed-point.md), represented by $(p)$. The [scheme-theoretic fiber](../../../../scheme-theoretic-fiber.md) over $(2)$ has one [closed point](../../../../closed-point.md), represented by $(1+i)$, but is a [nonreduced scheme](../../../../nonreduced-scheme.md): its nonzero element $\epsilon$ is [nilpotent](../../../../nilpotent.md). These descriptions retain the [residue fields](../../../../residue-field.md) and the [nilpotent](../../../../nilpotent.md) structure, which a count of points alone would lose.

**The topology.** The printed PDF says that the nonempty proper [Zariski closed](../../../../zariski-closed-set.md) subsets are finite subsets of $\mathbb Z[i]\setminus\{0\}$. Its points are [prime ideals](../../../../prime-ideal.md), so the intended set is $\operatorname{Spec}\mathbb Z[i]\setminus\{(0)\}$.

Put $R=\mathbb Z[i]$. Since $R$ is a [principal ideal domain](../../../../principal-ideal-domain.md), every nonzero [prime ideal](../../../../prime-ideal.md) is a [maximal ideal](../../../../maximal-ideal.md). Each such [prime ideal](../../../../prime-ideal.md) contains a nonzero [Gaussian integer](../../../../gaussian-integer.md) $z$, and therefore contains the positive integer $z\overline z$. Its contraction to $\mathbb Z$ is consequently a nonzero [prime ideal](../../../../prime-ideal.md) $(p)$, so the [scheme-theoretic fibers](../../../../scheme-theoretic-fiber.md) just computed list all the [closed points](../../../../closed-point.md) of $X$. The sole remaining point is the [generic point](../../../../generic-point.md) $(0)$.

Every proper [Zariski closed](../../../../zariski-closed-set.md) subset is $V((a))$ with $a\ne0$: if its defining [ideal](../../../../ideal.md) were zero, it would be all of $X$. A nonzero nonunit $a$ has a finite [unique factorization](../../../../unique-factorization-in-an-integral-domain.md)

$$
a=u\pi_1^{e_1}\cdots\pi_r^{e_r},\qquad
V((a))=\{(\pi_1),\ldots,(\pi_r)\}.
$$

Here the $\pi_j$ are pairwise nonassociate [prime elements](../../../../prime-element.md). Conversely, any finite set of nonzero [prime ideals](../../../../prime-ideal.md) $\{(\pi_1),\ldots,(\pi_r)\}$ equals $V((\pi_1\cdots\pi_r))$; the empty set is $V((1))$. Therefore

$$
\boxed{\begin{gathered}
X=\{(0)\}\ \cup\ \{\text{nonzero prime ideals of }\mathbb Z[i]\},\\
\text{proper closed subsets of }X=\text{finite subsets of its closed points}.
\end{gathered}}
$$

In particular, the closure of the [generic point](../../../../generic-point.md) is $X$, and every nonempty [open subset](../../../../open-set.md) contains that [generic point](../../../../generic-point.md) and all but finitely many [closed points](../../../../closed-point.md).

**A nonidentity automorphism.** [Complex conjugation](../../../../complex-conjugation.md)

$$
c:R\longrightarrow R,\qquad a+bi\longmapsto a-bi,
$$

is a [ring automorphism](../../../../ring-automorphism.md) fixing $\mathbb Z$. It induces the [automorphism](../../../../automorphism.md) $\sigma=\operatorname{Spec}(c)$ over $\operatorname{Spec}\mathbb Z$. Since $c(i)=-i\ne i$, this is not the identity [morphism of schemes](../../../../morphism-of-schemes.md). On the [generic fiber](../../../../generic-fiber.md) it is the nontrivial [field automorphism](../../../../field-automorphism.md) of $\mathbb Q(i)/\mathbb Q$. On a split [scheme-theoretic fiber](../../../../scheme-theoretic-fiber.md) it swaps the two [closed points](../../../../closed-point.md), since $i-a$ maps to $-(i+a)$. On an inert [scheme-theoretic fiber](../../../../scheme-theoretic-fiber.md) it fixes the only point but induces the nonidentity [finite-field Frobenius automorphism](../../../../finite-field-frobenius-automorphism.md) $z\mapsto z^p$ on its [residue field](../../../../residue-field.md), because $i^p=-i$. On the [scheme-theoretic fiber](../../../../scheme-theoretic-fiber.md) over $(2)$ it is the identity on the entire [scheme](../../../../scheme.md): $-i=i$ in $R/(2)$, so $\epsilon=i+1$ is fixed. Thus

$$
\boxed{\sigma:\quad\text{generic conjugation; split points exchanged; inert Frobenius; identity over }2.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Right multiplication gives a right action $(Hx)\cdot g=Hxg$. To obtain a [homomorphism](../../../../homomorphism.md) into [permutations](../../../../permutation.md) with the usual function-composition convention, use the associated left action

$$
\rho(g)(Hx)=Hxg^{-1}.
$$

This is well-defined: replacing $x$ by $hx$, $h\in H$, does not change the image [coset](../../../../coset.md). Moreover $\rho(g)\rho(k)(Hx)=Hxk^{-1}g^{-1}=\rho(gk)(Hx)$, and each map is bijective with inverse $\rho(g^{-1})$.

An element $g$ is in the [kernel](../../../../kernel-of-a-linear-map-split.md) precisely when $Hxg^{-1}=Hx$ for every $x\in G$. This says $xg^{-1}x^{-1}\in H$, equivalently $g\in x^{-1}Hx$. Hence

$$
\boxed{\ker\rho=\bigcap_{x\in G}x^{-1}Hx.}
$$

This is the largest [normal subgroup](../../../../normal-subgroup.md) of $G$ contained in $H$.

Now the index of $H$ is $q$, so $G/\ker\rho$ embeds into $S_q$. Its order therefore divides $q!$. Since $p>q$ is [prime](../../../../prime-number-split.md), $p$ does not divide $q!$. From $|G|=pq$ it follows that $p$ divides $|\ker\rho|$. But $\ker\rho\subseteq H$ and $|H|=p$, forcing $\ker\rho=H$. Therefore **$H$ is normal**.

For the last case let $H=\langle b\rangle$. Normality makes [conjugation](../../../../conjugation.md) by $a$ an [automorphism](../../../../automorphism.md), so $a^{-1}ba=b^r$ with $r\in\{1,2,3,4\}$. Applying it twice and using $a^2=1$ gives $b=b^{r^2}$, so $r^2\equiv1\pmod5$. Thus $(r-1)(r+1)\equiv0\pmod5$, and

$$
\boxed{a^{-1}ba=b\ \text{or}\ b^{-1}.}
$$

Both possibilities are allowed; the order assumptions alone do not force the inverse case.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

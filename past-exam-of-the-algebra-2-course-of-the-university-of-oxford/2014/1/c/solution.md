<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take a reduced fraction $a/b\in R$, with $b\neq0$. Since $\gcd(a,b)=1$, [Bézout's identity](../../../../bezout-s-identity.md) supplies integers $u,v$ with $ua+vb=1$. As the [subring](../../../../subring.md) $R$ contains all [integers](../../../../integer-split.md),

$$
\boxed{\frac1b=u\frac ab+v\in R.}
$$

Thus a denominator appearing in a reduced fraction in $R$ is automatically a [unit](../../../../unit-in-a-ring.md) of $R$.

Now let $I\cap\mathbb Z=d\mathbb Z$. Because $d\in I$, the [principal ideal](../../../../principal-ideal.md) $dR$ is contained in $I$. For the reverse inclusion, take $x\in I$ and write $x=a/b$ in lowest terms. Multiplying by $b\in R$ gives $a=bx\in I\cap\mathbb Z=d\mathbb Z$, so $a=dc$ for some integer $c$. The preceding result gives $1/b\in R$, whence

$$
x=\frac ab=d\left(\frac cb\right)\in dR.
$$

Therefore

$$
\boxed{I=dR.}
$$

This includes $d=0$: the same argument forces every $x\in I$ to be zero. This is the [ideals of subrings of the rational numbers](../../../../ideals-of-subrings-of-the-rational-numbers.md) property; every such [ring](../../../../ring.md) is a [principal ideal domain](../../../../principal-ideal-domain.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the algebra 2 course of the University of Oxford](../../../split.md)
5. [Algebra 2 course of the University of Oxford](../../../../algebra-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

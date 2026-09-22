# Torsion submodule

↑ **Parent:** [Torsion module](torsion-module.md)

For a [module](module-mathematics.md) $M$ over an [integral domain](integral-domain.md) $R$, its torsion submodule is

$$
T(M)=\{m\in M:rm=0\text{ for some }0\ne r\in R\}.
$$

This is a [submodule](submodule.md). If $rm=0$ and $sn=0$ with $r,s\ne0$, then $rs(m+n)=0$ and $rs\ne0$; also $r(am)=a(rm)=0$ for every $a\in R$. The [integral domain](integral-domain.md) hypothesis supplies both the nonzero product and commutativity. These are the conventions of [Keith Conrad's Introductory Notes on Modules, section 4](https://kconrad.math.uconn.edu/blurbs/linmultialg/moduleintro.pdf).

A mixed example is the [direct sum](direct-sum.md) $M=\mathbb Z^2\oplus\mathbb Z/6\mathbb Z$. If a nonzero [integer](integer.md) kills $(a,b,\overline c)$, then $a=b=0$. Conversely, $6$ kills every $(0,0,\overline c)$. Thus

$$
T(M)=\{(0,0,\overline c):\overline c\in\mathbb Z/6\mathbb Z\},\qquad M/T(M)\cong\mathbb Z^2.
$$

The [torsion submodule](torsion-submodule.md) isolates the finite-order part while the [quotient module](quotient-module.md) keeps the independent [integer](integer.md) directions. In general $M/T(M)$ is a [torsion-free module](torsion-free-module.md): if $r(m+T(M))=0$ with $r\ne0$, some $s\ne0$ kills $rm$, so $sr\ne0$ kills $m$.

The hypothesis matters. In the [ring](ring.md) $R=\mathbb Z/6\mathbb Z$ viewed as a [module](module-mathematics.md) over itself, the elements $\overline2$ and $\overline3$ are killed by nonzero scalars $\overline3$ and $\overline2$, but their sum $\overline5$ is a [unit](unit-in-a-ring.md) and is killed by no nonzero scalar. Thus using arbitrary nonzero scalars in a [ring](ring.md) with [zero divisors](zero-divisor.md) need not give a [submodule](submodule.md). A common broader convention uses [regular elements of a ring](regular-element-of-a-ring.md) as annihilators; the [integral domain](integral-domain.md) convention here avoids that ambiguity.

**Table of contents**

- [Torsion element of a module](torsion-element-of-a-module.md)

## ↑ Ancestors (8)

1. [Torsion module](torsion-module.md)
2. [Module (mathematics)](module-mathematics.md)
3. [Module theory](module-theory-split.md)
4. [Commutative algebra](commutative-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Invariant factor of a finitely generated module](invariant-factor-of-a-finitely-generated-module.md)
- [Maximal torsion-free quotient](maximal-torsion-free-quotient.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-4/2f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-2/11g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-2/2g/solution.md)
- [Torsion element of a module](torsion-element-of-a-module.md)
- [Torsion-free module](torsion-free-module.md)
- [Torsion submodule](torsion-submodule.md)

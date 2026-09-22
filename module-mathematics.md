# Module (mathematics)

↑ **Parent:** [Module theory](module-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Module_(mathematics))

A left $R$-module consists of an [abelian group](abelian-group.md) $(M,+)$ and [scalar multiplication](scalar-multiplication.md) $R\times M\to M$, written $(r,m)\mapsto rm$, where $R$ is a [ring](ring.md) with [identity element](identity-element.md) $1$. For every $r,s\in R$ and $m,n\in M$, require

$$
r(m+n)=rm+rn,\qquad (r+s)m=rm+sm,\qquad (rs)m=r(sm),\qquad 1m=m.
$$

The [module](module-mathematics.md) elements can be added to one another and multiplied by scalars; a product of two [module](module-mathematics.md) elements is not part of the definition. These conventions agree with [Keith Conrad's Introductory Notes on Modules, Definition 1.2](https://kconrad.math.uconn.edu/blurbs/linmultialg/moduleintro.pdf). For a [noncommutative ring](noncommutative-ring.md), the side matters: a right [module](module-mathematics.md) instead has $(mr)s=m(rs)$. Over a [commutative ring](commutative-ring.md), the two conventions agree.

Over a [field](field.md) $k$, these are exactly the [vector space axioms](vector-space-axioms.md). A nonzero $a\in k$ has a [multiplicative inverse](multiplicative-inverse.md), so $am=0$ implies $m=a^{-1}(am)=0$. Over the [integers](integer.md), $2$ has no [multiplicative inverse](multiplicative-inverse.md): $2x=1$ has no solution in $\mathbb Z$. In the [module](module-mathematics.md) $\mathbb Z/6\mathbb Z$, division can also lose uniqueness: $2\overline1=2\overline4=\overline2$. A [ring](ring.md) element which is a [unit](unit-in-a-ring.md) still acts invertibly on every [module](module-mathematics.md); the difficulty lies with scalars which are not [units](unit-in-a-ring.md).

**Table of contents**

- [Abelian groups as integer modules](abelian-groups-as-integer-modules.md)
- [Polynomial module from a linear operator](polynomial-module-from-a-linear-operator.md)
- [Finitely presented module](finitely-presented-module.md)
  - [Fitting ideal](fitting-ideal.md)
- [Locally free module](locally-free-module.md)
- [Finite presentation of a module](finite-presentation-of-a-module.md)
- [Change of rings](change-of-rings.md)
  - [Coextension of scalars](coextension-of-scalars.md)
  - [Extension of scalars](extension-of-scalars.md)
  - [Restriction of scalars](restriction-of-scalars.md)
- [Module isomorphism](module-isomorphism.md)
- [Torsion module](torsion-module.md)
  - [Torsion submodule](torsion-submodule.md)
    - [Torsion element of a module](torsion-element-of-a-module.md)
- [Module homomorphism](module-homomorphism.md)
  - [Module endomorphism](module-endomorphism.md)
    - [Module automorphism](module-automorphism.md)
  - [Module retraction](module-retraction.md)
  - [Endomorphism ring](endomorphism-ring.md)
    - [Local endomorphism ring](local-endomorphism-ring.md)
    - [Semisimple quotient of a module endomorphism algebra](semisimple-quotient-of-a-module-endomorphism-algebra.md)
    - [Brick module](brick-module.md)
      - [Ringel lemma on bricks](ringel-lemma-on-bricks.md)
        - [Proof of Ringel lemma on bricks](proof-of-ringel-lemma-on-bricks.md)
- [Submodule](submodule.md)
  - [Essential submodule](essential-submodule.md)
    - [Essential right ideal](essential-right-ideal.md)
      - [A regular principal right ideal in a right Noetherian ring is essential](a-regular-principal-right-ideal-in-a-right-noetherian-ring-is-essential.md)
    - [Essential extension](essential-extension.md)
  - [Primary decomposition](primary-decomposition.md)
    - [Lasker–Noether theorem](lasker-noether-theorem.md)
    - [Primary submodule](primary-submodule.md)

## ↑ Ancestors (6)

1. [Module theory](module-theory-split.md)
2. [Commutative algebra](commutative-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

# Discontinuous additive function

↑ **Parent:** [Additive function](additive-function.md)

Assuming the [axiom of choice](axiom-of-choice.md), [Cauchy's functional equation](cauchy-s-functional-equation.md) has solutions that are not [linear maps](linear-map.md) over the [real numbers](real-number.md). Regard $\mathbb R$ as a [vector space over the rational numbers](vector-space-over-the-rational-numbers.md). Because $\sqrt2$ is an [irrational number](irrational-number.md), $1$ and $\sqrt2$ are [linearly independent](linear-independence.md) over $\mathbb Q$. [Zorn's lemma](zorn-s-lemma.md) extends them to a [Hamel basis](basis.md) $B$; assigning arbitrary real outputs to its [basis vectors](basis-vector.md) and extending by finite rational [linear combinations](linear-combination.md) gives an [additive function](additive-function.md).[§4, printed pp. 19–20, Corollaries 4.2 and 4.5: basis extension and an additive map not of the form cx](zorn%E2%80%99s-lemma-and-some-applications-by-keith-conrad.md)

For a particular choice, assign $g(1)=3$ and $g(b)=0$ for every $b\in B\setminus\{1\}$. Every [real number](real-number.md) has a unique finite [linear combination](linear-combination.md) $x=\sum_{b\in F}q_bb$ with $F\subset B$ finite and $q_b\in\mathbb Q$. Define

$$
g(x)=3q_1,
$$

where the coefficient $q_1$ is zero if $1\notin F$. The uniqueness of the [Hamel basis](basis.md) representation makes this definition unambiguous, and adding the coefficients proves $g(x+y)=g(x)+g(y)$. On the rational two-dimensional [vector subspace](vector-subspace.md) spanned by $1$ and $\sqrt2$, the rule is particularly simple:

$$
g(p+q\sqrt2)=3p\qquad(p,q\in\mathbb Q).
$$

For instance, $u=2/3+\sqrt2$ and $v=5/6-2\sqrt2$ give $g(u)=2$, $g(v)=5/2$, and $g(u+v)=9/2$. Thus the map still preserves [addition](addition.md), even though $g(\sqrt2)=0\ne3\sqrt2$ rules out being a [linear map](linear-map.md) over the [real numbers](real-number.md).

The rational approximants $q_n$ from [additive function continuous at one point is linear](additive-function-continuous-at-one-point-is-linear.md) expose the failure of [continuity](continuous-function.md): $q_n\to\sqrt2$ but $g(q_n)=3q_n\to3\sqrt2\ne g(\sqrt2)$. Moreover $h_n=\sqrt2-q_n\to0$ while $g(h_n)=-3q_n\to-3\sqrt2$. The map is [continuous](continuous-function.md) nowhere, since [continuity](continuous-function.md) at any point would imply [additive function continuous at one point is linear](additive-function-continuous-at-one-point-is-linear.md). It is unbounded on every [interval](interval-mathematics.md) of positive length by [additive function bounded on an interval is linear](additive-function-bounded-on-an-interval-is-linear.md).

The [axiom of choice](axiom-of-choice.md) is used to obtain the [Hamel basis](basis.md); the coefficient rule does not provide an explicit way to find the representation of an arbitrary [real number](real-number.md). A plot sampled only at [rational numbers](rational-number.md) would show exactly the same values as $f(x)=3x$, so that plot cannot reveal this [discontinuous additive function](discontinuous-additive-function.md).

## ↑ Ancestors (7)

1. [Additive function](additive-function.md)
2. [Cauchy's functional equation](cauchy-s-functional-equation.md)
3. [Functional equation](functional-equation.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Cauchy's functional equation](cauchy-s-functional-equation.md)
- [Discontinuous additive function](discontinuous-additive-function.md)
- [Rational homogeneity of an additive function](rational-homogeneity-of-an-additive-function.md)

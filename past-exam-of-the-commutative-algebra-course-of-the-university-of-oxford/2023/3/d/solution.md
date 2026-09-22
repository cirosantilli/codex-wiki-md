<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $N$ be the [nilradical](../../../../nilradical.md) of $R$. By [b](../b.md), the [reduced locus of a ring](../../../../reduced-locus-of-a-ring.md) is

$$
\mathcal R=\{\mathfrak p\in\operatorname{Spec}R:NR_{\mathfrak p}=0\}.
$$

The [Noetherian ring](../../../../noetherian-ring.md) hypothesis makes the [ideal](../../../../ideal.md) $N$ finitely generated; write $N=(n_1,\ldots,n_t)$. Fix $\mathfrak p\in\mathcal R$. For every $i$, the [vanishing criterion in a module localization](../../../../vanishing-criterion-in-a-module-localization.md) gives $s_i\notin\mathfrak p$ with $s_in_i=0$. The product $f=s_1\cdots s_t$ lies outside the [prime ideal](../../../../prime-ideal.md) $\mathfrak p$ and satisfies $fN=0$. When $N=0$, take $f=1$.

For every [prime ideal](../../../../prime-ideal.md) $\mathfrak q$ in the [distinguished open set](../../../../distinguished-open-set.md)

$$
D(f)=\{\mathfrak q\in\operatorname{Spec}R:f\notin\mathfrak q\},
$$

the element $f/1$ is a [unit](../../../../unit-in-a-ring.md) in $R_{\mathfrak q}$. The equality $fN=0$ therefore implies $NR_{\mathfrak q}=0$, so $R_{\mathfrak q}$ is [reduced](../../../../reduced-ring.md). Thus $\mathfrak p\in D(f)\subseteq\mathcal R$, proving that $\mathcal R$ is a [Zariski-open subset](../../../../zariski-open-set.md) of the [spectrum of a ring](../../../../spectrum-of-a-commutative-ring.md).

More precisely, let $A=\operatorname{Ann}_R(N)$, the [annihilator of a module](../../../../annihilator-of-a-module.md) $N$. The argument shows that $NR_{\mathfrak p}=0$ if and only if some $f\in A$ lies outside $\mathfrak p$. Hence

$$
\boxed{\mathcal R=\bigcup_{f\in\operatorname{Ann}_R(N)}D(f)
=\operatorname{Spec}R\setminus V(\operatorname{Ann}_R(N)).}
$$

Equivalently, the complement is the [support of a module](../../../../support-of-a-module.md) $N$. This is [vanishing of a finitely generated module near a prime](../../../../vanishing-of-a-finitely-generated-module-near-a-prime.md) applied to $N$: its finite generation lets the separately chosen denominators be combined into one element annihilating all of $N$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the commutative algebra course of the University of Oxford](../../../split.md)
5. [Commutative algebra course of the University of Oxford](../../../../commutative-algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

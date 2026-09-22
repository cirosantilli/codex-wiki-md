<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Normalize the [discrete valuations](../../../../../discrete-valuation.md) so a [uniformiser](../../../../../uniformizer.md) has value one, and write $k_K,k_L$ for the [residue fields](../../../../../residue-field.md). The [ramification index](../../../../../ramification-index.md) $e$ is specified by $v_L|_K=e\,v_K$, and the [residue degree](../../../../../residue-degree.md) is $f=[k_L:k_K]$. For finite extensions of complete discretely valued fields, $[L:K]=ef$. One way to see the degree equality is that $\mathcal O_L$ is a finite free $\mathcal O_K$-module of rank $[L:K]$; reduction modulo a [uniformiser](../../../../../uniformizer.md) of $K$ has $e$ successive quotients isomorphic to $k_L$, hence dimension $ef$ over $k_K$.

An [unramified extension](../../../../../unramified-extension.md) has $e=1$ and separable residue extension, equivalently $[L:K]=f$ with separable residue extension. A [totally ramified extension](../../../../../totally-ramified-extension.md) has $f=1$, equivalently $[L:K]=e$. The separability condition in the [unramified extension](../../../../../unramified-extension.md) definition matters if the [residue field](../../../../../residue-field.md) is imperfect; it is automatic for finite [residue fields](../../../../../residue-field.md).

Suppose $L/K$ is unramified. Choose a [primitive element of a field extension](../../../../../primitive-element-of-a-field-extension.md) $\bar x$ for the finite separable extension $k_L/k_K$ and lift it to $x\in\mathcal O_L$. Since the residue degree of $K(x)/K$ is at least $[k_K(\bar x):k_K]=[L:K]$, necessarily $K(x)=L$. Its monic [minimal polynomial of an algebraic element](../../../../../minimal-polynomial-of-an-algebraic-element.md) $f_x$ has coefficients in $\mathcal O_K$. Its reduction has degree $[L:K]$ and annihilates $\bar x$, whose minimal polynomial over $k_K$ has that same degree. The two coincide, so $\bar f_x$ is separable.

Conversely, suppose $L=K(x)$, $x\in\mathcal O_L$, and $\bar f_x$ is separable. It must be irreducible: otherwise its coprime factors lift by the factorization form of [Hensel's lemma](../../../../../hensel-s-lemma.md), contradicting irreducibility of $f_x$. Hence $\bar x$ has degree $[L:K]$ over $k_K$. The degree equality forces $f=[L:K]$ and $e=1$, and the residue extension is separable. We have proved the [unramified generator criterion with separable reduction](../../../../../unramified-generator-criterion-with-separable-reduction.md):

$$
\boxed{L/K\text{ unramified}\iff L=K(x),\ x\in\mathcal O_L,\ \bar f_x\text{ separable}.}
$$

Now let $k_L=\mathbb F_q$, $q=p^f$. Every element of $k_L^\times$ is a simple root of $X^{q-1}-1$, whose derivative is a unit at each root. [Hensel's lemma](../../../../../hensel-s-lemma.md) lifts each of these $q-1$ elements uniquely to a root in $\mathcal O_L^\times$. Thus **$L$ contains all $q-1$ roots of $X^{q-1}-1$**; these are the nonzero [Teichmuller lifts](../../../../../teichmuller-representative.md).

More generally, a [root of unity](../../../../../root-of-unity.md) of order prime to $p$ reduces injectively into $k_L^\times$. Indeed, if such a root reduces to $1$, uniqueness in [Hensel's lemma](../../../../../hensel-s-lemma.md) for $X^m-1$ makes it equal to $1$. Consequently every prime-to-$p$ order divides $q-1$.

A root whose order has a nontrivial $p$-part produces a primitive $p$th [root of unity](../../../../../root-of-unity.md) $\zeta$. It reduces to $1$ in characteristic $p$. Since

$$
p=\prod_{j=1}^{p-1}(1-\zeta^j),\qquad \frac{1-\zeta^j}{1-\zeta}=1+\zeta+\cdots+\zeta^{j-1}\equiv j\pmod{\mathfrak p_L},
$$

all the factors have the same positive integral [valuation](../../../../../valuation.md). Hence

$$
e(L/\mathbb Q_p)=v_L(p)=(p-1)v_L(1-\zeta)\geq p-1.
$$

This is the [ramification bound for a primitive pth root of unity](../../../../../ramification-bound-for-a-primitive-pth-root-of-unity.md). Therefore

$$
\boxed{e<p-1\implies\mu(L)=\mu_{p^f-1}.}
$$

For $p=2$ the hypothesis $e<1$ cannot occur, so that instance is vacuous rather than a claim excluding the ever-present root $-1$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

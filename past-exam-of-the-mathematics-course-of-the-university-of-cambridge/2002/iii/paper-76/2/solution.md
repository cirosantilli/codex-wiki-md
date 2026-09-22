<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [fixed-point combinator](../../../../../fixed-point-combinator.md) is a closed [lambda term](../../../../../lambda-term.md) $Z$ such that $ZF\equiv_\beta F(ZF)$ for every [lambda term](../../../../../lambda-term.md) $F$. It suffices to check this for a fresh [free variable](../../../../../free-variable.md) $f$, since [capture-avoiding substitution](../../../../../capture-avoiding-substitution.md) then gives every instance. Take

$$
\boxed{G=\lambda z f.f(zf).}
$$

If $GZ\equiv_\beta Z$, applying both sides to $f$ gives $Zf\equiv_\beta f(Zf)$. Conversely suppose $Z$ is a [fixed-point combinator](../../../../../fixed-point-combinator.md). Its application to a fresh $f$ has a [head normal form](../../../../../head-normal-form.md), because it is [beta equivalent](../../../../../beta-equivalence.md) to $f(Zf)$. Since $Z$ is closed, head reduction of $Zf$ must first expose a [lambda abstraction](../../../../../lambda-abstraction.md) in $Z$ itself. Thus $Z\to_\beta^*\lambda u.P$, and

$$
\lambda f.Zf\equiv_\beta\lambda f.P[u:=f]\equiv_\alpha\lambda u.P\equiv_\beta Z.
$$

This establishes the needed abstraction equality by [beta reduction](../../../../../beta-reduction.md), without assuming [eta conversion](../../../../../eta-conversion.md). Abstracting $Zf\equiv_\beta f(Zf)$ now gives $Z\equiv_\beta\lambda f.f(Zf)\equiv_\beta GZ$.

Two examples are the [Curry fixed-point combinator](../../../../../curry-fixed-point-combinator.md) and the [Turing fixed-point combinator](../../../../../turing-fixed-point-combinator.md):

$$
Y=\lambda f.(\lambda x.f(xx))(\lambda x.f(xx)),\qquad D=\lambda x f.f(xxf),\qquad\Theta=DD.
$$

Writing $A_f=\lambda x.f(xx)$, we have $Yf\to_\beta A_fA_f\to_\beta f(A_fA_f)\equiv_\beta f(Yf)$, while $\Theta f\to_\beta^2 f(\Theta f)$. Different displayed syntax alone would not prove that the two [combinators](../../../../../combinator.md) are distinct under [beta equivalence](../../../../../beta-equivalence.md). Here is a reduct invariant that does. Every finite reduct of $Y$ is $\lambda f.f^n(A_fA_f)$, up to [alpha equivalence](../../../../../alpha-equivalence.md): $A_f$ is beta-normal and the one remaining [beta-redex](../../../../../beta-redex.md) is its self-application. No such reduct contains the closed subterm $DD$.

Every finite reduct of $\Theta$, in contrast, retains a closed subterm $DD$. The contraction $DD\to\lambda f.f(DDf)$ recreates one. The only other redexes created by these expansions are abstractions applied to variables; contracting them substitutes a variable, so preserves any closed $DD$ inside their bodies. This describes all redexes inductively: expansion inserts only a variable-headed application and a copy of $DD$, and a variable substitution preserves that description. Thus every finite reduct contains $DD$. A common reduct of $Y$ and $\Theta$ is impossible, so the [Church-Rosser theorem](../../../../../church-rosser-theorem.md) proves **$Y\not\equiv_\beta\Theta$**.

Finally put $P=ZK$, with $K=\lambda xy.x$. The [fixed-point combinator](../../../../../fixed-point-combinator.md) equation gives

$$
P\equiv_\beta KP\equiv_\beta\lambda y.P,
$$

where $y$ is fresh. If $P$ had a [head normal form](../../../../../head-normal-form.md) with $n$ leading abstractions, then $\lambda y.P$ would have one with $n+1$. A reduct of a [head normal form](../../../../../head-normal-form.md) preserves its initial abstraction count and variable-headed spine: only its argument subterms can still contract. These two [head normal forms](../../../../../head-normal-form.md) therefore cannot have a common reduct, contradicting the [Church-Rosser theorem](../../../../../church-rosser-theorem.md). Hence **$ZK$ is unsolvable**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

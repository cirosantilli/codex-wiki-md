<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume the [coequalizers](../../../../../../coequalizer.md) from part (b) exist and write them $q_a:FA\to L(A,a)$. The underlying arrow of the comparison-adjunction unit is

$$
\lambda_a=Gq_a\eta_A:A\to GL(A,a).
$$

We first relate it to the [monad algebra](../../../../../../algebra-for-a-monad.md) action. [Naturality](../../../../../../naturality.md) of $\eta$, the [coequalizer](../../../../../../coequalizer.md) equation and a [monad](../../../../../../monad.md) unit law give

$$
\begin{aligned}
\lambda_a a
&=Gq_a\eta_A a=Gq_a,Ta\,\eta_{TA}\\
&=G(q_aFa)\eta_{TA}=G(q_a\varepsilon_{FA})\eta_{TA}\\
&=Gq_a\mu_A\eta_{TA}=Gq_a.
\end{aligned}
$$

In $\mathcal C$, $a:TA\to A$ is itself a [split coequalizer](../../../../../../split-coequalizer.md) of $Ta,\mu_A:T^2A\rightrightarrows TA$. Indeed,

$$
aTa=a\mu_A,\quad a\eta_A=1_A,\quad
\mu_A\eta_{TA}=1_{TA},\quad Ta\eta_{TA}=\eta_Aa.
$$

For an explicit universal-property proof, if $r:TA\to X$ satisfies $rTa=r\mu_A$, then $s=r\eta_A$ obeys

$$
sa=r\eta_Aa=rTa\eta_{TA}=r\mu_A\eta_{TA}=r.
$$

Its uniqueness follows by composing any equation $sa=r$ with $\eta_A$.

Now $Gq_a$ equalizes $Ta$ and $\mu_A$. If it is a [coequalizer](../../../../../../coequalizer.md), then $a$ and $Gq_a$ are [coequalizers](../../../../../../coequalizer.md) of the same pair. Their unique comparison map is $\lambda_a$, since $\lambda_a a=Gq_a$, and is therefore invertible. Conversely, if $\lambda_a$ is invertible, $Gq_a=\lambda_a a$ is an isomorphic copy of the [coequalizer](../../../../../../coequalizer.md) $a$, so it is a [coequalizer](../../../../../../coequalizer.md) too.

The [forgetful functor](../../../../../../forgetful-functor.md) $\mathcal C^T\to\mathcal C$ reflects [isomorphisms](../../../../../../isomorphism.md): if an [monad algebra](../../../../../../algebra-for-a-monad.md) [morphism](../../../../../../morphism.md) $u$ has an inverse as an underlying arrow, the equation $ua=bTu$ rearranges to $u^{-1}b=aT(u^{-1})$, making that inverse an [monad algebra](../../../../../../algebra-for-a-monad.md) [morphism](../../../../../../morphism.md). Thus underlying invertibility here is exactly invertibility of the unit component. For all [monad algebras](../../../../../../algebra-for-a-monad.md) together, the [comparison-adjunction unit criterion](../../../../../../comparison-adjunction-unit-criterion.md) is

$$
\boxed{\lambda\text{ is invertible}\quad\Longleftrightarrow\quad
G\text{ preserves every specified coequalizer }q_a.}
$$

Equivalently, the necessary-and-sufficient conditions for a [left adjoint](../../../../../../adjoint-functors.md) with invertible unit are existence of the [coequalizers](../../../../../../coequalizer.md) in part (b) and their preservation by $G$. No preservation of arbitrary [coequalizers](../../../../../../coequalizer.md) is required.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [8](../../8.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For $F\dashv G$ with unit $\eta$ and counit $\varepsilon$, the [monad induced by an adjunction](../../../../../monad-induced-by-an-adjunction.md) is

$$
T=GF,\qquad \mu=G\varepsilon F,
$$

with unit $\eta$. An [algebra for a monad](../../../../../algebra-for-a-monad.md) is $(A,a:TA\to A)$ satisfying $a\eta_A=1_A$ and $aT(a)=a\mu_A$.

The [Eilenberg-Moore comparison functor](../../../../../eilenberg-moore-comparison-functor.md) is

$$
K:\mathcal D\to\mathcal C^T,\qquad K(D)=(GD,G\varepsilon_D).
$$

If $\mathcal D$ has coequalizers of reflexive pairs, define

$$
FTA\mathrel{\substack{\xrightarrow{Fa}\\[-2pt]\xrightarrow[\varepsilon_{FA}]{} }}FA
\xrightarrow{q}L(A,a)
$$

for a $T$-algebra $(A,a)$. The pair has common section $F\eta_A$. Maps $L(A,a)\to D$ correspond by the coequalizer property and the adjunction exactly to algebra morphisms $(A,a)\to K(D)$, naturally in both variables. Hence this is the [Left adjoint to the Eilenberg-Moore comparison functor](../../../../../left-adjoint-to-the-eilenberg-moore-comparison-functor.md). The [monadic length](../../../../../monadic-length.md) is the least number of successive comparison steps required for the resulting monadic tower to become an equivalence.

For $A\in\mathcal C_n$, let $A_n=\{a:\alpha_n(a)=a\}$. The free $\mathcal C_{n+1}$-object has underlying set

$$
B=A\times\{0\}\;\cup\;A_n\times\mathbb N_{>0}.
$$

Retain all old operations on $A\times\{0\}$. Put

$$
\alpha_{n+1}(a,0)=(a,1)\quad(a\in A_n),
$$

and on every new chain put

$$
\alpha_1(a,k)=(a,k+1).
$$

For $i>1$, $\alpha_i$ is undefined on the new points because none is fixed by $\alpha_1$. These definitions satisfy the domain conditions. If $f:A\to U(B')$ is a $\mathcal C_n$-morphism, its unique extension sends

$$
(a,k)\longmapsto\beta_1^{\,k-1}\bigl(\beta_{n+1}(f(a))\bigr)
\quad(k>0).
$$

This proves the required left adjoint.

After adjoining $\alpha_{m+1}$ freely, the newly added points lie on fixed-point-free $\alpha_1$-chains, while each old point where $\alpha_{m+1}$ was added is no longer fixed by $\alpha_{m+1}$. Consequently there are no points at which a further free operation must be adjoined. Thus for every $n>m$ the endofunctor and unit/multiplication of the monad induced on $\mathcal C_m$ are already those induced by $\mathcal C_m\rightleftarrows\mathcal C_{m+1}$.

By assumption each adjacent adjunction is a [monadic adjunction](../../../../../monadic-adjunction.md). The first comparison for $\mathcal C_m\rightleftarrows\mathcal C_n$ therefore recovers $\mathcal C_{m+1}$, and iteration successively recovers $\mathcal C_{m+2},\ldots,\mathcal C_n$. None of the intervening forgetful functors is an equivalence, since the next partial operation can be chosen differently on a fixed point. Starting at $\mathcal C_0$ takes exactly $n$ steps:

$$
\boxed{\text{the monadic length of }\mathcal C_0\rightleftarrows\mathcal C_n\text{ is }n.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

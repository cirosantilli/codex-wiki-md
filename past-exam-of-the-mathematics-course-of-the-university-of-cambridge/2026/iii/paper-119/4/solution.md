<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For an adjunction $F\dashv U:\mathcal D\to\mathcal C$ with monad $T=UF$, the comparison functor sends $D$ to the $T$-algebra $(UD,U\varepsilon_D)$. The adjunction is [monadic](../../../../../monadic-adjunction.md) when this comparison is an equivalence. The comparison-left-adjoint lemma says that if $\mathcal D$ has coequalizers of the reflexive pairs used to present $T$-algebras and $U$ preserves them, then the comparison has a left adjoint. Applying the unit and counit criteria yields the [Beck monadicity theorem](../../../../../beck-s-monadicity-theorem.md): $U$ is monadic exactly when it reflects isomorphisms and creates coequalizers of all parallel pairs whose images under $U$ admit split coequalizers.

Let $A_n\subseteq A$ be the fixed-point set of $\alpha_n$ and identify $A$ with $A\times\{0\}$. Define $F_nA$ to have underlying set

$$
A\times\{0\}\;\sqcup\;A_n\times\mathbb N_{>0}.
$$

Keep the old operations on the first summand, put $\alpha_{n+1}(a,0)=(a,1)$ for $a\in A_n$, and put $\alpha_1(a,m)=(a,m+1)$ for $m>0$; the remaining higher operations on these new points are undefined. Given $A\to U_nB$, the only possible extension sends $(a,m)$ along the iterates of $\alpha_1$ beginning at $\alpha_{n+1}(a)$. This proves $F_n\dashv U_n$.

The forgetful functor $U_n:\mathcal C_{n+1}\to\mathcal C_n$ reflects isomorphisms. A $U_n$-split coequalizer carries a unique descended partial operation: splitness prevents any new fixed point of $\alpha_n$ from appearing without a representative on which $\alpha_{n+1}$ is already prescribed. Hence $U_n$ creates these coequalizers, and Beck's theorem proves the adjunction monadic.

The composite $U_nU_{n+1}:\mathcal C_{n+2}\to\mathcal C_n$ is not monadic. To see the Beck obstruction explicitly, take $B=\{x,y,z\}$, let all operations through $\alpha_n$ be the identity, let $\alpha_{n+1}$ swap $x,y$ and fix $z$, and define $\alpha_{n+2}(z)=z$. Let $q:B\to Q=\{w,z\}$ identify $x$ and $y$, choose the section $s(w)=x$, $s(z)=z$, and put $h=sq$. Form the kernel pair $A=B\times_QB$ with coordinatewise operations and projections $f,g:A\rightrightarrows B$. The map $t:B\to A$, $t(b)=(b,h(b))$, satisfies

$$
ft=1_B,qquad gt=sq,qquad qs=1_Q,
$$

so $q$ is a split coequalizer of the underlying pair in $\mathcal C_n$.

Any lifted structure on $Q$ must have $\alpha_{n+1}(w)=w$, so $\alpha_{n+2}(w)$ must be defined. If it is $w$, map $x,y$ to a fixed point $d$ and $z$ to a fixed point $e\ne d$ in a target with $\alpha_{n+2}(d)=e$ and $\alpha_{n+2}(e)=e$; this equalizes $f,g$ but its set-theoretic factor through $Q$ does not preserve $\alpha_{n+2}$ at $w$. If instead $\alpha_{n+2}(w)=z$, use a target with $\alpha_{n+2}(d)=d$ and $\alpha_{n+2}(e)=e$ to obtain the same failure. Thus the underlying split coequalizer cannot be created in $\mathcal C_{n+2}$, and Beck's theorem proves that the composite is not monadic.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

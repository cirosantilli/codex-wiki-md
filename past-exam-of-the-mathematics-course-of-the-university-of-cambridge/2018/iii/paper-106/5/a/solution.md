<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the first norm-one assertion, use the usual unital [Banach algebra](../../../../../../banach-algebra-split.md) convention $\|1\|=1$. A [character of an algebra](../../../../../../character-of-an-algebra.md) is a nonzero complex linear multiplicative functional, initially without any continuity assumption. It satisfies $\varphi(1)=1$, since otherwise $\varphi(a)=\varphi(a1)=0$ for every $a$. Moreover, $a-\varphi(a)1$ cannot be invertible: applying $\varphi$ to an inverse identity would give $0=1$. Thus

$$
\varphi(a)\in\sigma_A(a),\qquad |\varphi(a)|\leq r(a)\leq\|a\|.
$$

This proves [automatic continuity of characters](../../../../../../automatic-continuity-of-characters.md) and $\|\varphi\|\leq1$. Evaluation at the normalized identity gives the reverse inequality, so

$$
\boxed{\varphi\text{ is continuous and }\|\varphi\|=1.}
$$

If a convention permits $\|1\|>1$, only $\|\varphi\|\leq1$ follows in general: on $\mathbb C$ with norm $2|z|$, the identity character has norm $1/2$. The later completion argument needs only the upper bound.

If $a$ is invertible, $\varphi(a)\varphi(a^{-1})=1$, so every character is nonzero on $a$. Conversely, if $a$ is not invertible, its principal ideal is proper and lies in a [maximal ideal](../../../../../../maximal-ideal.md) $M$ by [Zorn lemma](../../../../../../zorn-s-lemma.md). The ideal $M$ is closed: if its closure were the whole algebra, it would contain $m$ with $\|1-m\|<1$, making $m$ invertible by the [Neumann series](../../../../../../neumann-series.md), which is impossible for a proper ideal. Maximality therefore gives $\overline M=M$. The quotient $A/M$ is a complex Banach division algebra, hence is $\mathbb C$ by the [Gelfand-Mazur theorem](../../../../../../gelfand-mazur-theorem.md). The quotient map yields a character vanishing at $a$. Consequently

$$
\boxed{a\text{ is invertible}\quad\Longleftrightarrow\quad\varphi(a)\ne0\text{ for every }\varphi\in\Phi_A.}
$$

Now let $A=C(K)$. Its [evaluation characters](../../../../../../evaluation-character.md) give the map $x\mapsto\delta_x\in\Phi_A$. Every character has this form. Indeed, its kernel is a proper ideal. If the functions in that kernel had no common zero, compactness would give finitely many $f_1,\ldots,f_m$ in the kernel with no common zero. Then $h=\sum_j\overline{f_j}f_j$ belongs to the kernel and is everywhere positive, hence is invertible in $C(K)$, a contradiction. At a common zero $x$, the fact that $f-\varphi(f)1$ belongs to the kernel gives $f(x)=\varphi(f)$ for every $f$. Continuous functions distinguish points of the [compact Hausdorff space](../../../../../../compact-hausdorff-space.md) $K$, so the map is bijective. It is continuous for the [Gelfand topology](../../../../../../gelfand-topology.md), and the [compact-to-Hausdorff continuous bijection theorem](../../../../../../compact-to-hausdorff-continuous-bijection-theorem.md) gives

$$
\boxed{\Phi_{C(K)}\cong K.}
$$

For $K=\varnothing$ the norm comparison is trivial; assume henceforth that $K\ne\varnothing$.

Let $B$ be the completion for the other [algebra norm](../../../../../../algebra-norm.md) $\|\cdot\|_1$. It remains commutative and unital, with $A$ embedded densely. The restriction of any $\psi\in\Phi_B$ is a nonzero character of $A$, since it takes $1$ to $1$, and is automatically continuous for the original [supremum norm](../../../../../../supremum-norm.md). Thus $R(\psi)=\psi|_A$ maps into $\Phi_A$. It is injective because two continuous characters agreeing on the dense subalgebra $A$ agree on $B$, and it is continuous because each coordinate $R(\psi)(f)=\psi(f)$ is weak-star continuous.

The [character space](../../../../../../character-space-of-an-algebra.md) $\Phi_B$ is weak-star compact even if its identity was not normalized: the spectral bound puts all its characters in $B_{B^*}$, and the conditions $\psi(1)=1$, $\psi(bc)=\psi(b)\psi(c)$ define a weak-star closed set. Apply [Banach-Alaoglu theorem](../../../../../../banach-alaoglu-theorem.md). Consequently $R$ is a [homeomorphism](../../../../../../homeomorphism.md) onto a closed subset $L\subseteq K$.

Suppose $x\in U=K\setminus L$. The [compact Hausdorff space](../../../../../../compact-hausdorff-space.md) $K$ is normal, so choose an open $V$ with $x\in V\subseteq\overline V\subseteq U$. By the [Urysohn lemma](../../../../../../urysohn-s-lemma.md), choose $g\in C(K)$ with $g(x)=1$ and $g=0$ on $K\setminus V$, and choose $f\in C(K)$ with $f=0$ on $\overline V$ and $f=1$ on $L$. Then $fg=0$. Every character $\psi$ of $B$ restricts to evaluation at a point of $L$, so $\psi(f)=1$. The invertibility criterion proved above makes $f$ invertible in $B$. Multiplying $fg=0$ by $f^{-1}$ in $B$ gives $g=0$, contradicting $g(x)=1$. Therefore $U=\varnothing$ and $R$ is onto $K$.

For each $x\in K$, choose a character $\psi_x\in\Phi_B$ extending $\delta_x$. Its spectral bound gives

$$
|f(x)|=|\psi_x(f)|\leq\|f\|_1.
$$

Taking the supremum over $x$ proves the [minimality of the supremum norm on C(K)](../../../../../../minimality-of-the-supremum-norm-on-c-k.md):

$$
\boxed{\|f\|_\infty\leq\|f\|_1\quad(f\in C(K)).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

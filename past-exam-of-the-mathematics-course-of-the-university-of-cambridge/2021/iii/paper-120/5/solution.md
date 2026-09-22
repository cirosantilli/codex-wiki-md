<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Fix an effective enumeration $(\varphi_e)$ of the unary partial computable functions. Suppose the set

$$
\operatorname{Tot}=\{e:\varphi_e\text{ is total}\}
$$

were computably enumerable, say as $e_0,e_1,\ldots$. Then

$$
g(n)=\varphi_{e_n}(n)+1
$$

would be a [total computable function](../../../../../total-computable-function.md). Hence $g=\varphi_{e_k}$ for some $k$, but

$$
g(k)=\varphi_{e_k}(k)+1=g(k)+1,
$$

a contradiction. Thus the set of Gödel numbers of total computable functions is not recursively axiomatizable; this is the [totality problem is not computably enumerable](../../../../../totality-problem-is-not-computably-enumerable.md) argument.

Let $T$ be a recursively axiomatized theory of arithmetic. For each program index $e$, fix an arithmetical sentence

$$
\operatorname{Tot}(e)\equiv
\forall x\,\exists y\,\operatorname{Comp}(e,x,y)
$$

expressing that the computation with index $e$ halts on every input. Enumerate all formal $T$-proofs and output $e$ whenever a proof ending in $\operatorname{Tot}(e)$ appears. This enumerates exactly the Gödel numbers of the computable functions that $T$ proves total, namely the [provably total computable functions](../../../../../provably-total-computable-function.md), so that set is recursively axiomatizable.

Assume now that $T$ is sound. Repeat every discovered index indefinitely, obtaining an effective infinite list $e_0,e_1,\ldots$ of the functions whose totality $T$ proves. Define

$$
f_T(n)=\varphi_{e_n}(n)+1.
$$

Soundness makes every $\varphi_{e_n}$ genuinely total, so $f_T$ is total and computable. If $T$ proved its totality, an index $e$ for $f_T$ would occur in the list, say $e_k=e$, and then

$$
f_T(k)=\varphi_e(k)+1=f_T(k)+1,
$$

which is impossible. Thus $f_T$ is a total computable function whose totality is not provable in $T$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 120](../../paper-120-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

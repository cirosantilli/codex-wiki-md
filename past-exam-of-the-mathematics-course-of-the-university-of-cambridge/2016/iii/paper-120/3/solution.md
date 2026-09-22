<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**[Rice theorem](../../../../../rice-s-theorem.md): every nontrivial [extensional property of programs](../../../../../extensional-property-of-programs.md) computing [partial computable functions](../../../../../computable-function.md) has an undecidable [index set](../../../../../index-set.md).** More precisely, take an acceptable effective enumeration $(\varphi_e)$ of the unary [partial computable functions](../../../../../computable-function.md). If $\mathcal P$ contains some but not all of these functions, then

$$
\boxed{I_{\mathcal P}=\{e:\varphi_e\in\mathcal P\}\text{ is not computable.}}
$$

“Extensional” means that equality of [partial functions](../../../../../partial-function.md), including their domains, preserves membership; no syntactic restriction on program codes is being considered.

We use two standard facts, stated explicitly. The [diagonal halting set](../../../../../diagonal-halting-set.md) $K=\{e:\varphi_e(e)\downarrow\}$ is undecidable. For the associated acceptable enumerations $\varphi_e^{(r)}$ of $r$-ary [partial computable functions](../../../../../computable-function.md), with $\varphi_e=\varphi_e^{(1)}$, the [S-m-n theorem](../../../../../smn-theorem.md) says that for every $m,n\geq1$ there is a [total computable function](../../../../../total-computable-function.md) $s_n^m$ such that

$$
\varphi_{s_n^m(e,x_1,\ldots,x_m)}^{(n)}(y_1,\ldots,y_n)
\simeq\varphi_e^{(m+n)}(x_1,\ldots,x_m,y_1,\ldots,y_n),
$$

where $\simeq$ means equality of defined values and equality of undefinedness. Thus fixed parameters in a program can be compiled into its index effectively.

Let $\bot$ be the nowhere-defined [partial computable function](../../../../../computable-function.md). Choose a [partial computable function](../../../../../computable-function.md) $h$ whose membership in $\mathcal P$ is opposite to that of $\bot$; this is possible by nontriviality. For each $e$, construct the program

$$
\psi_e(y):\quad\text{first simulate }\varphi_e(e);
\quad\text{if it halts, simulate }h(y)\text{ and return its value}.
$$

This is a uniform partial computation. Take an index $d$ for the binary [partial computable function](../../../../../computable-function.md) $(e,y)\mapsto\psi_e(y)$. The [S-m-n theorem](../../../../../smn-theorem.md) gives the [total computable function](../../../../../total-computable-function.md) $q(e)=s_1^1(d,e)$ with $\varphi_{q(e)}=\psi_e$. Crucially,

$$
\psi_e=\begin{cases}h,&e\in K,\\\bot,&e\notin K.\end{cases}
$$

Even when $h(y)$ itself is undefined, the equality of [partial functions](../../../../../partial-function.md) remains correct. If $\bot\notin\mathcal P$, this gives a [many-one reduction](../../../../../many-one-reduction.md) of $K$ to $I_{\mathcal P}$; if $\bot\in\mathcal P$, it gives a [many-one reduction](../../../../../many-one-reduction.md) of $K$ to the complement of $I_{\mathcal P}$. A decision procedure for $I_{\mathcal P}$ would therefore decide $K$ in either case, a contradiction.

The equivalent language formulation says that every nontrivial property of [computably enumerable languages](../../../../../recursively-enumerable-language.md) depending only on the recognized language has an undecidable [index set](../../../../../index-set.md). Apply the function formulation to the property of a [partial computable function](../../../../../computable-function.md) that its domain has the specified language property: every [computably enumerable language](../../../../../recursively-enumerable-language.md) occurs as such a domain.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 120](../../paper-120-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

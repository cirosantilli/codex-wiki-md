<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Łoś theorem](../../../../../los-theorem.md) states that, for every [first-order formula](../../../../../first-order-formula.md) $\varphi(\mathbf x)$ and product representatives $\mathbf a^1,\ldots,\mathbf a^r$,

$$
\boxed{\prod_i\mathcal A_i/\mathcal U\models\varphi([\mathbf a^1],\ldots,[\mathbf a^r])\iff\{i:\mathcal A_i\models\varphi(a_i^1,\ldots,a_i^r)\}\in\mathcal U.}
$$

It extends the defining relation-symbol rule to arbitrary [first-order formulas](../../../../../first-order-formula.md), including quantified ones.

Identify the countable index set with $\mathbb N$. A [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md) on it contains every cofinite set. Let $p(x)$ be a type over a finite parameter set in the ultraproduct $\mathcal M$, finitely satisfiable in $\mathcal M$. Because the language and parameter set are countable, enumerate it as $\varphi_0(x),\varphi_1(x),\ldots$, with chosen product representatives for the parameters. By finite satisfiability and Łoś,

$$
X_n=\left\{i:\mathcal A_i\models\exists x\bigwedge_{j\leq n}\varphi_j(x)\right\}\in\mathcal U.
$$

Make these large sets decrease while forcing their intersection to be empty:

$$
Y_n=\{i:i\geq n\}\cap\bigcap_{k\leq n}X_k\in\mathcal U.
$$

For each index $i$, let $r(i)$ be the largest $n\leq i$ with $i\in Y_n$, if one exists. Choose $b_i\in A_i$ satisfying the first $r(i)+1$ [first-order formulas](../../../../../first-order-formula.md); this is possible because $i\in X_{r(i)}$. If no such $n$ exists, choose any $b_i$.

For each fixed $n$, every $i\in Y_n$ has $r(i)\geq n$, so $b_i$ satisfies $\varphi_n$. Its coordinate truth set contains $Y_n$ and belongs to $\mathcal U$. Another use of Łoś gives $\mathcal M\models\varphi_n([\mathbf b])$ for every $n$. Thus $[\mathbf b]$ realizes the type. This proves the [countable saturation of an ultraproduct over omega](../../../../../countable-saturation-of-an-ultraproduct-over-omega.md), and in particular **the ultraproduct is omega-saturated**. The construction chooses a finite number of requirements at each coordinate; it does not presume the whole infinite type has a witness in any factor.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the model theory course of the University of Oxford](../../../../split.md)
6. [Model theory course of the University of Oxford](../../../../../model-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

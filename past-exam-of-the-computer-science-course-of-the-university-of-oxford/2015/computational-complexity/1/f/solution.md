<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Let $V$ be the [decidable language](../../../../../recursive-language.md) of syntactically valid descriptions $\operatorname{enc}(M)\#\#w$. Then

$$
\mathcal L_{\mathrm H}\mathbin{\dot\cup}\mathcal L_{\mathrm{NH}}=V,
\qquad
\overline{\mathcal L_{\mathrm H}}
=\mathcal L_{\mathrm{NH}}\mathbin{\dot\cup}(\Sigma^*\setminus V).
$$

Here the [complement of a set](../../../../../complement-of-a-set.md) on the left is taken in all [words over an alphabet](../../../../../string.md), while the non-halting problem only has valid machine-and-input descriptions as instances. **Any malformed description belongs to $\overline{\mathcal L_{\mathrm H}}$ but not to $\mathcal L_{\mathrm{NH}}$.** For example, the [empty word](../../../../../empty-word.md) has no separating `##`, so cannot be a valid instance under the displayed encoding.

Fix valid descriptions $h$ and $\ell$ of, respectively, an immediately halting [Turing machine](../../../../../turing-machine.md) on the [empty word](../../../../../empty-word.md) and a [Turing machine](../../../../../turing-machine.md) looping forever on the [empty word](../../../../../empty-word.md). Then

$$
h\in\mathcal L_{\mathrm H},\qquad
\ell\in\mathcal L_{\mathrm{NH}}.
$$

For the first [many-one reduction](../../../../../many-one-reduction.md), use the total [computable function](../../../../../computable-function.md)

$$
f(x)=
\begin{cases}
x,&x\in V,\\
\ell,&x\notin V.
\end{cases}
$$

For a valid [input](../../../../../input-computer-science.md), nonmembership in $\mathcal L_{\mathrm H}$ is exactly membership in $\mathcal L_{\mathrm{NH}}$, so retaining it is correct. Every invalid [input](../../../../../input-computer-science.md) is a yes-instance of $\overline{\mathcal L_{\mathrm H}}$, and $f$ sends it to the fixed yes-instance $\ell$. Therefore $x\in\overline{\mathcal L_{\mathrm H}}$ if and only if $f(x)\in\mathcal L_{\mathrm{NH}}$.

For the reverse [many-one reduction](../../../../../many-one-reduction.md), use

$$
g(x)=
\begin{cases}
x,&x\in V,\\
h,&x\notin V.
\end{cases}
$$

The equivalence again holds on valid [inputs](../../../../../input-computer-science.md). Invalid [inputs](../../../../../input-computer-science.md) are no-instances of $\mathcal L_{\mathrm{NH}}$, and $h$ is a no-instance of $\overline{\mathcal L_{\mathrm H}}$. Syntax checking terminates, so $g$ is also a total [computable function](../../../../../computable-function.md). We have proved

$$
\boxed{\overline{\mathcal L_{\mathrm H}}\leq_m\mathcal L_{\mathrm{NH}}
\quad\text{and}\quad
\mathcal L_{\mathrm{NH}}\leq_m\overline{\mathcal L_{\mathrm H}}.}
$$

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Computational complexity](../../../computational-complexity-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)

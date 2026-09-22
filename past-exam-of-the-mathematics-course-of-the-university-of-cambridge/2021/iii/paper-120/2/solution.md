<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

We prove the claim by [structural induction for primitive recursive functions](../../../../../structural-induction-for-primitive-recursive-functions.md). A formula is bounded when every quantifier is a [bounded quantifier](../../../../../bounded-quantifier.md); this is a [Delta-0 formula](../../../../../delta-0-formula.md). The graphs of the initial functions have quantifier-free definitions:

$$
Z(\mathbf x)=y\Longleftrightarrow y=0,
\qquad
S(x)=y\Longleftrightarrow y=x+1,
\qquad
\pi_i^k(\mathbf x)=y\Longleftrightarrow y=x_i.
$$

Suppose $f(\mathbf x)=g(h_1(\mathbf x),\ldots,h_m(\mathbf x))$ and the graphs of $g,h_1,\ldots,h_m$ have existential bounded definitions. Introduce variables $u_1,\ldots,u_m$ for the intermediate values and conjoin the graph formulas

$$
u_j=h_j(\mathbf x),
\qquad
y=g(u_1,\ldots,u_m).
$$

Pulling all unrestricted existential witnesses to the front leaves a bounded matrix, so the required form is preserved by composition.

For primitive recursion, use [Gödel beta-function sequence coding](../../../../../godel-beta-function-sequence-coding.md). The relation

$$
\beta(b,c,i)=r
\quad\Longleftrightarrow\quad
r<1+(i+1)c\ \land\
\exists q\leq b\,[b=q(1+(i+1)c)+r]
$$

is bounded in the language of ordered rings. Given any finite sequence $a_0,\ldots,a_n$, choose $c$ larger than all its entries and divisible by $1,\ldots,n+1$. The moduli $1+(i+1)c$ are pairwise coprime, so the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) supplies $b$ with $\beta(b,c,i)=a_i$ for every $i\leq n$.

Suppose

$$
f(\mathbf x,0)=g(\mathbf x),
\qquad
f(\mathbf x,n+1)=h(\mathbf x,n,f(\mathbf x,n)),
$$

and the induction hypothesis gives existential bounded graph formulas for $g$ and $h$. Then $y=f(\mathbf x,n)$ exactly when there are $b,c$ coding values $a_0,\ldots,a_n$, together with a common witness bound $W$, such that:

$$
\begin{aligned}
&a_0=g(\mathbf x),\\
&\forall i<n\quad a_{i+1}=h(\mathbf x,i,a_i),\\
&a_n=y.
\end{aligned}
$$

Write each $a_i$ using $\beta(b,c,i)$, bound the variables representing $a_i$ by $1+(n+1)c$, and bound every witness used by the graph formulas for $g$ and $h$ by $W$. All quantifiers checking the displayed finite recursion are then bounded; only $b,c,W$ and the finitely many outer coding witnesses are unrestricted existential variables. Conversely, any code passing these bounded checks satisfies the recursion equations, and induction on $i\leq n$ forces its $i$th entry to be $f(\mathbf x,i)$. This proves the [existential bounded representation of a primitive recursive function](../../../../../existential-bounded-representation-of-a-primitive-recursive-function.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 120](../../paper-120-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

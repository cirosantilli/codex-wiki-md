<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We prove closure under the defining schemes for [primitive recursive functions](../../../../../primitive-recursive-function.md), keeping all unbounded existential variables outside a [bounded arithmetic formula](../../../../../arithmetic-bounded-formula.md). A [bounded quantifier](../../../../../bounded-quantifier.md) means $\exists v<t$ or $\forall v<t$, where $t$ does not contain $v$. All formulas are interpreted in the standard [natural numbers](../../../../../natural-number.md).

First we need a finite [sequence](../../../../../sequence.md) code using only the permitted [language of ordered rings](../../../../../language-of-ordered-rings.md). Define the [bounded arithmetic formula](../../../../../arithmetic-bounded-formula.md)

$$
B(b,c,i,a)\;:\Longleftrightarrow\;a<1+(i+1)c\ \wedge\ (\exists q<b+1)\,[b=q(1+(i+1)c)+a].
$$

For given $b,c,i$, it specifies the unique remainder of $b$ modulo $1+(i+1)c$. In particular the quotient and remainder variables are bounded by [arithmetic](../../../../../arithmetic-split.md) terms; division is not a new language symbol.

Every finite list $a_0,\ldots,a_n$ can be coded by some pair $b,c$. Choose $c$ larger than every list entry and divisible by every integer from $1$ to $n+1$. The moduli $m_i=1+(i+1)c$ are pairwise coprime. Indeed a prime dividing both $m_i,m_j$ cannot divide $c$, but then divides $j-i$; since $0<j-i\leq n$ and $c$ is divisible by that integer, this is impossible. The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) gives $b$ with $b\equiv a_i\pmod{m_i}$ for every $i$. Since $a_i<c<m_i$, each $B(b,c,i,a_i)$ holds. This is [Gödel beta-function sequence coding](../../../../../godel-beta-function-sequence-coding.md). The external choice of a divisible $c$ proves that codes exist; factorial and exponentiation do not occur in the [existential bounded representation of a primitive recursive function](../../../../../existential-bounded-representation-of-a-primitive-recursive-function.md).

For the zero [function](../../../../../function-split.md), [successor function](../../../../../successor-function.md) and projections use $y=0$, $y=x+1$ and $y=x_j$. These formulas need no auxiliary variables. For [function composition in recursion theory](../../../../../function-composition-in-recursion-theory.md), suppose $g_1,\ldots,g_m,h$ have representations with [bounded arithmetic formulas](../../../../../arithmetic-bounded-formula.md) $\theta_1,\ldots,\theta_m,\theta_h$. A [bounded arithmetic formula](../../../../../arithmetic-bounded-formula.md) for $h(g_1(\vec x),\ldots,g_m(\vec x))$ is

$$
\bigwedge_{j=1}^m\theta_j(u_j,\vec x,\vec v_j)\ \wedge\ \theta_h(y,u_1,\ldots,u_m,\vec w).
$$

Treat every $u_j,\vec v_j,\vec w$ as an auxiliary variable in the outer existential block. The [logical conjunction](../../../../../logical-conjunction.md) is true for some such variables exactly when $y$ is the desired output.

Now suppose

$$
f(0,\vec x)=g(\vec x),\qquad f(i+1,\vec x)=h(i,f(i,\vec x),\vec x).
$$

By [structural induction for primitive recursive functions](../../../../../structural-induction-for-primitive-recursive-functions.md), assume $\theta_g(a,\vec x,\vec v)$ and $\theta_h(a',i,a,\vec x,w_1,\ldots,w_m)$ are [bounded arithmetic formulas](../../../../../arithmetic-bounded-formula.md) representing $g,h$. We code the values $f(0,\vec x),\ldots,f(n,\vec x)$ with $b,c$. For [finite witness array coding](../../../../../finite-witness-array-coding.md), give each component of the step witness another code pair $d_j,e_j$, so that the witness at step $i$ is the remainder specified by $B(d_j,e_j,i,w_j)$.

With these code pairs and $\vec v$ as free auxiliary variables, take the following [bounded arithmetic formula](../../../../../arithmetic-bounded-formula.md):

$$
\begin{aligned}
\phi(y,n,\vec x,b,c,\vec d,\vec e,\vec v)\;:\Longleftrightarrow{}&B(b,c,n,y)\\
&\wedge(\exists a<1+c)\,[B(b,c,0,a)\wedge\theta_g(a,\vec x,\vec v)]\\
&\wedge(\forall i<n)(\exists a<1+(i+1)c)(\exists a'<1+(i+2)c)\\
&\quad(\exists w_1<1+(i+1)e_1)\cdots(\exists w_m<1+(i+1)e_m)\\
&\quad\left[B(b,c,i,a)\wedge B(b,c,i+1,a')\wedge\bigwedge_{j=1}^mB(d_j,e_j,i,w_j)\wedge\theta_h(a',i,a,\vec x,\vec w)\right].
\end{aligned}
$$

The displayed line breaks are only for readability: the [bounded quantifiers](../../../../../bounded-quantifier.md) on the last three lines bind the entire bracket. If $m=0$, their empty block and [logical conjunction](../../../../../logical-conjunction.md) are omitted. Expanding every occurrence of $B$ leaves only [bounded quantifiers](../../../../../bounded-quantifier.md), [logical conjunctions](../../../../../logical-conjunction.md), the bounded [arithmetic](../../../../../arithmetic-split.md) formulas already obtained, and the symbols $0,1,+,\times,<,=$.

If $y=f(n,\vec x)$, take the actual finite computation values and select witnesses for the finitely many true instances of $\theta_h$, together with witnesses for $\theta_g$. The [Gödel beta-function sequence coding](../../../../../godel-beta-function-sequence-coding.md) provides $b,c$ and the finitely many $d_j,e_j$. These make $\phi$ true. Conversely, suppose some code pairs and initial witnesses make $\phi$ true. The unique remainders of $b$ give values $a_0,\ldots,a_n$. The initial clause makes $a_0=g(\vec x)$. Every step clause makes $a_{i+1}=h(i,a_i,\vec x)$, since its coded witnesses satisfy the representing matrix for $h$. Induction on $i$ gives $a_i=f(i,\vec x)$, and the final remainder clause gives $y=a_n$. This argument includes $n=0$, when the step condition is empty.

Closure under the [initial functions of recursion theory](../../../../../initial-function-of-recursion-theory.md), composition and [primitive recursion](../../../../../primitive-recursion.md) proves

$$
\boxed{y=f(\vec x)\quad\Longleftrightarrow\quad(\exists\vec z)\,\phi(y,\vec x,\vec z),\qquad\phi\text{ has only bounded quantifiers}.}
$$

Coding the step witnesses is essential: leaving an unrestricted existential witness block inside $\forall i<n$ would not give the required syntactic form.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

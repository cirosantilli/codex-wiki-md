<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work over the [finite field](../../../../../finite-field.md) $\mathbb F_2$, and write $A_i$ for row $i$ of the PDF's $12\times12$ matrix. The first row has [Hamming weight](../../../../../hamming-weight.md) eleven; all other rows have [Hamming weight](../../../../../hamming-weight.md) seven. To check their intersections economically, index the last eleven columns modulo eleven. The last eleven rows, after deleting the first column, are the successive cyclic shifts of the set $D=\{0,1,3,4,5,9\}$. Direct calculation gives

$$
\begin{array}{c|ccccc}t&1&2&3&4&5\\\hline D\cap(D+t)&\{1,4,5\}&\{0,3,5\}&\{1,3,4\}&\{4,5,9\}&\{3,5,9\}\end{array}.
$$

The intersection sizes for $-t$ equal those for $t$. Thus two different rows among $A_2,\ldots,A_{12}$ meet in four positions, including their shared first coordinate, whereas $A_1$ meets each of these rows in six positions. All these intersection sizes are [even numbers](../../../../../even-number.md), while each row weight is an [odd number](../../../../../odd-number.md). Consequently $AA^T=I$. The first row and column agree, and the entry of the last eleven-by-eleven block depends only on the sum of its row and column indices modulo eleven, because successive rows are left shifts. Thus $A$ is a [symmetric matrix](../../../../../symmetric-matrix.md), so $A^2=I$.

The [generator matrix](../../../../../generator-matrix.md) $G=(I\mid A)$ has [rank](../../../../../rank-one-quadratic-form.md) twelve, and

$$
GG^T=I+AA^T=0.
$$

Hence its [linear code](../../../../../linear-code.md) $C$ lies in its [dual code](../../../../../dual-code.md) $C^\perp$. Both have [dimension](../../../../../dimension-vector-space.md) twelve, so $C=C^\perp$: it is a [self-dual code](../../../../../self-dual-code.md). Moreover $AG=(A\mid A^2)=(A\mid I)$, and $A$ is an [invertible matrix](../../../../../invertible-matrix.md), so this is another [generator matrix](../../../../../generator-matrix.md) for the same code. In the column [parity-check matrix](../../../../../parity-check-matrix.md) convention of the question,

$$
\boxed{C=C^\perp,\qquad G'=(A\mid I),\qquad H=\begin{pmatrix}I\\A\end{pmatrix},\qquad GH=0.}
$$

The matrix $H$ has [rank](../../../../../rank-one-quadratic-form.md) twelve, so its nullspace condition $cH=0$ characterizes $C$ exactly.

To prove the [minimum Hamming distance](../../../../../minimum-distance-of-a-code.md), first observe that the rows of $G$ have [Hamming weights](../../../../../hamming-weight.md) twelve and eight. For binary vectors,

$$
\operatorname{wt}(v+w)=\operatorname{wt}(v)+\operatorname{wt}(w)-2|\operatorname{supp}(v)\cap\operatorname{supp}(w)|.
$$

Every partial sum of generator rows is orthogonal to every further generator row, by $GG^T=0$. Its intersection with that row therefore contains an [even number](../../../../../even-number.md) of positions. Induction using this identity proves that every [codeword](../../../../../codeword.md) has weight divisible by four: $C$ is a [doubly even code](../../../../../doubly-even-code.md).

The [systematic-matrix proof of extended Golay distance](../../../../../systematic-matrix-proof-of-extended-golay-distance.md) now excludes weight four. Write a [codeword](../../../../../codeword.md) as $(u,uA)$ and put $k=\operatorname{wt}(u)$. If its total weight were four, $1\leq k\leq4$. For $k=1$, the right half is a row of $A$ and has weight seven or eleven. For $k=2$, the right half is the sum of two distinct rows; the intersection counts above give weight $11+7-2\cdot6=6$ or $7+7-2\cdot4=6$. For $k=3$, the right half would be a unit vector, but then $u=(uA)A$ would be a row of $A$, of weight seven or eleven. For $k=4$, the right half would vanish, contradicting invertibility of $A$. Thus no nonzero word has weight four. Every nonzero weight is consequently at least eight, and any generator row other than the first attains eight. Since the [minimum Hamming distance of a linear code](../../../../../minimum-hamming-distance-of-a-linear-code.md) is its least nonzero weight,

$$
\boxed{d(C)=8,\qquad C\text{ has parameters }[24,12,8].}
$$

Define the length-$23$ [binary Golay code](../../../../../binary-golay-code.md) $C_{23}$ as the [punctured code](../../../../../punctured-code.md) obtained by deleting the first coordinate of this [extended binary Golay code](../../../../../extended-binary-golay-code.md). This [puncturing](../../../../../puncturing-coding-theory.md) is injective on $C$, because a nonzero word in its kernel would have weight one. Thus $\dim C_{23}=12$, and deleting one coordinate gives $d(C_{23})\geq7$. The sum of the first two generator rows has weight eight and first coordinate one, so its puncture has weight seven. Therefore $d(C_{23})=7$. In fact any coordinate can be punctured: every left coordinate except the first occurs in a weight-eight generator row, the first occurs in the sum just used, and every right coordinate occurs in at least one of the weight-eight generator rows.

The radius-three [Hamming balls](../../../../../hamming-ball.md) around the $2^{12}$ words of $C_{23}$ are disjoint, since two centers in intersecting balls would have [Hamming distance](../../../../../hamming-distance.md) at most six. Each ball contains

$$
\sum_{j=0}^3\binom{23}{j}=1+23+253+1771=2048=2^{11}
$$

words. Their combined size is $2^{12}2^{11}=2^{23}$, the size of the entire binary [Hamming space](../../../../../hamming-space.md). Hence

$$
\boxed{C_{23}\text{ is a perfect }[23,12,7]\text{ code, correcting three errors}.}
$$

For decoding in $C$, write the received word as $y=c+(p,q)$, where $(p,q)$ is the unknown error in its two halves. Its [syndrome](../../../../../syndrome.md) is

$$
s=yH=p+qA,\qquad t=sA=pA+q.
$$

Let $e_i$ denote the length-twelve unit vector. For [bounded-distance decoding](../../../../../bounded-distance-decoding.md), the [three-error syndrome decoding of extended Golay code](../../../../../three-error-syndrome-decoding-of-extended-golay-code.md) is the following finite search, returning the first successful candidate error:

- If $\operatorname{wt}(s)\leq3$, return $(s,0)$.
- Otherwise, if some $i$ satisfies $\operatorname{wt}(s+A_i)\leq2$, return $(s+A_i,e_i)$.
- Otherwise, compute $t=sA$; if $\operatorname{wt}(t)\leq3$, return $(0,t)$.
- Otherwise, if some $i$ satisfies $\operatorname{wt}(t+A_i)\leq2$, return $(e_i,t+A_i)$.
- If no test succeeds, declare that no error of weight at most three has this [syndrome](../../../../../syndrome.md).

Every returned candidate has total [Hamming weight](../../../../../hamming-weight.md) at most three and the required [syndrome](../../../../../syndrome.md). Conversely, an error of total weight at most three has a half of weight zero or one. The tests exhaust respectively $q=0$, $q=e_i$, $p=0$, and $p=e_i$, so they find every such error. Two distinct successful candidates would differ by a nonzero [codeword](../../../../../codeword.md) of weight at most six, contradicting $d(C)=8$. Thus the result is unique, and the decoded word is $y+(p,q)$. The condition $\operatorname{wt}(s)\geq3$ still allows the first test when the weight is exactly three; for larger syndrome weight begin with the second test. A large syndrome weight alone does not imply more than three errors.

**The decoder corrects every error of weight at most three; failure means that the received word is outside all radius-three decoding balls.** Unlike its puncture, $C$ is not a [perfect code](../../../../../perfect-code.md): its radius-three balls cover only $2^{12}(1+24+276+2024)=2^{12}\cdot2325<2^{24}$ words. Without the three-error assumption, a successful test identifies a nearby codeword but need not identify the transmitted word.

For an arbitrary received word, a complete [minimum-distance decoding](../../../../../minimum-distance-decoding.md) fallback is to enumerate $q\in\mathbb F_2^{12}$ and minimize $\operatorname{wt}(s+qA)+\operatorname{wt}(q)$. Every error with the observed [syndrome](../../../../../syndrome.md) has exactly the form $(s+qA,q)$, so a minimizer gives a nearest [codeword](../../../../../codeword.md) $y+(s+qA,q)$. Report all minimizers if there is a tie. This also decodes outside the guaranteed radius in the nearest-word sense, while making no unsupported claim that the transmitted word is determined. Thus a syndrome of weight at least three alone is insufficient for guaranteed recovery; either the three-error hypothesis or a choice among nearest words is needed.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 87](../../paper-87-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

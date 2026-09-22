<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $\mathcal E$ be an [elementary topos](../../../../../elementary-topos.md) with [subobject classifier](../../../../../subobject-classifier.md) $\top:1\to\Omega$. A [local operator](../../../../../lawvere-tierney-topology.md) is a map $j:\Omega\to\Omega$ which is inflationary, idempotent, preserves truth, and preserves binary meets:

$$
p\leq j(p),
\qquad j(jp)=j(p),
\qquad j(\top)=\top,
\qquad j(p\wedge q)=j(p)\wedge j(q).
$$

If $m:A'\hookrightarrow A$ is classified by $\chi_m:A\to\Omega$, its [closure operation of a local operator](../../../../../closure-operation-of-a-local-operator.md) is classified by $j\chi_m$. The mono is [j-dense monomorphism](../../../../../j-dense-monomorphism.md) when this closure is all of $A$, and $j$-closed when it equals its closure. An object $X$ is a [j-sheaf](../../../../../j-sheaf.md) when every map $A'\to X$ along a $j$-dense mono $A'\hookrightarrow A$ extends uniquely to $A\to X$.

The [closed-subobject classifier](../../../../../closed-subobject-classifier.md) is the equalizer

$$
i:\Omega_j\hookrightarrow\Omega
\mathrel{\substack{\xrightarrow{\mathrm{id}}\\[-2pt]\xrightarrow[j]{} }}\Omega.
$$

Thus maps to $\Omega_j$ classify precisely the $j$-closed subobjects. Idempotence factors $j$ as

$$
\Omega\xrightarrow{q}\Omega_j\xrightarrow{i}\Omega,
\qquad qi=1_{\Omega_j},
\qquad iq=j.
$$

To prove that $\Omega_j$ is a $j$-sheaf, let $m:B\hookrightarrow A$ be dense and let $f:B\to\Omega_j$ classify a closed subobject $C\hookrightarrow B$. Take the closure in $A$ of the composite $C\hookrightarrow A$. Pullback stability of closure gives

$$
\overline C^{,A}\cap B=\overline C^{,B}=C,
$$

so the classifier $A\to\Omega_j$ of $\overline C^{,A}$ extends $f$. If two closed subobjects of $A$ restrict to the same subobject of dense $B$, the equalizer of their classifiers is a closed subobject containing $B$; it is both closed and dense and hence equals $A$. The extension is therefore unique.

Let

$$
L:\mathcal E\longrightarrow\mathbf{sh}_j(\mathcal E)
$$

be the [sheaf reflector for a local operator](../../../../../sheaf-reflector-for-a-local-operator.md). The subobject classifier in the sheaf topos is $\Omega_j$. We prove the four assertions through the cycle

$$
(i)\Longleftrightarrow(ii)\Longleftrightarrow(iii)\Longleftrightarrow(iv).
$$

The canonical map comparing the reflected ambient classifier with the sheaf classifier is

$$
L(q):L(\Omega)\longrightarrow L(\Omega_j)\cong\Omega_j.
$$

Consequently $L$ preserves the subobject classifier exactly when $L(q)$ is an isomorphism. This proves $(i)\Longleftrightarrow(ii)$.

Since $qi=1_{\Omega_j}$, one has

$$
L(q)L(i)=1_{\Omega_j}.
$$

If $L(q)$ is an isomorphism then $L(i)$ is its inverse. Conversely, if $L(i)$ is an isomorphism, the same equation makes $L(q)$ its inverse. A monomorphism is sent to an isomorphism by sheafification exactly when it is $j$-dense, so $(ii)\Longleftrightarrow(iii)$.

Assume $(iii)$ and let $m:A'\hookrightarrow A$ have characteristic map $\chi:A\to\Omega$. Form the [pullback](../../../../../pullback-category-theory.md)

$$
\begin{array}{ccc}
A''&\longrightarrow&\Omega_j\\
\downarrow d&&\downarrow i\\
A&\xrightarrow{\chi}&\Omega.
\end{array}
$$

Because dense monos are pullback-stable, $d:A''\hookrightarrow A$ is $j$-dense. The original $A'$ factors through $A''$, and its characteristic map inside $A''$ is the top horizontal map followed by $i$, which is fixed by $j$. Hence $A'\hookrightarrow A''$ is $j$-closed. This proves $(iv)$.

Finally assume $(iv)$ and apply it to $i:\Omega_j\hookrightarrow\Omega$:

$$
\Omega_j\xrightarrow{c}A''\xrightarrow{d}\Omega,
$$

where $c$ is closed and $d$ is dense. Since $d$ is monic and $i=dc$, the map $c$ is the pullback of $d$ along $i$. It is therefore dense as well as closed, and hence is an isomorphism. Thus $i$ is, up to an isomorphism, the dense mono $d$, proving $(iii)$. All four conditions are equivalent, as summarized by the [subobject-classifier preservation criterion for a sheaf reflector](../../../../../subobject-classifier-preservation-criterion-for-a-sheaf-reflector.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

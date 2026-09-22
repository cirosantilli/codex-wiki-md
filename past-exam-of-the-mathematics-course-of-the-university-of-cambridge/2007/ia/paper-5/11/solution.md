<h1 id="11/solution">Solution</h1>

↑ **Parent:** [11](../11.md)

For finite sets $A_1,\ldots,A_m$, the [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) states

$$
\boxed{\left|\bigcup_{i=1}^mA_i\right|=\sum_{\varnothing\ne I\subseteq\{1,\ldots,m\}}(-1)^{|I|+1}\left|\bigcap_{i\in I}A_i\right|.}
$$

To prove it, count one element at a time. An element belonging to exactly $r\ge1$ of the sets occurs in $\binom rj$ of their $j$-fold intersections, so its total coefficient on the right is $\sum_{j=1}^r(-1)^{j+1}\binom rj=1$, using $(1-1)^r=0$. An element in no set has coefficient zero. Every element of the union is therefore counted once, proving the identity.

For the keypad, an initial zero can never be entered: it has no preceding pair of ones and the first key is not two. Define four classes of valid four-digit sequences. Let $A$ contain sequences starting with two, with the last three digits arbitrary; let $B$ contain sequences with no zeros; let $C$ contain sequences of the form $110d$ with $d\in\{1,\ldots,9\}$; and let $D$ contain sequences $d110$ with $d\in\{1,\ldots,9\}$.

These classes exhaust the valid codes. A sequence starting with two is unrestricted thereafter. Otherwise a zero cannot occur in position two, a zero in position three requires the first two digits to be ones, and a zero in position four requires digits two and three to be ones. Positions three and four cannot both be zero, since the last zero would then lack the required preceding pair. Thus a code outside $A$ either belongs to $B$ or has precisely one of the zero patterns covered by $C,D$.

Their sizes are

$$
|A|=10^3=1000,\quad |B|=9^4=6561,\quad |C|=9,\quad |D|=9.
$$

The only nonempty pairwise intersections are $A\cap B$, consisting of first digit two and three nonzero remaining digits, and $A\cap D$, containing the single code $2110$. Hence $|A\cap B|=9^3=729$ and $|A\cap D|=1$. All other pairwise intersections vanish, and therefore so do all intersections of three or four classes. Applying [inclusion-exclusion](../../../../../inclusion-exclusion-principle.md) gives

$$
\boxed{|A\cup B\cup C\cup D|=1000+6561+9+9-729-1=6849.}
$$

This counts sequences actually enterable under the history-dependent zero-key rule, rather than simply counting sequences which contain the substring $110$.

## ↑ Ancestors (10)

1. [11](../11.md)
2. [Paper 5](../../paper-5-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

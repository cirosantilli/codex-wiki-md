<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Abbreviate the [database attributes](../../../../../database-attribute.md) by $E,C,B,S,T,O$ for `EventId`, `ConfId`, `BuildingId`, `StartTime`, `EndTime` and `ConfOrganizer`. Write $\mathcal A=\{E,C,B,S,T,O\}$ for the full [relational schema](../../../../../relational-schema.md).

The explicit event assumptions give the [functional dependency](../../../../../functional-dependency.md)

$$
EC\to BSTO.
$$

I additionally interpret the conference's organizer as a single organizer for the whole conference, giving $C\to O$. This is the natural reading of `ConfOrganizer`, but it is stronger than saying only that each event has one organizer. Under this interpretation a compact generating basis of [functional dependencies](../../../../../functional-dependency.md) is

$$
\boxed{F=\{EC\to BST,\ C\to O\}.}
$$

There is no premise that an `EventId` is globally unique, that a conference has one building, or that a start time determines an end time. In particular, the single-room requirement for one subtype in part (a) must not be imposed on this entire [database relation](../../../../../database-relation.md).

To specify **all** non-trivial [functional dependencies](../../../../../functional-dependency.md) without listing every augmented version, the [attribute closure](../../../../../attribute-closure.md) is

$$
X^+=\begin{cases}
\mathcal A,&\{E,C\}\subseteq X,\\
X\cup\{O\},&C\in X,\ E\notin X,\\
X,&C\notin X.
\end{cases}
$$

Exactly the [functional dependencies](../../../../../functional-dependency.md) $X\to Y$ with $Y\subseteq X^+$ and $Y\not\subseteq X$ are non-trivial consequences of the assumptions. In particular, $EC$ is the only [candidate key](../../../../../candidate-key.md): both $E$ and $C$ must be present because neither is generated from other [database attributes](../../../../../database-attribute.md).

Every [functional dependency](../../../../../functional-dependency.md) implies the corresponding [multivalued dependency](../../../../../multivalued-dependency.md). Thus $C\twoheadrightarrow O$ and, by complementation, $C\twoheadrightarrow EBST$ hold. Also $EC\twoheadrightarrow Y$ holds for every $Y\subseteq\mathcal A$, with the usual trivial cases omitted. A complete compact description, including all augmented and complemented cases, is

$$
\boxed{F\models X\twoheadrightarrow Y\quad\Longleftrightarrow\quad
Y\subseteq X^+\ \text{or}\ \mathcal A\setminus(X\cup Y)\subseteq X^+.}
$$

For a non-trivial [multivalued dependency](../../../../../multivalued-dependency.md), additionally require $Y\not\subseteq X$ and $X\cup Y\ne\mathcal A$. To see the criterion, if either side of the split is determined by $X$, swapping that side requires no new [database tuple](../../../../../database-tuple.md). Conversely, if both sides contain a [database attribute](../../../../../database-attribute.md) outside $X^+$, choose two [database tuples](../../../../../database-tuple.md) agreeing exactly on $X^+$. They satisfy every [functional dependency](../../../../../functional-dependency.md) in $F$, but a mixed [database tuple](../../../../../database-tuple.md) required by the proposed [multivalued dependency](../../../../../multivalued-dependency.md) is neither of them. The two-row [database relation](../../../../../database-relation.md) is therefore a counterexample.

There is no independent many-valued fact such as buildings freely combining with event times. For example, two events of one conference might have $(E,B,S,T)=(e_1,b_1,s_1,t_1)$ and $(e_2,b_2,s_2,t_2)$. A [multivalued dependency](../../../../../multivalued-dependency.md) $C\twoheadrightarrow B$ would require the building to be swappable independently of the event and its times, which these assumptions do not require and the event [functional dependency](../../../../../functional-dependency.md) may forbid.

Since $C$ is not a [superkey](../../../../../superkey.md), $C\to O$ violates [Boyce-Codd normal form](../../../../../boyce-codd-normal-form.md). The corresponding non-trivial [multivalued dependency](../../../../../multivalued-dependency.md) $C\twoheadrightarrow O$ violates [fourth normal form](../../../../../fourth-normal-form.md). Use the decomposition

$$
\boxed{\begin{aligned}
\mathsf{ConferenceOrganizer}&(C,O),\\
\mathsf{EventSchedule}&(E,C,B,S,T).
\end{aligned}}
$$

Their common [database attribute](../../../../../database-attribute.md) is $C$, which determines the whole first component. Consequently the decomposition is a [lossless-join decomposition](../../../../../lossless-join-decomposition.md): each event joins to exactly its own conference's organizer, producing no spurious [database tuples](../../../../../database-tuple.md).

In the first component, the only basic non-trivial [functional dependency](../../../../../functional-dependency.md) is $C\to O$, whose determinant is a [candidate key](../../../../../candidate-key.md). In the second it is $EC\to BST$, again with a [candidate key](../../../../../candidate-key.md) determinant. No independent non-trivial [multivalued dependencies](../../../../../multivalued-dependency.md) with determinants that are not [superkeys](../../../../../superkey.md) are implied in either component, so both are in [fourth normal form](../../../../../fourth-normal-form.md), and therefore in [Boyce-Codd normal form](../../../../../boyce-codd-normal-form.md). This reaches the strongest normal form tested here. The decomposition is a [dependency-preserving decomposition](../../../../../dependency-preserving-decomposition.md): $C\to O$ is enforced in the first component, $EC\to BST$ in the second, and together they imply $EC\to O$.

If only the explicitly stated event-level organizer uniqueness is assumed, omit $C\to O$. The basis is then just $EC\to BSTO$; $X^+=\mathcal A$ when $EC\subseteq X$ and $X^+=X$ otherwise. Under those weaker assumptions the original [database relation](../../../../../database-relation.md) is already in [fourth normal form](../../../../../fourth-normal-form.md) and [Boyce-Codd normal form](../../../../../boyce-codd-normal-form.md), so no decomposition is necessary. In particular, separating $(C,O)$ under that reading could create extra [database tuples](../../../../../database-tuple.md) when different events of one conference have different organizers.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Databases](../../../databases-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)

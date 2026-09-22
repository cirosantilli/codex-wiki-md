<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Keep the corrected one-place [STRIPS](../../../../../strips.md) model, replace the item constants and their initial typing facts by $\mathrm{FOX},\mathrm{RABBIT},\mathrm{CARROT}$, and require all three west in the goal. The farmer travels with the boat, so the boat's bank also records where supervision is available. The new requirement concerns the bank being left: incompatible items may coexist at the farmer's current bank, but must not be left there together.

Here is a compilation using only ordinary positive [STRIPS](../../../../../strips.md) [preconditions](../../../../../precondition.md). Replace $\mathrm{onBoat}(x)$ everywhere by $\mathrm{at}(x,\mathrm{BOAT})$, extending the item's possible locations to

$$
\mathcal L=\{\mathrm{EAST},\mathrm{WEST},\mathrm{BOAT}\}.
$$

The boat itself still has only bank locations, enforced by $\mathrm{isBank}$. Initialize a static relation $\mathrm{SafePair}(p,q,s)$ for every $p,q\in\mathcal L$ and bank $s$ except $p=q=s$. It states that two incompatible items at locations $p,q$ are not both on the bank about to be left.

Introduce [planning safety certificates](../../../../../planning-safety-certificate.md) $\mathrm{SafeToSail}(\mathrm{EAST})$ and $\mathrm{SafeToSail}(\mathrm{WEST})$, neither initially true. The following checking action grants a certificate:

$$
\begin{aligned}
\mathrm{Check}(s,p_F,p_R,p_C):\quad
P=\{&
\mathrm{isBank}(s),\mathrm{at}(\mathrm{BOAT},s),\\
&\mathrm{at}(\mathrm{FOX},p_F),\mathrm{at}(\mathrm{RABBIT},p_R),
\mathrm{at}(\mathrm{CARROT},p_C),\\
&\mathrm{SafePair}(p_F,p_R,s),\mathrm{SafePair}(p_R,p_C,s)\},\\
A&=\{\mathrm{SafeToSail}(s)\},\qquad D=\varnothing.
\end{aligned}
$$

Add $\mathrm{SafeToSail}(s)$ to the [preconditions](../../../../../precondition.md) of $\mathrm{Move}(s,t)$. Every load, unload and move deletes **both** certificate facts. The other movement and capacity effects remain unchanged.

Deleting certificates on every location change prevents a stale safety check from authorizing a later unsafe departure. A certificate is granted only for the actual current locations and only when both incompatible pairs are separated on the departure bank. During a crossing the remaining bank is therefore safe; on arrival the farmer supervises the destination bank. This proves the required safety property by [mathematical induction](../../../../../mathematical-induction.md) over crossings. The static $\mathrm{SafePair}$ facts are never changed.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)

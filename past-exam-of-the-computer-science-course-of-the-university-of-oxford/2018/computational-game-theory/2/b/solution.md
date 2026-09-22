<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply [backward induction in games](../../../../../backward-induction-in-games.md), or [Zermelo's algorithm](../../../../../backward-induction-in-games.md), from the terminal decision points. At node 4, player 1 chooses $R_4$ because $6>3$, giving continuation payoffs $(6,9)$. At node 5, player 1 chooses $L_5$ because $4>2$, giving $(4,6)$. At node 3, player 2 compares its continuation payoffs nine and six, so chooses $L_3$. At node 2, player 2 chooses $R_2$, receiving four rather than two.

At the root, player 1 consequently receives six from either action: $L_1$ leads to $(6,4)$ and $R_1$ to $(6,9)$. Thus **there are two pure [subgame perfect equilibria](../../../../../subgame-perfect-equilibrium.md)**, with strategies

$$
\boxed{(L_1,R_4,L_5;\ R_2,L_3),\qquad(R_1,R_4,L_5;\ R_2,L_3).}
$$

The semicolon separates the players, and each list specifies the player's action at every one of its decision points. All four non-root choices are strict. If mixed strategies are included, **every mixture between $L_1$ and $R_1$ at the root is also an equilibrium**, with those other actions fixed. There are no further mixtures at the strict decision points.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)

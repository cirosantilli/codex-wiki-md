# Cached cell value

↑ **Parent:** [Spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md)

A numerical value retained for reuse by [memoization](memoization.md). It is usable only while the [spreadsheet formula](spreadsheet-formula.md) and all its relevant [inputs](input-computer-science.md) remain valid. After changing `A1` from 3 to 5, following outgoing [directed edges](directed-edge.md) finds exactly `B1,B2,C1,D1`. Invalidate their [cached cell values](cached-cell-value.md) before evaluating another requested result; install the new input value for `A1`. The [cached cell values](cached-cell-value.md) of `A2` and `E1` remain valid because neither has a [directed path](directed-path.md) from `A1`.

<a id="image-downstream-invalidation-after-an-input-edit-and-a-different-formula-edit-creating-a-spreadsheet-circular-reference"></a>
![](spreadsheet-cycle-downstream-invalidation.png)

**[Figure 23](#image-downstream-invalidation-after-an-input-edit-and-a-different-formula-edit-creating-a-spreadsheet-circular-reference). Downstream invalidation after an input edit, and a different formula edit creating a spreadsheet circular reference**.

One recomputation in the restricted [topological order](topological-order.md) `B1,B2,C1,D1` gives $9,10,19,19/2$. Four [spreadsheet formulas](spreadsheet-formula.md) are recomputed, while `E1` stays at 16. Removing invalid values from the cache prevents a subtle error: a finished marker from the previous evaluation does not prove that the old value is correct after an edit. The affected set is conservative; a changed prerequisite might leave a consumer's value numerically equal, but this simple scheme still invalidates it. For a formula edit, update the incoming [directed edges](directed-edge.md) and corresponding outgoing consumer lists as well as invalidating the edited [spreadsheet cell](spreadsheet-cell.md) and its downstream consumers. Microsoft's documentation explicitly describes both direct and indirect dependents being marked for recalculation.[Dependence, Dirty Cells, and Recalculated Cells: paragraph beginning “When a structural change is made”; B1/A1 and C1/B1 dirty-cell example](excel-recalculation-by-microsoft.md)

For demand-driven evaluation, [memoization](memoization.md) combines with [depth-first search](depth-first-search.md). Each [spreadsheet cell](spreadsheet-cell.md) has one of three states: `UNSEEN` means no valid [cached cell value](cached-cell-value.md); `ACTIVE` means its evaluation is on the current [call stack](call-stack.md); `FINISHED` means a valid value is available. Initialize valid input [spreadsheet cells](spreadsheet-cell.md) as `FINISHED`. Start with all [spreadsheet formulas](spreadsheet-formula.md) `UNSEEN`, or retain only valid `FINISHED` entries after invalidation. The following original [algorithm](algorithm.md) uses an ordered `references` list and an `apply_formula` operation for each [spreadsheet formula](spreadsheet-formula.md):

```
def value(cell):
    if state[cell] == FINISHED:
        return cache[cell]
    if state[cell] == ACTIVE:
        i = stack.index(cell)
        raise CircularReference(stack[i:] + [cell])
    state[cell] = ACTIVE
    stack.append(cell)
    try:
        args = [value(p) for p in references[cell]]
        cache[cell] = apply_formula(cell, args)
        state[cell] = FINISHED
        return cache[cell]
    except Exception:
        state[cell] = UNSEEN
        raise
    finally:
        stack.pop()
```

Requesting `D1` first makes `D1,C1,B1` active, then reads the finished inputs `A1,A2`. `B1` finishes at 7. Evaluating `B2` reuses the finished value of `A1` and finishes at 6; `C1` finishes at 13 and `D1` at $13/2$. A later request for `D1` immediately returns its [cached cell value](cached-cell-value.md). The shared prerequisite `A1` is not a [directed cycle](directed-cycle.md): it was finished before the second request. The crucial distinction is between a previously visited [vertex](vertex-graph-theory.md) and a still-active [vertex](vertex-graph-theory.md). The exceptional path restores unfinished states while unwinding the [call stack](call-stack.md), so failed evaluations are not cached as successful results. MIT's [depth-first search](depth-first-search.md) notes use stack-duration marks to distinguish an [edge](edge-of-a-graph.md) to an active ancestor and to detect a [directed cycle](directed-cycle.md).[Lecture 14: Graphs II: Depth-First Search, printed pp. 3–4: stack-duration marks and cycle detection](6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-14-graphs-ii-depth-first-search.md)

With [adjacency lists](adjacency-list.md) and constant-time state/cache access, the structural work of a successful demand-driven evaluation is $O(|V_R|+|E_R|)$ in [big O notation](big-o-notation.md), where $V_R$ and $E_R$ are the requested [spreadsheet cells](spreadsheet-cell.md) and their recursively reached prerequisites and references. Each reached [spreadsheet formula](spreadsheet-formula.md) is computed once; each reference is inspected once. This [time complexity](time-complexity.md) counts dependency bookkeeping separately from the cost of the [arithmetic operations](arithmetic-operation.md). Detecting a [spreadsheet circular reference](spreadsheet-circular-reference.md) can additionally scan the current [call stack](call-stack.md) once to report its witness.

## ↑ Ancestors (4)

1. [Spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md)
2. [Spreadsheet](spreadsheet.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Cached cell value](cached-cell-value.md)
- [Memoization](memoization.md)
- [Spreadsheet cell](spreadsheet-cell.md)

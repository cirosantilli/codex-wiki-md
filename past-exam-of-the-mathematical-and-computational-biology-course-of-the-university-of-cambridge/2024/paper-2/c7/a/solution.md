<h1 id="c7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the supplied [BLOSUM62](../../../../../blosum62.md) entry for every diagonal move in the [Smith-Waterman algorithm](../../../../../smith-waterman-algorithm.md), while retaining the stipulated linear [gap penalty](../../../../../gap-penalty.md) of $-1$. If $q_i$ and $r_j$ are the current [amino acids](../../../../../amino-acid.md), the [dynamic programming](../../../../../dynamic-programming.md) recurrence is

$$
H_{ij}=\max\{0,H_{i,j-1}-1,H_{i-1,j}-1,H_{i-1,j-1}+B(q_i,r_j)\}.
$$

The zero option permits a new local start. The following original implementation also records the traceback coordinates needed in part (c); its tie ordering is left, up, diagonal, and an equal overall maximum replaces the previous best cell, as in the supplied convention:

```
def local_alignment(query,reference,alphabet,scores,gap=-1):
    lookup={aa:i for i,aa in enumerate(alphabet)}
    table=np.asarray(scores,dtype=int)
    height,width=len(query)+1,len(reference)+1
    H=np.zeros((height,width),dtype=int)
    back=np.zeros((height,width),dtype=np.int8)
    best=(0,0,0)
    for i,a in enumerate(query,1):
        for j,b in enumerate(reference,1):
            # Order implements the printed LEFT, UP, DIAGONAL tie priority.
            candidates=(0,H[i,j-1]+gap,H[i-1,j]+gap,
                        H[i-1,j-1]+int(table[lookup[a],lookup[b]]))
            value=max(candidates);H[i,j]=value
            back[i,j]=0 if value==0 else candidates.index(value)
            if value>=best[0]:best=(value,i,j)
    score,i,j=best;query_end,ref_end=i,j
    aq=[];ar=[]
    while H[i,j]>0:
        step=back[i,j]
        if step==1:aq.append('-');ar.append(reference[j-1]);j-=1
        elif step==2:aq.append(query[i-1]);ar.append('-');i-=1
        elif step==3:aq.append(query[i-1]);ar.append(reference[j-1]);i-=1;j-=1
    qa=''.join(reversed(aq));ra=''.join(reversed(ar));length=len(qa)
    identities=sum(a==b and a!='-' for a,b in zip(qa,ra))
    similarities=sum(a!='-' and b!='-' and table[lookup[a],lookup[b]]>0 for a,b in zip(qa,ra))
    gaps=sum(a=='-' or b=='-' for a,b in zip(qa,ra))
    return dict(query=qa,reference=ra,score=int(score),query_start=i+1,query_end=query_end,
                reference_start=j+1,reference_end=ref_end,query_length=len(query),reference_length=len(reference),
                alignment_length=length,identities=int(identities),similarities=int(similarities),gaps=int(gaps),
                identity_percent=100*identities/length if length else 0.,
                similarity_percent=100*similarities/length if length else 0.,gap_percent=100*gaps/length if length else 0.)

queries = {"baboon": baboon, "squirrel_monkey": squirrel_monkey,
           "dingo": dingo, "goldfish": goldfish}
alignments = {
    name: local_alignment(seq, reference_epo_receptor_human, amino_acids, bmat)
    for name, seq in queries.items()
}
for name, result in alignments.items():
    print(name, "score", result["score"])
    print(result["query"])
    print(result["reference"])
```

The resulting local [sequence alignments](../../../../../sequence-alignment.md), with the query above the reference, are:

**baboon; score 314**

```
SLLTPSDLDPLILTLSLILVLIVVLLTVLALLSHRRALKQKIWPGIPSPESEFEGLFTTHKG-FQL
SLLTPSDLDPLILTLSLILVVILVLLTVLALLSHRRALKQKIWPGIPSPESEFEGLFTTHKGNFQL
```

**squirrel monkey; score 278**

```
VCFWEEAASAGMGPDNYSFSYQL-DNEPWKR-CRLHQTPTARGVVRFWCSLPRADTSS
VCFWEEAASAGVGPGNYSFSYQLED-EPWK-LCRLHQAPTARGAVRFWCSLPTADTSS
```

**dingo; score 301**

```
MNHLW--THLWPG-VGSLCLLLAGAAWASLPKP-L-DPKFESKAALLAARAPEELLCFTERLEDLVCFWEE
MDHL-GAS-LWP-QVGSLCLLLAGAAWAP-P-PNLPDPKFESKAALLAARGPEELLCFTERLEDLVCFWEE
```

**goldfish; score 190**

```
L--LVLSIGLILC--L-LSLTVI-L-SHQKFLLK-KLWPDIPTPEHKFPGLFTVYKGDFKE-WMSH-NNGSM
LDPLILTLSLILVVILVL-LTVLALLSHRR-ALKQKIWPGIPSPESEFEGLFTTHKGNF-QLWL-YQNDGCL
```

The several short gaps are a consequence of the specified inexpensive linear [gap penalty](../../../../../gap-penalty.md); substituting a different default or an affine [gap penalty](../../../../../gap-penalty.md) would solve a different scoring problem.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [C7](../../c7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

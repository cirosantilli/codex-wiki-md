# Computer science

↑ **Parent:** [Codex Wiki](README.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Computer_science)

**Table of contents**

- [Encapsulation (computer programming)](#encapsulation-computer-programming)
- [Hash function](#hash-function)
  - [Almost strongly universal hash family](#almost-strongly-universal-hash-family)
    - [Polynomial almost strongly universal hashing](#polynomial-almost-strongly-universal-hashing)
  - [Universal hash family](#universal-hash-family)
    - [Strongly universal hash family](#strongly-universal-hash-family)
- [Conway Game of Life](#conway-game-of-life)
  - [One-row in-place Life update](#one-row-in-place-life-update)
- [Instruction pointer](#instruction-pointer)
- [Computer bus](#computer-bus)
  - [Direct memory access](#direct-memory-access)
- [Temporal locality](#temporal-locality)
- [Spreadsheet](#spreadsheet)
  - [Spreadsheet dependency evaluation](#spreadsheet-dependency-evaluation)
- [Operating system](#operating-system)
  - [Unix](#unix)
  - [Windows XP](#windows-xp)
  - [Polled input-output](#polled-input-output)
  - [Access matrix](#access-matrix)
  - [File system](#file-system)
    - [Buffer cache](#buffer-cache)
    - [File-system journaling](#file-system-journaling)
    - [Access control list](#access-control-list)
    - [File Allocation Table](#file-allocation-table)
      - [FAT32](#fat32)
    - [NTFS](#ntfs)
    - [Inode](#inode)
  - [Interrupt](#interrupt)
    - [Interrupt-driven input-output](#interrupt-driven-input-output)
    - [Interrupt masking](#interrupt-masking)
  - [Processor privilege level](#processor-privilege-level)
  - [Multics](#multics)
  - [Virtual memory](#virtual-memory)
    - [Thrashing (computer science)](#thrashing-computer-science)
    - [Working set](#working-set)
    - [Memory-mapped file](#memory-mapped-file)
    - [Memory segmentation](#memory-segmentation)
    - [Paging](#paging)
      - [Page replacement](#page-replacement)
        - [CLOCK page replacement](#clock-page-replacement)
        - [LRU replacement](#lru-replacement)
        - [FIFO page replacement](#fifo-page-replacement)
      - [Page fault](#page-fault)
      - [Translation lookaside buffer](#translation-lookaside-buffer)
      - [Page table](#page-table)
  - [Set-user-ID execution](#set-user-id-execution)
  - [Kernel (operating system)](#kernel-operating-system)
    - [Monolithic kernel](#monolithic-kernel)
    - [Microkernel](#microkernel)
    - [Kernel preemption](#kernel-preemption)
  - [Process scheduling](#process-scheduling)
    - [Context switch](#context-switch)
  - [Process (computing)](#process-computing)
    - [Thread (computing)](#thread-computing)
- [Data structure](#data-structure)
  - [FIFO queue](#fifo-queue)
    - [Two-list functional queue](#two-list-functional-queue)
  - [Binary tree](#binary-tree)
    - [Binary search tree](#binary-search-tree)
      - [Dictionary intersection](#dictionary-intersection)
    - [Full binary tree](#full-binary-tree)
  - [Linked list](#linked-list)
    - [Mutable list](#mutable-list)
    - [Lazy list](#lazy-list)
- [Programming language](#programming-language)
  - [Bit mask](#bit-mask)
  - [Bit shift](#bit-shift)
  - [Two's complement](#two-s-complement)
  - [Hexadecimal](#hexadecimal)
  - [Abstract syntax tree](#abstract-syntax-tree)
  - [Object-oriented programming](#object-oriented-programming)
    - [Encapsulation in object-oriented programming](#encapsulation-in-object-oriented-programming)
    - [Class (programming)](#class-programming)
  - [Java (programming language)](#java-programming-language)
    - [Java interface](#java-interface)
    - [Private field in Java](#private-field-in-java)
    - [Final class in Java](#final-class-in-java)
    - [Protected method in Java](#protected-method-in-java)
    - [Java array](#java-array)
    - [Generics in Java](#generics-in-java)
      - [Generic method in Java](#generic-method-in-java)
      - [Generic type invariance](#generic-type-invariance)
      - [Type erasure](#type-erasure)
  - [Exception handling](#exception-handling)
    - [ML exception type](#ml-exception-type)
  - [Type system](#type-system)
    - [Type variable](#type-variable)
      - [Occurs check](#occurs-check)
    - [Function type](#function-type)
    - [Parametric polymorphism](#parametric-polymorphism)
  - [Imperative programming](#imperative-programming)
  - [Functional programming](#functional-programming)
    - [Structural recursion](#structural-recursion)
  - [Standard ML](#standard-ml)
    - [ML reference type](#ml-reference-type)
- [Linial-Mansour-Nisan theorem](#linial-mansour-nisan-theorem)
- [Image processing](#image-processing)
  - [Image segmentation](#image-segmentation)
  - [Image signal](#image-signal)
    - [Image noise](#image-noise)
  - [Structure tensor](#structure-tensor)
  - [Image edge](#image-edge)
    - [Image edge enhancement](#image-edge-enhancement)
      - [Shock filter for image enhancement](#shock-filter-for-image-enhancement)
      - [Unsharp masking](#unsharp-masking)
  - [Diffusion image processing](#diffusion-image-processing)
    - [Diffusion tensor for image filtering](#diffusion-tensor-for-image-filtering)
    - [Image smoothing](#image-smoothing)
      - [Median filter](#median-filter)
        - [Disk-median curvature expansion](#disk-median-curvature-expansion)
      - [Gaussian blur](#gaussian-blur)
        - [Gaussian filtering Fourier multiplier](#gaussian-filtering-fourier-multiplier)
  - [Variational image processing](#variational-image-processing)
    - [Mumford–Shah functional](#mumford-shah-functional)
      - [Ambrosio–Tortorelli approximation](#ambrosio-tortorelli-approximation)
      - [Segmentation overfitting without an edge penalty](#segmentation-overfitting-without-an-edge-penalty)
      - [Nonconvexity of Mumford–Shah segmentation](#nonconvexity-of-mumford-shah-segmentation)
      - [Fixed-edge Euler-Lagrange equation for Mumford–Shah](#fixed-edge-euler-lagrange-equation-for-mumford-shah)
      - [Edge-free Mumford–Shah limit](#edge-free-mumford-shah-limit)
      - [Piecewise-constant Mumford–Shah problem](#piecewise-constant-mumford-shah-problem)
        - [Piecewise-constant segmentation contrast threshold](#piecewise-constant-segmentation-contrast-threshold)
        - [Segmentation interface curvature balance](#segmentation-interface-curvature-balance)
          - [Triple-junction angle in isotropic segmentation](#triple-junction-angle-in-isotropic-segmentation)
        - [Region means in piecewise-constant segmentation](#region-means-in-piecewise-constant-segmentation)
      - [Essential closedness of Mumford–Shah jump sets](#essential-closedness-of-mumford-shah-jump-sets)
- [Cryptography](#cryptography)
  - [One-way function](#one-way-function)
    - [One-way permutation](#one-way-permutation)
  - [Hard-core predicate](#hard-core-predicate)
  - [Bit commitment](#bit-commitment)
    - [Ensemble-steering attack on quantum bit commitment](#ensemble-steering-attack-on-quantum-bit-commitment)
  - [Quantum key distribution](#quantum-key-distribution)
    - [Premature basis announcement in quantum key distribution](#premature-basis-announcement-in-quantum-key-distribution)
  - [Coin flipping by telephone](#coin-flipping-by-telephone)
  - [Privacy amplification](#privacy-amplification)
  - [Message authentication](#message-authentication)
    - [Message authentication code](#message-authentication-code)
      - [Wegman–Carter authentication](#wegman-carter-authentication)
  - [Cryptographic nonce](#cryptographic-nonce)
  - [Public-key cryptography](#public-key-cryptography)
    - [Public key](#public-key)
    - [Private key](#private-key)
  - [Encryption](#encryption)
  - [Chosen-ciphertext attack](#chosen-ciphertext-attack)
  - [Cryptographic hash function](#cryptographic-hash-function)
    - [Collision resistance](#collision-resistance)
    - [Preimage resistance](#preimage-resistance)
  - [Digital signature](#digital-signature)
    - [ElGamal signature scheme](#elgamal-signature-scheme)
    - [RSA signature](#rsa-signature)
- [Algorithm](#algorithm)
  - [Strength reduction](#strength-reduction)
  - [Statistical program profiling](#statistical-program-profiling)
  - [Depth-first search](#depth-first-search)
  - [Memoization](#memoization)
  - [Merge sort](#merge-sort)
  - [Merge algorithm](#merge-algorithm)
  - [Binary search](#binary-search)
  - [Karatsuba multiplication](#karatsuba-multiplication)
  - [Randomized algorithm](#randomized-algorithm)
    - [Derandomization](#derandomization)
      - [Method of conditional probabilities](#method-of-conditional-probabilities)
    - [Probabilistic Turing machine](#probabilistic-turing-machine)
    - [One-sided error](#one-sided-error)
      - [RP (complexity)](#rp-complexity)
      - [co-RP](#co-rp)
    - [ZPP](#zpp)
    - [Error reduction for a randomized algorithm](#error-reduction-for-a-randomized-algorithm)
    - [Polynomial identity testing](#polynomial-identity-testing)
- [Theoretical computer science](#theoretical-computer-science)
  - [Formal language](#formal-language)
    - [Binary string](#binary-string)
      - [Counting binary strings with bounded ones](#counting-binary-strings-with-bounded-ones)
      - [Self-delimiting binary code](#self-delimiting-binary-code)
    - [Concatenation of formal languages](#concatenation-of-formal-languages)
    - [Empty language](#empty-language)
  - [Turing machine](#turing-machine)
    - [Instantaneous description of a Turing machine](#instantaneous-description-of-a-turing-machine)
    - [Instruction of a Turing machine](#instruction-of-a-turing-machine)
    - [Two-stack encoding of a Turing tape](#two-stack-encoding-of-a-turing-tape)
    - [Modular machine](#modular-machine)
      - [Group encoding of a modular machine](#group-encoding-of-a-modular-machine)
      - [Halting set at a designated terminal configuration](#halting-set-at-a-designated-terminal-configuration)
    - [Deterministic computation](#deterministic-computation)
    - [Reversible computation](#reversible-computation)
      - [Reversible circuit](#reversible-circuit)
    - [Nondeterministic Turing machine](#nondeterministic-turing-machine)
    - [Oracle machine](#oracle-machine)
      - [Relativization (complexity theory)](#relativization-complexity-theory)
  - [Boolean operation](#boolean-operation)
    - [Exclusive or](#exclusive-or)
    - [Negation](#negation)
    - [De Morgan's laws](#de-morgan-s-laws)
  - [Computational complexity theory](#computational-complexity-theory)
    - [Communication complexity](#communication-complexity)
    - [Promise problem](#promise-problem)
    - [Quantum complexity theory](#quantum-complexity-theory)
      - [BQP](#bqp)
        - [BQP error reduction](#bqp-error-reduction)
      - [Quantum witness](#quantum-witness)
      - [StoqMA](#stoqma)
      - [QMA](#qma)
        - [Witness acceptance operator](#witness-acceptance-operator)
          - [Trace-power witness optimization](#trace-power-witness-optimization)
        - [QMA error reduction](#qma-error-reduction)
        - [QMA parallel repetition with entangled witnesses](#qma-parallel-repetition-with-entangled-witnesses)
        - [Quantum verifier acceptance operator](#quantum-verifier-acceptance-operator)
      - [Quantum query complexity](#quantum-query-complexity)
        - [Polynomial method for quantum query lower bounds](#polynomial-method-for-quantum-query-lower-bounds)
        - [Exact quantum query complexity](#exact-quantum-query-complexity)
          - [Exact two-query majority algorithm](#exact-two-query-majority-algorithm)
        - [Quantum collision finding](#quantum-collision-finding)
          - [Brassard–Høyer–Tapp collision algorithm](#brassard-hoyer-tapp-collision-algorithm)
    - [Decision tree model](#decision-tree-model)
      - [Decision tree](#decision-tree)
        - [Decision-tree depth](#decision-tree-depth)
          - [Certificate complexity of a Boolean function](#certificate-complexity-of-a-boolean-function)
            - [Query certificate](#query-certificate)
          - [Evasive Boolean function](#evasive-boolean-function)
            - [Alternating-sum criterion for decision-tree evasiveness](#alternating-sum-criterion-for-decision-tree-evasiveness)
          - [Decision-tree adversary for a threshold function](#decision-tree-adversary-for-a-threshold-function)
    - [Computational problem](#computational-problem)
      - [Input (computer science)](#input-computer-science)
      - [Output (computing)](#output-computing)
      - [Decision problem](#decision-problem)
      - [Search problem](#search-problem)
        - [Search-to-decision reduction](#search-to-decision-reduction)
    - [Complexity class](#complexity-class)
      - [Time complexity](#time-complexity)
        - [Amortized analysis](#amortized-analysis)
        - [Polynomial time](#polynomial-time)
          - [Polynomial-time algorithm](#polynomial-time-algorithm)
          - [P (complexity)](#p-complexity)
            - [P-completeness](#p-completeness)
          - [NP (complexity)](#np-complexity)
            - [Certificate (complexity)](#certificate-complexity)
      - [Space complexity](#space-complexity)
        - [Polynomial space](#polynomial-space)
        - [Nondeterministic space complexity class](#nondeterministic-space-complexity-class)
          - [Savitch's theorem](#savitch-s-theorem)
            - [Space-bound discovery by exit reachability](#space-bound-discovery-by-exit-reachability)
        - [Deterministic space complexity class](#deterministic-space-complexity-class)
          - [PSPACE](#pspace)
        - [Polynomial-register real-arithmetic computation](#polynomial-register-real-arithmetic-computation)
        - [Logarithmic space](#logarithmic-space)
          - [L (complexity)](#l-complexity)
          - [NL (complexity)](#nl-complexity)
            - [NL-complete](#nl-complete)
              - [Directed cycle detection](#directed-cycle-detection)
              - [ST-connectivity](#st-connectivity)
                - [Configuration graph](#configuration-graph)
            - [co-NL](#co-nl)
              - [Immerman–Szelepcsényi theorem](#immerman-szelepcsenyi-theorem)
                - [Inductive counting](#inductive-counting)
    - [Polynomial-time reduction](#polynomial-time-reduction)
      - [Polynomial-time many-one reduction](#polynomial-time-many-one-reduction)
        - [Logspace many-one reduction](#logspace-many-one-reduction)
        - [NP-hardness](#np-hardness)
          - [NP-completeness](#np-completeness)
            - [Set cover problem](#set-cover-problem)
              - [Set cover reduction to equilibrium support](#set-cover-reduction-to-equilibrium-support)
            - [Cook-Levin theorem](#cook-levin-theorem)
            - [Subset sum problem](#subset-sum-problem)
            - [Boolean satisfiability problem](#boolean-satisfiability-problem)
              - [Integer programming formulation of satisfiability](#integer-programming-formulation-of-satisfiability)
              - [Maximum satisfiability](#maximum-satisfiability)
                - [Literal-frequency greedy approximation for MAX-SAT](#literal-frequency-greedy-approximation-for-max-sat)
              - [2UN-SAT](#2un-sat)
              - [Maximum 2-satisfiability](#maximum-2-satisfiability)
                - [Golden ratio approximation for MAX-2SAT](#golden-ratio-approximation-for-max-2sat)
                - [Seven-clause gadget for MAX-2SAT](#seven-clause-gadget-for-max-2sat)
              - [Boolean formula](#boolean-formula)
                - [Disjunctive normal form](#disjunctive-normal-form)
                - [Conjunctive normal form](#conjunctive-normal-form)
                  - [Tseytin transformation](#tseytin-transformation)
                - [Clause of a Boolean formula](#clause-of-a-boolean-formula)
                - [Boolean literal](#boolean-literal)
                - [Boolean variable](#boolean-variable)
              - [3-SAT](#3-sat)
              - [Horn clause](#horn-clause)
                - [Horn-SAT](#horn-sat)
                  - [Horn-SAT forward-chaining algorithm](#horn-sat-forward-chaining-algorithm)
            - [Quadratic-equation satisfiability over F2](#quadratic-equation-satisfiability-over-f2)
            - [Ladner's theorem](#ladner-s-theorem)
    - [Circuit complexity](#circuit-complexity)
      - [NC1](#nc1)
        - [MOD3 binary divisibility problem](#mod3-binary-divisibility-problem)
        - [Balanced finite-monoid reduction circuit](#balanced-finite-monoid-reduction-circuit)
      - [Boolean circuit](#boolean-circuit)
        - [Circuit size](#circuit-size)
        - [Depth of a Boolean circuit](#depth-of-a-boolean-circuit)
        - [Circuit value problem](#circuit-value-problem)
          - [AND-NOT circuit value problem](#and-not-circuit-value-problem)
        - [Circuit satisfiability problem](#circuit-satisfiability-problem)
        - [Threshold function](#threshold-function)
          - [Majority function](#majority-function)
            - [Block conjunction of three-bit majorities](#block-conjunction-of-three-bit-majorities)
        - [Dual Boolean function](#dual-boolean-function)
      - [Circuit family](#circuit-family)
        - [Circuit size class](#circuit-size-class)
          - [Truth-table upper bound for circuit size](#truth-table-upper-bound-for-circuit-size)
        - [Polynomial-size circuit family](#polynomial-size-circuit-family)
          - [Undecidable unary languages with linear-size circuits](#undecidable-unary-languages-with-linear-size-circuits)
          - [P/poly](#p-poly)
      - [Constant-depth circuit complexity](#constant-depth-circuit-complexity)
        - [Håstad switching lemma](#hastad-switching-lemma)
          - [Switching-lemma depth reduction](#switching-lemma-depth-reduction)
      - [Monotone circuit complexity](#monotone-circuit-complexity)
        - [Monotone circuit](#monotone-circuit)
        - [Superpolynomial monotone clique lower bound](#superpolynomial-monotone-clique-lower-bound)
        - [Razborov approximation method](#razborov-approximation-method)
          - [Finite lattice approximation for monotone clique circuits](#finite-lattice-approximation-for-monotone-clique-circuits)
            - [Negative colouring error of a forced-set closure](#negative-colouring-error-of-a-forced-set-closure)
            - [Positive clique error of a truncated lattice meet](#positive-clique-error-of-a-truncated-lattice-meet)
          - [Razborov closure](#razborov-closure)
            - [Sunflower bound for minimal members of a Razborov-closed family](#sunflower-bound-for-minimal-members-of-a-razborov-closed-family)
            - [Minimal-member bound for a Razborov-closed family](#minimal-member-bound-for-a-razborov-closed-family)
          - [Razborov gate-by-gate approximation lemma](#razborov-gate-by-gate-approximation-lemma)
      - [Natural proof](#natural-proof)
        - [Constructive property of Boolean functions](#constructive-property-of-boolean-functions)
        - [Large property of Boolean functions](#large-property-of-boolean-functions)
        - [Useful property against a circuit class](#useful-property-against-a-circuit-class)
        - [Razborov–Rudich natural-proofs barrier](#razborov-rudich-natural-proofs-barrier)
      - [Pseudorandom function family](#pseudorandom-function-family)
    - [Counting complexity](#counting-complexity)
      - [Valiant's permanent reduction](#valiant-s-permanent-reduction)
        - [Variable gadget in Valiant's permanent reduction](#variable-gadget-in-valiant-s-permanent-reduction)
        - [Clause gadget in Valiant's permanent reduction](#clause-gadget-in-valiant-s-permanent-reduction)
        - [Exclusive-or gadget in Valiant's permanent reduction](#exclusive-or-gadget-in-valiant-s-permanent-reduction)
        - [Binary path-counting gadget](#binary-path-counting-gadget)
      - [Balanced number 3-SAT](#balanced-number-3-sat)
    - [Polynomial hierarchy](#polynomial-hierarchy)
      - [Second level of the polynomial hierarchy](#second-level-of-the-polynomial-hierarchy)
      - [Karp–Lipton theorem](#karp-lipton-theorem)
    - [Primality testing](#primality-testing)
      - [Miller-Rabin primality test](#miller-rabin-primality-test)
      - [Fermat primality test](#fermat-primality-test)
      - [Pseudoprime base](#pseudoprime-base)
      - [Agrawal–Biswas primality test](#agrawal-biswas-primality-test)

## Encapsulation (computer programming)

↑ **Parent:** [Computer science](computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Encapsulation_(computer_programming))

[Encapsulation](#encapsulation-computer-programming) bundles related program state and operations or hides implementation details behind an interface. [Encapsulation in object-oriented programming](#encapsulation-in-object-oriented-programming) realizes this through objects and their permitted operations; encapsulation also applies to modules outside object-oriented programs.

## Hash function

↑ **Parent:** [Computer science](computer-science.md)

A function mapping a large input set to a smaller set of hash values. It is used to index data or summarize an input; its required properties depend on the task. A [cryptographic hash function](#cryptographic-hash-function) is designed for computational security properties, whereas a [universal hash family](#universal-hash-family) controls collision probabilities under random choice of the function.

### Almost strongly universal hash family

↑ **Parent:** [Hash function](#hash-function)

In the convention used here, an $\varepsilon$-almost-strongly-universal family has uniform individual outputs and satisfies the displayed bound for every pair of distinct inputs and specified outputs. Equivalently $\Pr[h(y)=v\mid h(x)=u]\leq\varepsilon$. Necessarily $\varepsilon\geq1/q$, and equality gives a [strongly universal hash family](#strongly-universal-hash-family). Bounds greater than $1/q$ need not imply exact universality; the hierarchy therefore does not put this class under [universal hash family](#universal-hash-family).

#### Polynomial almost strongly universal hashing

↑ **Parent:** [Almost strongly universal hash family](#almost-strongly-universal-hash-family)

For fixed-length messages in $\mathbb F_q^L$, choose independent uniform field elements $a,b$. Each output is uniform because $b$ masks it. For distinct messages and prescribed output difference $d$, the equation $\sum_{j=1}^L(m'_j-m_j)a^j=d$ is a nonzero polynomial equation of degree at most $L$, so the [root bound for a polynomial](polynomial.md#lagrange-root-bound-over-a-field) gives at most $L$ choices of $a$. The joint output probability is at most $L/q^2$. Thus the family is $(L/q)$-almost strongly universal when $L<q$. Starting the message polynomial at power one matters: using a freely varying message coefficient at power zero would permit a known constant tag shift after observing one tag.

### Universal hash family

↑ **Parent:** [Hash function](#hash-function)

For finite output set of size $q$, choose $h$ uniformly from the family. Universality of order two means the displayed collision bound for every distinct pair of inputs. It does not require uniform individual hash values or independence of two output values. [Strongly universal hash families](#strongly-universal-hash-family) impose both of those stronger requirements.

#### Strongly universal hash family

↑ **Parent:** [Universal hash family](#universal-hash-family)

For every distinct pair of inputs and every specified pair of output values, the displayed joint probability holds. Thus outputs at distinct inputs are independent and uniform. Summing over equal output values gives the [universal hash family](#universal-hash-family) collision bound with equality.

## Conway Game of Life

↑ **Parent:** [Computer science](computer-science.md)

A cellular automaton on a square grid with eight adjacent neighbors. A live cell survives with two or three live neighbors; a dead cell is born with three. All decisions use the previous generation. Finite boards need an explicit convention for locations outside the board.

// Destination: computer-science.bigb

### One-row in-place Life update

↑ **Parent:** [Conway Game of Life](#conway-game-of-life)

On a finite rectangular boolean board, retain the preceding row's old values in one auxiliary row. Before overwriting a column, retain rolling sums of the old three-cell vertical columns. Their sum minus the old center is the old neighbor count. Read the next column before changing the current one; replace the saved row entry by the old current cell. This uses linear-row auxiliary storage and linear-board time without asynchronous update artifacts.

// Destination: foundations-of-mathematics.bigb

## Instruction pointer

↑ **Parent:** [Computer science](computer-science.md)

A processor register identifying the current or next instruction according to the architecture. A timer interrupt can record the saved instruction address of a running process, permitting [statistical program profiling](#statistical-program-profiling) without source code.

// Destination: computer-science.bigb

## Computer bus

↑ **Parent:** [Computer science](computer-science.md)

A communication interconnect carrying addresses or destinations, data, and control information such as read/write requests and completion. A shared bus also needs rules for granting access when multiple devices can initiate transfers.

// Destination: computer-science.bigb

### Direct memory access

↑ **Parent:** [Computer bus](#computer-bus)

Transfer between a device and memory without a processor instruction for each item. The processor sets up a transfer and later observes completion. Multiple bus initiators require arbitration; safe access also requires correct buffer addresses, protection and any necessary cache-coherence handling.

// Destination: computer-science.bigb

## Temporal locality

↑ **Parent:** [Computer science](computer-science.md)

The tendency of a recently used item to be used again soon. It motivates [LRU replacement](#lru-replacement) and recency-based approximations, but is a workload property rather than a guarantee for every future access.

// Destination: computer-science.bigb

## Spreadsheet

↑ **Parent:** [Computer science](computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spreadsheet)

// Target: computer-science.bigb

### Spreadsheet dependency evaluation

↑ **Parent:** [Spreadsheet](#spreadsheet)

Evaluate numeric formula dependencies using [depth-first search](#depth-first-search) and [memoization](#memoization), or a [topological ordering](combinatorics.md#topological-ordering). Marking active evaluations detects cycles; repeated numerical sweeps need not terminate or determine a unique result.

// Target: computer-science.bigb

## Operating system

↑ **Parent:** [Computer science](computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Operating_system)

// Target: computer-science.bigb

### Unix

↑ **Parent:** [Operating system](#operating-system)

An operating-system family with process, file and pipe abstractions. The traditional discretionary file-permission model separates owner, group and other users and read, write and execute rights. Individual Unix systems can add richer [access control lists](#access-control-list) and other protection mechanisms.

// Destination: computer-science.bigb

### Windows XP

↑ **Parent:** [Operating system](#operating-system)

A member of the Windows NT operating-system family. Executive services such as object, memory and input-output management execute in privileged kernel mode. Its object-level [access control lists](#access-control-list) and subject tokens permit finer authorization policies than traditional owner-group-other file permissions.

// Destination: computer-science.bigb

### Polled input-output

↑ **Parent:** [Operating system](#operating-system)

A processor checks device status explicitly, typically repeatedly, until service is possible. Frequent predictable events or very short waits can make polling cheaper than an [interrupt](#interrupt). Infrequent or long waits waste processor time if busy polling is used.

// Destination: computer-science.bigb

### Access matrix

↑ **Parent:** [Operating system](#operating-system)

An authorization table with subjects or protection domains as rows, objects as columns, and sets of allowed operations as entries. An [access control list](#access-control-list) stores an object column; a capability list stores a subject row. This representation is not a numerical linear map and has no ordinary floating-point matrix inverse.

// Destination: computer-science.bigb

### File system

↑ **Parent:** [Operating system](#operating-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/File_system)

// Target: computer-science.bigb

#### Buffer cache

↑ **Parent:** [File system](#file-system)

A memory cache of device blocks indexed by device identity and block number. A hit avoids slow device access; a miss obtains a buffer and reads the block. Dirty buffers carry modified data that must be written before reuse, and pinned buffers cannot be evicted while an operation uses them. Deferred writes improve throughput but need explicit durability handling.

// Destination: computer-science.bigb

#### File-system journaling

↑ **Parent:** [File system](#file-system)

Recording intended metadata updates in a recoverable log before applying them. Journaling aids crash recovery; metadata journaling alone does not guarantee preservation of all recent file data.

// Target: computer-science.bigb

#### Access control list

↑ **Parent:** [File system](#file-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Access_control_list)

// Target: computer-science.bigb

#### File Allocation Table

↑ **Parent:** [File system](#file-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/File_Allocation_Table)

// Target: computer-science.bigb

##### FAT32

↑ **Parent:** [File Allocation Table](#file-allocation-table)

// Target: computer-science.bigb

#### NTFS

↑ **Parent:** [File system](#file-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/NTFS)

// Target: computer-science.bigb

#### Inode

↑ **Parent:** [File system](#file-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inode)

// Target: computer-science.bigb

### Interrupt

↑ **Parent:** [Operating system](#operating-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interrupt)

// Target: computer-science.bigb

#### Interrupt-driven input-output

↑ **Parent:** [Interrupt](#interrupt)

A device signals an [interrupt](#interrupt) when it needs service, allowing the processor to perform unrelated work until then. Delivery, entry and completion have costs, so very high event rates can favor [polled input-output](#polled-input-output) or a combined scheme.

// Destination: computer-science.bigb

#### Interrupt masking

↑ **Parent:** [Interrupt](#interrupt)

Disabling selected asynchronous interrupt delivery, normally under privileged control. It does not necessarily disable processor exceptions, nonmaskable interrupts or activity on other processors.

// Target: computer-science.bigb

### Processor privilege level

↑ **Parent:** [Operating system](#operating-system)

// Target: computer-science.bigb

### Multics

↑ **Parent:** [Operating system](#operating-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multics)

// Target: computer-science.bigb

### Virtual memory

↑ **Parent:** [Operating system](#operating-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Virtual_memory)

// Target: computer-science.bigb

#### Thrashing (computer science)

↑ **Parent:** [Virtual memory](#virtual-memory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thrashing_(computer_science))

Excessive paging when active memory demand exceeds available frames, leaving little useful computation between [page faults](#page-fault).

// Target: computer-science.bigb

#### Working set

↑ **Parent:** [Virtual memory](#virtual-memory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Working_set)

Pages recently used by a process within a declared time or reference window. Keeping the active processes' combined working sets resident reduces [memory thrashing](#thrashing-computer-science).

// Target: computer-science.bigb

#### Memory-mapped file

↑ **Parent:** [Virtual memory](#virtual-memory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Memory-mapped_file)

// Target: computer-science.bigb

#### Memory segmentation

↑ **Parent:** [Virtual memory](#virtual-memory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Memory_segmentation)

// Target: computer-science.bigb

#### Paging

↑ **Parent:** [Virtual memory](#virtual-memory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Paging)

// Target: computer-science.bigb

##### Page replacement

↑ **Parent:** [Paging](#paging)

Choosing a resident page to evict when a new page needs a memory frame. A dirty victim must be preserved before reuse. Replacement policy should consider future reuse and the overhead of tracking past references.

// Destination: computer-science.bigb

###### CLOCK page replacement

↑ **Parent:** [Page replacement](#page-replacement)

Keep frames in a circular list with a reference flag and a scanning hand. Clear set flags while scanning; choose the first eligible frame with a clear flag. This second chance approximates [LRU replacement](#lru-replacement) with cheaper tracking. When hardware reference flags are absent, revoking a mapping and handling its first later [page fault](#page-fault) can supply a software reference observation.

// Destination: computer-science.bigb

###### LRU replacement

↑ **Parent:** [Page replacement](#page-replacement)

Evict the least recently accessed eligible item. Exact recency tracking on every memory reference can be expensive, whereas accesses to a [buffer cache](#buffer-cache) already pass through software. Recency captures [temporal locality](#temporal-locality) but can be defeated by a one-pass scan.

// Destination: computer-science.bigb

###### FIFO page replacement

↑ **Parent:** [Page replacement](#page-replacement)

Evict the page loaded earliest among currently resident pages, without refreshing its position on access. It is simple but ignores recent reuse and can evict a frequently accessed page.

// Destination: computer-science.bigb

##### Page fault

↑ **Parent:** [Paging](#paging)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Page_fault)

// Target: computer-science.bigb

##### Translation lookaside buffer

↑ **Parent:** [Paging](#paging)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Translation_lookaside_buffer)

// Target: computer-science.bigb

##### Page table

↑ **Parent:** [Paging](#paging)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Page_table)

// Target: computer-science.bigb

### Set-user-ID execution

↑ **Parent:** [Operating system](#operating-system)

Execution of a suitable executable with effective user identity set to its owner. A privileged executable writable by untrusted users permits code replacement and privilege escalation.

// Target: computer-science.bigb

### Kernel (operating system)

↑ **Parent:** [Operating system](#operating-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kernel_(operating_system))

// Target: computer-science.bigb

#### Monolithic kernel

↑ **Parent:** [Kernel (operating system)](#kernel-operating-system)

A kernel design in which major operating-system services execute within one privileged address space and can call one another directly. Avoiding cross-domain communication can improve performance, while increasing the trusted code base and the reach of a faulty service.

// Destination: computer-science.bigb

#### Microkernel

↑ **Parent:** [Kernel (operating system)](#kernel-operating-system)

A kernel design retaining a small set of essential mechanisms in privileged code while services communicate across protection boundaries. Isolation and modularity are benefits; extra messages and address-space transitions can cost time compared with a [monolithic kernel](#monolithic-kernel). Neither architecture alone establishes a universal performance ordering.

// Destination: computer-science.bigb

#### Kernel preemption

↑ **Parent:** [Kernel (operating system)](#kernel-operating-system)

Allows a running kernel execution to be involuntarily suspended for another schedulable context. Interrupt delivery and voluntary blocking are separate mechanisms.

// Target: computer-science.bigb

### Process scheduling

↑ **Parent:** [Operating system](#operating-system)

// Target: computer-science.bigb

#### Context switch

↑ **Parent:** [Process scheduling](#process-scheduling)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Context_switch)

// Target: computer-science.bigb

### Process (computing)

↑ **Parent:** [Operating system](#operating-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Process_(computing))

A running program with an address space, execution context and operating-system resources.

// Target: computer-science.bigb

#### Thread (computing)

↑ **Parent:** [Process (computing)](#process-computing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thread_(computing))

An execution stream with its own registers and stack, usually sharing its process address space and resources with other threads.

// Target: computer-science.bigb

## Data structure

↑ **Parent:** [Computer science](computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Data_structure)

// Target: computer-science.bigb

### FIFO queue

↑ **Parent:** [Data structure](#data-structure)

A [data structure](#data-structure) in which insertion occurs at the rear and removal at the front. The earliest unremoved item is removed first. This is a queue as an abstract data structure, rather than a stochastic [queueing theory](queueing-theory.md) model.

// Destination: computer-science.bigb

#### Two-list functional queue

↑ **Parent:** [FIFO queue](#fifo-queue)

Represent the abstract sequence by `front @ rev rear`. Keep the front nonempty unless both lists are empty. Prepending to the rear enqueues; when the front is exhausted, reverse the rear once. Along a single sequence of uses, each element crosses between lists at most once, giving constant [amortized analysis](#amortized-analysis) cost per operation. Reusing an old persistent version can repeat a reversal and needs a separate analysis.

// Destination: computer-science.bigb

### Binary tree

↑ **Parent:** [Data structure](#data-structure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_tree)

// Target: computer-science.bigb

#### Binary search tree

↑ **Parent:** [Binary tree](#binary-tree)

A [binary tree](#binary-tree) storing key-value entries with smaller keys in the left subtree and larger keys in the right subtree. Unique keys identify a partial map. Lookup follows a root-to-leaf path; without balancing the height may be linear in the number of entries.

// Destination: computer-science.bigb

##### Dictionary intersection

↑ **Parent:** [Binary search tree](#binary-search-tree)

For partial maps $D_1,D_2$, retain exactly entries $(k,v)$ for which both maps define the same value $v$ at $k$. Merely sharing a key is insufficient. Traverse one [binary search tree](#binary-search-tree), look up each key in the other, and insert only equal-value matches into the result.

// Destination: computer-science.bigb

#### Full binary tree

↑ **Parent:** [Binary tree](#binary-tree)

A full binary tree is a binary tree in which every nonleaf has exactly two children. A binary [Huffman code](information-theory.md#huffman-code) with at least two positive-probability symbols has a full code tree: a vertex with only one child could be suppressed to shorten all codewords below it.

// Target: probability-and-statistics.bigb

### Linked list

↑ **Parent:** [Data structure](#data-structure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linked_list)

// Target: computer-science.bigb

#### Mutable list

↑ **Parent:** [Linked list](#linked-list)

A [linked list](#linked-list) whose links are held in [ML reference type](#ml-reference-type) cells and may be changed. Deleting a node updates the link that reaches it, including the root link when the head is removed. Aliases of links observe these mutations; no fresh list spine is needed for destructive filtering.

// Destination: computer-science.bigb

#### Lazy list

↑ **Parent:** [Linked list](#linked-list)

A [linked list](#linked-list) whose future structure is obtained by calling a delayed computation. In [Standard ML](#standard-ml), `unit -> node` delays a computation until demand. Filtering may need to force arbitrarily many rejected elements to produce its next retained element; filtering an infinite list need not produce a result. Delay alone does not imply [memoization](#memoization).

// Destination: computer-science.bigb

## Programming language

↑ **Parent:** [Computer science](computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Programming_language)

// Target: computer-science.bigb

### Bit mask

↑ **Parent:** [Programming language](#programming-language)

A word selecting specified binary positions under a bitwise operation. To extract a stored bit at position $b$, logically shift by $b$ and combine with the mask `1`. Grouping thirty-two cells into one [Java](#java-programming-language) integer permits a compact representation of a [Conway Game of Life](#conway-game-of-life) board.

// Destination: computer-science.bigb

### Bit shift

↑ **Parent:** [Programming language](#programming-language)

A fixed-width left shift discards high bits and inserts low zeros. A logical right shift inserts high zeros; an arithmetic right shift propagates the sign bit. In [Java](#java-programming-language), `<<`, `>>>` and `>>` distinguish these operations. Left shift by $k$ is multiplication by $2^k$ modulo the word modulus.

// Destination: computer-science.bigb

<h3 id="two-s-complement">Two's complement</h3>

↑ **Parent:** [Programming language](#programming-language)

For a fixed word width $w$, signed integers have the same bit patterns as residues modulo $2^w$. The leading bit has negative positional weight in the signed interpretation. Reading the same bits as unsigned gives $2^w+x$ for a negative signed integer $x$.

// Destination: computer-science.bigb

### Hexadecimal

↑ **Parent:** [Programming language](#programming-language)

Base-sixteen representation, with digit values zero through fifteen conventionally written `0` through `9` and `a` through `f`. A group of four binary digits selects one hexadecimal digit.

// Destination: computer-science.bigb

### Abstract syntax tree

↑ **Parent:** [Programming language](#programming-language)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Abstract_syntax_tree)

// Target: computer-science.bigb

### Object-oriented programming

↑ **Parent:** [Programming language](#programming-language)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Object-oriented_programming)

// Target: computer-science.bigb

#### Encapsulation in object-oriented programming

↑ **Parent:** [Object-oriented programming](#object-oriented-programming)

In [object-oriented programming](#object-oriented-programming), encapsulation packages an object's state with the operations that act on it and can restrict direct access to its implementation. It is the object-oriented use of [encapsulation](#encapsulation-computer-programming).

#### Class (programming)

↑ **Parent:** [Object-oriented programming](#object-oriented-programming)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Class_(programming))

// Target: computer-science.bigb

### Java (programming language)

↑ **Parent:** [Programming language](#programming-language)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Java_(programming_language))

// Target: computer-science.bigb

#### Java interface

↑ **Parent:** [Java (programming language)](#java-programming-language)

An interface specifies a type contract that independent classes can implement. Code accepting the interface can operate on multiple implementations, avoiding dependence on one concrete class. A class may implement several interfaces despite having only one direct class superclass.

// Destination: computer-science.bigb

#### Private field in Java

↑ **Parent:** [Java (programming language)](#java-programming-language)

A field declared `private` is hidden from ordinary external source-level access. Library methods can enforce invariants and change the representation without exposing storage to clients. Returning a mutable internal object can still undermine this [encapsulation in object-oriented programming](#encapsulation-in-object-oriented-programming).

// Destination: computer-science.bigb

#### Final class in Java

↑ **Parent:** [Java (programming language)](#java-programming-language)

A class declared `final` cannot be subclassed. This can protect an implementation contract against overriding in an untrusted subclass. It does not by itself make the class immutable, and it rules out subclass-based customization.

// Destination: computer-science.bigb

#### Protected method in Java

↑ **Parent:** [Java (programming language)](#java-programming-language)

A `protected` method is accessible to code in its package and, subject to the cross-package receiver restriction, to subclasses elsewhere. It can expose a subclass customization hook without being a public client operation. Protected access is broader than subclass-only access.

// Destination: computer-science.bigb

#### Java array

↑ **Parent:** [Java (programming language)](#java-programming-language)

Java arrays are fixed-length objects. A two-dimensional array is an array of row-array references, so rows can have different lengths and must be allocated separately if not allocated by the initial expression.

// Target: computer-science.bigb

#### Generics in Java

↑ **Parent:** [Java (programming language)](#java-programming-language)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generics_in_Java)

// Target: computer-science.bigb

##### Generic method in Java

↑ **Parent:** [Generics in Java](#generics-in-java)

A method declaring its own type parameters, for example `<T> List<T> singletonList(T value)`. The type parameter connects argument and result types and permits compile-time checking without casts at ordinary call sites. A method mentioning only a generic class's type parameter need not itself be a generic method.

// Destination: computer-science.bigb

##### Generic type invariance

↑ **Parent:** [Generics in Java](#generics-in-java)

Even when `S` is a subtype of `T`, neither `G<S>` nor `G<T>` is generally a subtype of the other. This prevents unsafe writes into mutable generic containers. Wildcards express restricted views.

// Target: computer-science.bigb

##### Type erasure

↑ **Parent:** [Generics in Java](#generics-in-java)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Type_erasure)

// Target: computer-science.bigb

### Exception handling

↑ **Parent:** [Programming language](#programming-language)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exception_handling)

// Target: computer-science.bigb

#### ML exception type

↑ **Parent:** [Exception handling](#exception-handling)

In [Standard ML](#standard-ml), `exn` is an extensible datatype of exception packets. Fresh declarations introduce constructors, optionally with payloads; rebinding can alias an existing constructor; `raise` propagates a packet and `handle` performs dynamic pattern-based recovery.

// Target: computer-science.bigb

### Type system

↑ **Parent:** [Programming language](#programming-language)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Type_system)

// Target: computer-science.bigb

#### Type variable

↑ **Parent:** [Type system](#type-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Type_variable)

// Target: computer-science.bigb

##### Occurs check

↑ **Parent:** [Type variable](#type-variable)

A recursive check that a given type variable is absent from a type expression. It prevents constructing a cyclic infinite type when solving an equation such as $\alpha=\alpha\to\beta$.

#### Function type

↑ **Parent:** [Type system](#type-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Function_type)

// Target: computer-science.bigb

#### Parametric polymorphism

↑ **Parent:** [Type system](#type-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parametric_polymorphism)

A function or data structure is parameterized by types and can operate uniformly over their instantiations.

// Target: computer-science.bigb

### Imperative programming

↑ **Parent:** [Programming language](#programming-language)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Imperative_programming)

// Target: computer-science.bigb

### Functional programming

↑ **Parent:** [Programming language](#programming-language)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Functional_programming)

// Target: computer-science.bigb

#### Structural recursion

↑ **Parent:** [Functional programming](#functional-programming)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Structural_recursion)

Recursion following the constructors of a finite inductive datatype. Correctness is naturally proved by [structural induction](foundations-of-mathematics.md#structural-induction).

// Target: computer-science.bigb

### Standard ML

↑ **Parent:** [Programming language](#programming-language)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Standard_ML)

A strict functional [programming language](#programming-language) with [parametric polymorphism](#parametric-polymorphism), algebraic datatypes, [exception handling](#exception-handling) and mutable references.

// Target: computer-science.bigb

#### ML reference type

↑ **Parent:** [Standard ML](#standard-ml)

A mutable cell holding a value of type `'a`. `ref` allocates a cell, `!` reads it and `:=` updates it. Aliases share the same cell; the value restriction prevents unsafe polymorphic mutable storage.

// Target: computer-science.bigb

## Linial-Mansour-Nisan theorem

↑ **Parent:** [Computer science](computer-science.md)

The Linial-Mansour-Nisan theorem bounds the high-degree Fourier weight of a Boolean function computed by a small bounded-depth circuit.

## Image processing

↑ **Parent:** [Computer science](computer-science.md)

[Image processing](#image-processing) transforms recorded [image signal](#image-signal) data to remove noise, recover detail or extract structure. [Variational image processing](#variational-image-processing) describes desired reconstructions through energies, while [diffusion image processing](#diffusion-image-processing) describes filtering through evolution equations.

### Image segmentation

↑ **Parent:** [Image processing](#image-processing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Image_segmentation)

[Image segmentation](#image-segmentation) divides an [image signal](#image-signal) domain into regions according to a chosen criterion, such as approximately constant or smoothly varying intensity. The [Mumford–Shah segmentation model](#mumford-shah-functional) balances fidelity, within-region smoothness and [image edge](#image-edge) length. An intensity segmentation need not coincide with semantic object identities.

### Image signal

↑ **Parent:** [Image processing](#image-processing)

A grey-value [image signal](#image-signal) is a scalar function on an [image signal](#image-signal) domain or an array of pixel values. Continuous [image processing](#image-processing) models use spaces such as $L^2$, [Sobolev spaces](sobolev-space.md) or the [BV space](inverse-problem.md#function-of-bounded-variation-on-a-domain), while discrete models use finite-dimensional arrays. The chosen representation distinguishes smooth transitions, noise and [image edges](#image-edge).

#### Image noise

↑ **Parent:** [Image signal](#image-signal)

Image noise is unwanted variation in an observed [image signal](#image-signal). In an additive model $g=u+\eta$, Gaussian noise motivates a squared data-fidelity penalty, while other statistics require different penalties. [Image smoothing](#image-smoothing) suppresses rapid fluctuations, but a filter must distinguish noise from genuine [image edges](#image-edge).

### Structure tensor

↑ **Parent:** [Image processing](#image-processing)

For a smoothed [image signal](#image-signal) $u_\sigma$, average the [gradient](calculus.md#gradient) outer product as $J_\rho=G_\rho*(\nabla u_\sigma\nabla u_\sigma^T)$. The dominant [eigenvector](linear-operator-theory.md#eigenvector) estimates the normal to a coherent [image edge](#image-edge), and [eigenvalue](linear-operator-theory.md#eigenvalue) contrast [measures](measure-theory.md#measure) local directional structure. Two distinct scales separate differentiation from orientation averaging.

### Image edge

↑ **Parent:** [Image processing](#image-processing)

An [image edge](#image-edge) is a rapid grey-value transition, modeled as a large [gradient](calculus.md#gradient) or a jump discontinuity. It differs from an [edge of a graph](graph-theory.md#edge-of-a-graph). Variational models can penalize [image edge](#image-edge) length, while [diffusion image processing](#diffusion-image-processing) estimates [image edge](#image-edge) directions to limit [image smoothing](#image-smoothing) across them.

#### Image edge enhancement

↑ **Parent:** [Image edge](#image-edge)

[image edge](#image-edge) enhancement increases the apparent sharpness or contrast of an [image edge](#image-edge). [Unsharp masking](#unsharp-masking) gives bounded linear high-frequency amplification; backward normal diffusion in the [Perona-Malik equation](diffusion-equation.md#perona-malik-equation) gives formal nonlinear sharpening with [ill-posedness](partial-differential-equation.md#ill-posed-problem) risks. Positive diffusion tensors chiefly preserve or connect structure rather than perform unbounded backward diffusion.

##### Shock filter for image enhancement

↑ **Parent:** [Image edge enhancement](#image-edge-enhancement)

The formal shock-filter equation $u_t=-\operatorname{sign}(\Delta u)|\nabla u|$ steepens transitions around inflection boundaries. It is a Hamilton–Jacobi-type transport mechanism rather than positive diffusion. Combining it with controlled forward [image smoothing](#image-smoothing) limits noise amplification.

##### Unsharp masking

↑ **Parent:** [Image edge enhancement](#image-edge-enhancement)

Subtract a smoothed [image signal](#image-signal) and add a scaled residual: $u=g+\lambda(g-G_t*g)$. The Fourier multiplier $1+\lambda(1-e^{-t|\xi|^2})$ is bounded by $1+\lambda$. This enhances apparent contrast but also amplifies noise; it is not a stable exact inverse of heat [image smoothing](#image-smoothing).

### Diffusion image processing

↑ **Parent:** [Image processing](#image-processing)

Diffusion filtering evolves an observed [image signal](#image-signal) using a [diffusion equation](diffusion-equation.md). The [heat equation](diffusion-equation.md#heat-equation) gives Gaussian [image smoothing](#image-smoothing), while gradient-dependent or tensor-dependent diffusion can reduce transport across [image edges](#image-edge). A [image smoothing](#image-smoothing) scale, stopping rule and appropriate boundary conditions are part of the filter.

#### Diffusion tensor for image filtering

↑ **Parent:** [Diffusion image processing](#diffusion-image-processing)

A positive tensor $D=a_ne_ne_n^T+a_te_te_t^T$ selects different diffusion strengths normal and tangent to an estimated [image edge](#image-edge). Taking $0<a_n\ll a_t$ smooths along the [image edge](#image-edge) while reducing mixing across it. A [structure tensor](#structure-tensor) provides robust orientation estimates. Positive [eigenvalues](linear-operator-theory.md#eigenvalue) ensure forward local parabolicity.

#### Image smoothing

↑ **Parent:** [Diffusion image processing](#diffusion-image-processing)

[Image smoothing](#image-smoothing) suppresses rapid fluctuations attributed to noise. Linear [heat equation](diffusion-equation.md#heat-equation) [image smoothing](#image-smoothing) attenuates Fourier frequencies by $e^{-t|\xi|^2}$ but also blurs [image edges](#image-edge). Nonlinear filtering uses [image signal](#image-signal) geometry to distinguish fluctuations from meaningful transitions.

##### Median filter

↑ **Parent:** [Image smoothing](#image-smoothing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Median_filter)

A [median filter](#median-filter) replaces an [image signal](#image-signal) value by the [median](probability-theory.md#median) of nearby values. Unlike a linear average, it can reject isolated extreme observations without averaging both sides of an [image edge](#image-edge). The small-radius response depends on neighbourhood geometry and measure; a uniform disk-area [median](probability-theory.md#median) and a circle-boundary [median](probability-theory.md#median) have different time scales.

###### Disk-median curvature expansion

↑ **Parent:** [Median filter](#median-filter)

At a smooth point with nonzero [gradient](calculus.md#gradient), rotate coordinates so $\nabla u=G e_2$. Write $u=u_0+Gy+\tfrac12(Ax^2+2Bxy+Cy^2)+O(|(x,y)|^3)$. A candidate [median](probability-theory.md#median) $u_0+dh^2$ has level boundary $y=(dh^2-Ax^2/2)/G+O(h^3)$ in the disk. The area imbalance is $(2d-A/3)h^3/G+o(h^3)$; equal half-areas force $d=A/6$. Here $A=\Delta u-\nabla u^T(D^2u)\nabla u/|\nabla u|^2$ is the tangential second [derivative](calculus.md#derivative), giving the formula. The disk uses uniform area measure, not its boundary measure.

##### Gaussian blur

↑ **Parent:** [Image smoothing](#image-smoothing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_blur)

[Gaussian blur](#gaussian-blur) applies [convolution](fourier-analysis.md#convolution) with $G_\sigma(x)=(2\pi\sigma^2)^{-n/2}e^{-|x|^2/(2\sigma^2)}$ to an [image signal](#image-signal). It averages over a spatial scale $\sigma$, suppressing rapid variation while also blurring [image edges](#image-edge). The [heat-kernel convolution](diffusion-equation.md#heat-kernel-convolution) realizes this filter at time $t=\sigma^2/2$.

###### Gaussian filtering Fourier multiplier

↑ **Parent:** [Gaussian blur](#gaussian-blur)

The [Fourier transform of a Gaussian](fourier-analysis.md#fourier-transform-of-a-gaussian) and the [convolution theorem](fourier-analysis.md#convolution-theorem) give this multiplier with the angular-frequency convention $e^{-ix\cdot\xi}$. In cycles-per-length [frequencies](physics.md#frequency) $k$, it is $e^{-2\pi^2\sigma^2|k|^2}$. Each coordinate has variance $\sigma^2$, and higher [frequencies](physics.md#frequency) receive stronger attenuation.

### Variational image processing

↑ **Parent:** [Image processing](#image-processing)

A variational model balances agreement with observed data against a regularity or geometric penalty. Examples include [total variation denoising](inverse-problem.md#total-variation-denoising), the [relaxed graph-area functional](inverse-problem.md#relaxed-graph-area-functional), and the [Mumford–Shah functional](#mumford-shah-functional). Convex penalties support unique reconstruction, while segmentation energies can have multiple competing partitions.

<h4 id="mumford-shah-functional">Mumford–Shah functional</h4>

↑ **Parent:** [Variational image processing](#variational-image-processing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mumford–Shah_functional)

The energy $\int_{\Omega\setminus K}(u-g)^2+\alpha\int_{\Omega\setminus K}|\nabla u|^2+\beta\mathcal H^1(K)$ balances data fidelity, within-region smoothness and [image edge](#image-edge) length. In its relaxed [SBV space](inverse-problem.md#special-bounded-variation-space) formulation the [image edge](#image-edge) set is $J_u$. Clipping to the bounded data range, the [SBV compactness theorem](inverse-problem.md#sbv-compactness-theorem) and [lower semicontinuity](calculus.md#lower-semicontinuity) prove existence; the full segmentation problem is not [strictly convex](real-analysis.md#strictly-convex-function).

<h5 id="ambrosio-tortorelli-approximation">Ambrosio–Tortorelli approximation</h5>

↑ **Parent:** [Mumford–Shah functional](#mumford-shah-functional)

The [Mumford–Shah functional](#mumford-shah-functional) can be approximated by an auxiliary edge field $0\le v\le1$ and energy

$$
E_\varepsilon=\int(u-g)^2+\alpha(v^2+\eta_\varepsilon)|\nabla u|^2+\beta\left[\varepsilon|\nabla v|^2+\frac{(1-v)^2}{4\varepsilon}\right],\qquad0<\eta_\varepsilon=o(\varepsilon).
$$

The field is near one inside regions and near zero across an [image edge](#image-edge), weakening smoothing there. The profile $v(s)=1-e^{-|s|/(2\varepsilon)}$ has unit edge energy per unit length in this normalization. The [1990 construction](https://onlinelibrary.wiley.com/doi/10.1002/cpa.3160430805) is a [Gamma-convergence](calculus-of-variations.md#gamma-convergence) approximation; its global-minimizer [limit](calculus.md#limit-of-a-function) does not guarantee global optimality of an alternating numerical solve. Each fixed-field subproblem is quadratic, but the joint energy is nonconvex.

##### Segmentation overfitting without an edge penalty

↑ **Parent:** [Mumford–Shah functional](#mumford-shah-functional)

Removing the jump-length cost from the [Mumford–Shah functional](#mumford-shah-functional) lets finer piecewise-constant partitions reduce squared fidelity without charging for their proliferating [image edges](#image-edge). For [continuous](calculus.md#continuous-function) data on a compact image domain, fine-cell averages converge in squared error while the ordinary within-cell [gradient](calculus.md#gradient) is zero. A finite interface penalty makes that geometry costly.

<h5 id="nonconvexity-of-mumford-shah-segmentation">Nonconvexity of Mumford–Shah segmentation</h5>

↑ **Parent:** [Mumford–Shah functional](#mumford-shah-functional)

On the unit square, let $g=0$ and take $u_0=\chi_{\{x_1>0.4\}}$, $u_1=\chi_{\{x_1>0.6\}}$. Both have one unit-length jump and zero ordinary [gradient](calculus.md#gradient). Their mean has two unit-length jumps. For squared-error coefficient one, $[E(u_0)+E(u_1)]/2=0.5+\beta$ while $E((u_0+u_1)/2)=0.45+2\beta$, violating [convexity](real-analysis.md#convex-function) when $\beta>0.05$. The [Mumford–Shah functional](#mumford-shah-functional) can therefore be nonconvex even though the fixed-edge reconstruction subproblem is [strictly convex](real-analysis.md#strictly-convex-function).

<h5 id="fixed-edge-euler-lagrange-equation-for-mumford-shah">Fixed-edge Euler-Lagrange equation for Mumford–Shah</h5>

↑ **Parent:** [Mumford–Shah functional](#mumford-shah-functional)

For a fixed sufficiently regular [image edge](#image-edge) set, the [Mumford–Shah functional](#mumford-shah-functional) is a [strictly convex](real-analysis.md#strictly-convex-function) quadratic energy on the [Sobolev space](sobolev-space.md) of its complement. A [first variation](calculus-of-variations.md#first-variation) gives $u-\alpha\Delta u=g$ within each region and separate one-sided [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) on free edges. A jump need not vanish across an edge. The weak solution is unique by the [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem); this does not prove uniqueness when the edge set is also optimized.

<h5 id="edge-free-mumford-shah-limit">Edge-free Mumford–Shah limit</h5>

↑ **Parent:** [Mumford–Shah functional](#mumford-shah-functional)

As the jump-length weight tends to infinity with the [gradient](calculus.md#gradient) weight fixed, the limiting problem minimizes $\|u-g\|_2^2+\alpha\|\nabla u\|_2^2$ on $H^1$. It has a unique [minimizer](analysis.md#global-minimizer) by the [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem) and strict convexity. Without prescribed boundary values, its weak equation is $u-\alpha\Delta u=g$ with natural [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition).

<h5 id="piecewise-constant-mumford-shah-problem">Piecewise-constant Mumford–Shah problem</h5>

↑ **Parent:** [Mumford–Shah functional](#mumford-shah-functional)

The infinite gradient-weight limit restricts to [SBV space](inverse-problem.md#special-bounded-variation-space) [image signals](#image-signal) with $\nabla u=0$ almost everywhere. Their energy is fidelity plus jump length, represented by constants on a [Caccioppoli partition](inverse-problem.md#caccioppoli-partition). Internal perimeter is counted once by $\tfrac12\sum_i\operatorname{Per}(E_i;\Omega)$; adjacent equal-valued regions can be merged.

###### Piecewise-constant segmentation contrast threshold

↑ **Parent:** [Piecewise-constant Mumford–Shah problem](#piecewise-constant-mumford-shah-problem)

Suppose two constant data intensities differ by $d$, have areas $a$ and $A-a$, and share an internal boundary of length $L$. Keeping the boundary costs $\beta L$ with zero fidelity; merging the two regions costs $a(A-a)d^2/A$ after fitting their common mean. The displayed inequality makes splitting cheaper among these two candidate geometries. This comparison does not prove either geometry is globally optimal among all partitions.

###### Segmentation interface curvature balance

↑ **Parent:** [Piecewise-constant Mumford–Shah problem](#piecewise-constant-mumford-shah-problem)

When grey values are fixed but region labels vary, a smooth interface satisfies $\beta\kappa=(c_j-g)^2-(c_i-g)^2$. The [curvature](differential-geometry.md#curvature) uses the normal pointing out of region $i$, positive on an outward-oriented circle. It balances the change in data cost against the first variation of interface length. Fixing a full spatial [image signal](#image-signal) instead fixes its jumps and leaves no such boundary-relocation freedom.

###### Triple-junction angle in isotropic segmentation

↑ **Parent:** [Segmentation interface curvature balance](#segmentation-interface-curvature-balance)

At a freely moving regular junction of three smooth [image edges](#image-edge) with equal isotropic length weights, the endpoint [first variation](calculus-of-variations.md#first-variation) requires the sum of their outward unit tangent vectors to vanish. Three unit vectors with zero sum have pairwise angles of $120$ degrees. Different interface weights instead give a weighted force balance, and constrained or singular junctions require separate hypotheses.

###### Region means in piecewise-constant segmentation

↑ **Parent:** [Piecewise-constant Mumford–Shah problem](#piecewise-constant-mumford-shah-problem)

For a fixed positive-area region $E_i$, its least-squares grey value is $c_i=|E_i|^{-1}\int_{E_i}g$. The minimum fidelity equals $\int g^2-\sum_i(\int_{E_i}g)^2/|E_i|$. This eliminates the grey values before optimizing the partition geometry.

<h5 id="essential-closedness-of-mumford-shah-jump-sets">Essential closedness of Mumford–Shah jump sets</h5>

↑ **Parent:** [Mumford–Shah functional](#mumford-shah-functional)

A [minimizer](analysis.md#global-minimizer) of the [Mumford–Shah functional](#mumford-shah-functional) with bounded [image signal](#image-signal) data has an essentially closed jump set: replacing $J_u$ by its relative closure adds no $(n-1)$-dimensional [measure](measure-theory.md#measure). Its complement supports a Sobolev representative. This regularity theorem connects a relaxed [SBV space](inverse-problem.md#special-bounded-variation-space) [minimizer](analysis.md#global-minimizer) to the classical closed-edge formulation; it is not a property of every special bounded-variation function.

## Cryptography

↑ **Parent:** [Computer science](computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cryptography)

The design and analysis of protocols that protect information or authenticate messages in the presence of adversaries. It includes [ciphers](coding-theory.md#cipher), [digital signatures](#digital-signature) and [cryptographic hash functions](#cryptographic-hash-function).

### One-way function

↑ **Parent:** [Cryptography](#cryptography)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/One-way_function)

A [one-way function](#one-way-function) is efficiently computable but computationally infeasible to invert on a randomly sampled input with nonnegligible success probability, under its stated security assumption. An [RSA cryptosystem](algebra.md#rsa-cryptosystem) supplies the candidate map $x\mapsto x^e\bmod N$ on units modulo $N$. Inversion hardness is an assumption; it is not a proved consequence of merely choosing large primes.

#### One-way permutation

↑ **Parent:** [One-way function](#one-way-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/One-way_permutation)

A [one-way permutation](#one-way-permutation) is a bijective [one-way function](#one-way-function) on its input domain. Injectivity is useful for binding in [bit commitment](#bit-commitment), because an output has only one possible preimage even if a dishonest sender has unlimited computation.

### Hard-core predicate

↑ **Parent:** [Cryptography](#cryptography)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hard-core_predicate)

A [hard-core predicate](#hard-core-predicate) is an efficiently computable bit of an input to a [one-way function](#one-way-function) that cannot be predicted from the function output with nonnegligible advantage over random guessing. For a [one-way function](#one-way-function) $f$, padding it to $F(x,r)=(f(x),r)$ gives the inner-product predicate $h(x,r)=\sum_jx_jr_j\bmod2$. This is the Goldreich–Levin construction. It provides a way to mask a bit using an otherwise publicly revealed [one-way function](#one-way-function) value.

### Bit commitment

↑ **Parent:** [Cryptography](#cryptography)

A bit commitment allows a sender to fix a bit while concealing it from the receiver until an opening phase. Binding prevents a sender from opening the same commitment as either bit; hiding prevents the receiver from learning the bit prematurely. With a [one-way permutation](#one-way-permutation) $F$ and a [hard-core predicate](#hard-core-predicate) $h$, a commitment can consist of $F(x)$ and the masked bit $b\mathbin{\oplus}h(x)$. Opening reveals $x$. Injectivity gives binding, while unpredictability of the [hard-core predicate](#hard-core-predicate) gives computational hiding. For an [RSA cryptosystem](algebra.md#rsa-cryptosystem), the receiver must not possess the inverse trapdoor.

#### Ensemble-steering attack on quantum bit commitment

↑ **Parent:** [Bit commitment](#bit-commitment)

If the two honest [quantum state ensembles](quantum-theory.md#quantum-state-ensemble) have the same [density operator](quantum-theory.md#density-matrix), their independently prepared blocks are perfectly hiding. A dishonest sender can instead send one half of a [purification of a density operator](quantum-theory.md#purification-of-a-density-operator) and retain the other. The [Hughston–Jozsa–Wootters theorem](quantum-theory.md#hughston-jozsa-wootters-theorem) allows a measurement of the retained system to prepare either honest ensemble after commitment. If verification checks only the declared states, either opening is then accepted with the honest probabilities. This gives a concrete failure of binding while preserving perfect hiding.

### Quantum key distribution

↑ **Parent:** [Cryptography](#cryptography)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_key_distribution)

Quantum key distribution uses a quantum channel and an authenticated public classical channel to establish matching random keys for two parties while limiting an eavesdropper's information. The public transcript is included in the adversary's information. In an ideal successful protocol, a key of length $\ell$ is uniform and independent of that information. Actual protocols allow small disagreement and secrecy errors and may abort. [Measurement in quantum mechanics](quantum-measurement.md) disturbance provides parameter tests, while [privacy amplification](#privacy-amplification) removes residual knowledge after classical reconciliation. The [BB84 protocol](quantum-theory.md#bb84) and entanglement-based protocols are examples.

#### Premature basis announcement in quantum key distribution

↑ **Parent:** [Quantum key distribution](#quantum-key-distribution)

If basis information and test positions are announced before the receiver confirms receipt of quantum carriers, an eavesdropper can store the carriers until learning that information. In a scheme sending one half of each [Bell pair](bell-state.md#bell-pair) after a [Hadamard gate](quantum-theory.md#hadamard-gate) encoding, the eavesdropper then forwards test qubits untouched and measures all data qubits in their now-known correct bases. Every test passes, while data are changed to classically correlated [product states](bell-state.md#product-state) whose bit labels the eavesdropper knows. This invalidates the sampling argument needed to justify [entanglement purification](bell-state.md#entanglement-distillation) and [quantum key distribution](#quantum-key-distribution). A sound additional purification certification could detect this attack and abort; it cannot generate private [Bell pairs](bell-state.md#bell-pair) from the separable attacked data. Announcing bases only after receipt prevents this particular delayed-carrier attack.

### Coin flipping by telephone

↑ **Parent:** [Cryptography](#cryptography)

A protocol for two distant parties to agree on a random bit without trusting either party to announce an unverified coin toss. In the [Rabin-Williams scheme](coding-theory.md#rabin-cryptosystem), a publicly committed square hides which of two half-interval roots the sender selected. The other party guesses a digit distinguishing those roots; subsequent root and factor revelations verify the completed exchange. The protocol's fairness relies on prescribed randomness and the difficulty of finding a second root; it does not force a party to complete communication.

### Privacy amplification

↑ **Parent:** [Cryptography](#cryptography)

[Privacy amplification](#privacy-amplification) compresses a partially secret random string into a shorter key by a publicly selected hash function, reducing an adversary's information about the final key. In the [BB84 protocol](quantum-theory.md#bb84) it follows parameter estimation and error correction, and accounts for information leaked in the public reconciliation transcript. Authentication of the public channel remains necessary.

### Message authentication

↑ **Parent:** [Cryptography](#cryptography)

Assurance of the source and integrity of a message against specified adversarial capabilities. [Digital signatures](#digital-signature) permit public verification, whereas a [message authentication](#message-authentication) code uses a shared secret; [encryption](#encryption) alone need not authenticate.

#### Message authentication code

↑ **Parent:** [Message authentication](#message-authentication)

A keyed function producing a tag that a holder of the shared secret can verify. Its [message authentication](#message-authentication) security requires that valid tags for new messages cannot be forged under the allowed adversarial queries. Unlike a [digital signature](#digital-signature), verification is not inherently public and the verifier also knows a key capable of making tags.

<h5 id="wegman-carter-authentication">Wegman–Carter authentication</h5>

↑ **Parent:** [Message authentication code](#message-authentication-code)

Combine a secret randomly selected [almost strongly universal hash family](#almost-strongly-universal-hash-family) member with a fresh secret output mask. An observed [message authentication code](#message-authentication-code) tag leaves the hash-selection key hidden, and the conditional hash bound controls substitution forgery probability. The message itself need not be encrypted. Mask reuse can reveal hash differences; repeated-use guarantees require fresh masks and an appropriate analysis of verification information. A one-use polynomial construction needs only two secret field elements, even for a much longer message.

### Cryptographic nonce

↑ **Parent:** [Cryptography](#cryptography)

A protocol value intended to be used only once under a specified key. In the [ElGamal signature scheme](#elgamal-signature-scheme) the signing nonce must also be secret and invertible modulo the group order; mere distinctness does not imply unpredictability.

### Public-key cryptography

↑ **Parent:** [Cryptography](#cryptography)

[Cryptography](#cryptography) using a [public key](#public-key) and a corresponding [private key](#private-key). Public-key [encryption](#encryption) lets others encrypt for the private-key holder; a [digital signature](#digital-signature) instead lets the holder authenticate messages for public verification.

#### Public key

↑ **Parent:** [Public-key cryptography](#public-key-cryptography)

The published member of a public-key cryptographic key pair. Its association with a particular identity must itself be authenticated; mere knowledge of a purported [public key](#public-key) does not establish that identity.

#### Private key

↑ **Parent:** [Public-key cryptography](#public-key-cryptography)

The secret member of a public-key cryptographic key pair, used for decryption or signing according to the scheme. In the [RSA cryptosystem](algebra.md#rsa-cryptosystem) the private exponent is not interchangeable with a security proof for textbook signing.

### Encryption

↑ **Parent:** [Cryptography](#cryptography)

The transformation of a message into a ciphertext using a key, with decryption recovering the message using an appropriate key. Confidentiality and [message authentication](#message-authentication) are separate properties; an [encryption](#encryption) scheme needs explicit security hypotheses.

### Chosen-ciphertext attack

↑ **Parent:** [Cryptography](#cryptography)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chosen-ciphertext_attack)

An attack in which an adversary obtains decryptions of selected ciphertexts, subject to the protocol’s restrictions. The multiplicative structure of textbook [RSA cryptosystem](algebra.md#rsa-cryptosystem) permits blinding an intercepted ciphertext by a known invertible factor.

### Cryptographic hash function

↑ **Parent:** [Cryptography](#cryptography)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cryptographic_hash_function)

A function mapping messages of arbitrary length to fixed-length digests, designed to provide [preimage resistance](#preimage-resistance) and [collision resistance](#collision-resistance). In a [digital signature](#digital-signature) protocol the digest also needs an encoding and security properties appropriate to that protocol.

#### Collision resistance

↑ **Parent:** [Cryptographic hash function](#cryptographic-hash-function)

Finding any distinct messages with equal cryptographic hash values should be computationally infeasible under the specified security model. A collision can let a signed digest authenticate an unintended message.

#### Preimage resistance

↑ **Parent:** [Cryptographic hash function](#cryptographic-hash-function)

Given a target digest h, finding a message m with H(m)=h should be computationally infeasible under the specified security model. This is distinct from finding two messages with equal digests.

### Digital signature

↑ **Parent:** [Cryptography](#cryptography)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Digital_signature)

A public-verification [message authentication](#message-authentication) scheme with key generation, signing using a [private key](#private-key), and verification using the corresponding [public key](#public-key). Signing an appropriate digest binds the signature to the message; [encryption](#encryption) alone does not provide this authenticity.

#### ElGamal signature scheme

↑ **Parent:** [Digital signature](#digital-signature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/ElGamal_signature_scheme)

For a [prime number](number-theory.md#prime-number) $p$, [primitive root](number-theory.md#primitive-root-modulo-n) $g$ and [public key](#public-key) $y=g^a$, choose a fresh secret $k$ [coprime](number-theory.md#coprime-integers) to $p-1$, set $r=g^k\pmod p$ and $s=k^{-1}(H(m)-ar)\pmod{p-1}$, and verify $g^{H(m)}=y^r r^s\pmod p$. Reusing the [cryptographic nonce](#cryptographic-nonce) can reveal secret information. The unhashed historical construction allows existential forgery of specially chosen message exponents, so authentication claims require suitable hashing and protocol assumptions.

#### RSA signature

↑ **Parent:** [Digital signature](#digital-signature)

A signature based on private [RSA cryptosystem](algebra.md#rsa-cryptosystem) exponentiation, with public exponentiation used for verification. Textbook $s=m^d\pmod N$ is multiplicatively forgeable; a secure scheme requires an appropriate encoding and message digest rather than raw message exponentiation.

## Algorithm

↑ **Parent:** [Computer science](computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algorithm)

An algorithm is a finite, precise procedure for transforming an [input](#input-computer-science) into an [output](#output-computing).

### Strength reduction

↑ **Parent:** [Algorithm](#algorithm)

Replace an operation by an equivalent operation sequence with lower cost on the target machine. For fixed-width wrapping integers, multiplication by eight equals left shift by three, and multiplication by fifteen equals left shift by four minus the original operand. Condition codes and wider results must also be preserved if the original machine instruction exposes them.

// Destination: computer-science.bigb

### Statistical program profiling

↑ **Parent:** [Algorithm](#algorithm)

Periodically sample an executing program's [instruction pointer](#instruction-pointer) and accumulate an address histogram. Samples approximate time spent in address regions, rather than exact instruction execution counts. Jittering the sampling interval reduces accidental synchronization with periodic code.

// Destination: computer-science.bigb

### Depth-first search

↑ **Parent:** [Algorithm](#algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Depth-first_search)

// Target: computer-science.bigb

### Memoization

↑ **Parent:** [Algorithm](#algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Memoization)

// Target: computer-science.bigb

### Merge sort

↑ **Parent:** [Algorithm](#algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Merge_sort)

// Target: computer-science.bigb

### Merge algorithm

↑ **Parent:** [Algorithm](#algorithm)

Merges two sorted sequences by repeatedly choosing their smaller remaining head. With constant-time comparisons it uses at most $m+n-1$ comparisons for nonempty inputs.

// Target: computer-science.bigb

### Binary search

↑ **Parent:** [Algorithm](#algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_search)

Binary search identifies a position in an ordered list by repeatedly comparing with a middle entry and keeping the appropriate half. For $N$ possible positions, this requires at most $\lceil\log_2N\rceil$ comparisons. The interval of remaining positions is an invariant of the [algorithm](#algorithm): every answer removes only positions incompatible with the comparison. A [decision tree](#decision-tree) with $q$ binary answers has at most $2^q$ leaves, explaining the logarithmic lower bound.

### Karatsuba multiplication

↑ **Parent:** [Algorithm](#algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Karatsuba_multiplication)

Karatsuba multiplication multiplies two $n$-digit integers using three, rather than four, multiplications of roughly half-size. Its recurrence $T(n)=3T(n/2)+O(n)$ gives $T(n)=O(n^{\log_2 3})$.

### Randomized algorithm

↑ **Parent:** [Algorithm](#algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Randomized_algorithm)

A randomized algorithm makes some choices using random bits.

#### Derandomization

↑ **Parent:** [Randomized algorithm](#randomized-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Derandomization)

Derandomization converts a randomized construction or algorithm into a deterministic one while preserving its desired guarantee. The [method of conditional probabilities](#method-of-conditional-probabilities) does this by maintaining a computable [conditional expectation](measure-theory.md#conditional-expectation) until all choices are fixed.

##### Method of conditional probabilities

↑ **Parent:** [Derandomization](#derandomization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Method_of_conditional_probabilities)

For a random objective with an easily computable [conditional expectation](measure-theory.md#conditional-expectation), reveal one random choice at a time and choose an outcome whose conditional expected objective is at least the current value. Such an outcome exists because the current value is an average of the child values. When all choices are fixed, the actual objective is at least the initial expectation. Biased as well as fair choices work. Efficient expectation updates make the resulting deterministic procedure a [polynomial-time algorithm](#polynomial-time-algorithm).

#### Probabilistic Turing machine

↑ **Parent:** [Randomized algorithm](#randomized-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Probabilistic_Turing_machine)

A probabilistic Turing machine is a [Turing machine](#turing-machine) whose transitions may depend on independent random bits.

#### One-sided error

↑ **Parent:** [Randomized algorithm](#randomized-algorithm)

A randomized decision algorithm has one-sided error when one answer is always correct and only the other answer can be mistaken.

##### RP (complexity)

↑ **Parent:** [One-sided error](#one-sided-error)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/RP_(complexity))

$\mathbf{RP}$ contains decision problems with a polynomial-time randomized algorithm that rejects every negative instance and accepts every positive instance with probability at least one half.

##### co-RP

↑ **Parent:** [One-sided error](#one-sided-error)

$\mathbf{co\text{-}RP}$ consists of complements of languages in [RP](#rp-complexity). Its algorithms always accept positive instances and reject negative instances with probability at least one half.

#### ZPP

↑ **Parent:** [Randomized algorithm](#randomized-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/ZPP)

$\mathbf{ZPP}=\mathbf{RP}\cap\mathbf{co\text{-}RP}$. Equivalently, it consists of problems having an always-correct randomized algorithm with polynomial expected running time.

#### Error reduction for a randomized algorithm

↑ **Parent:** [Randomized algorithm](#randomized-algorithm)

Independent repetitions reduce a randomized algorithm's error probability while preserving polynomial running time.

#### Polynomial identity testing

↑ **Parent:** [Randomized algorithm](#randomized-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_identity_testing)

Polynomial identity testing asks whether a polynomial represented implicitly, such as by an arithmetic circuit or a remainder computation, is the zero polynomial.

## Theoretical computer science

↑ **Parent:** [Computer science](computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Theoretical_computer_science)

### Formal language

↑ **Parent:** [Theoretical computer science](#theoretical-computer-science)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Formal_language)

A formal language is a set of finite strings over a fixed finite alphabet.

#### Binary string

↑ **Parent:** [Formal language](#formal-language)

A [binary string](#binary-string) is a finite word over the alphabet $\{0,1\}$. There are $2^n$ strings of length $n$. Finite [binary strings](#binary-string) have an effective [bijection](function.md#bijection) with [natural numbers](arithmetic.md#natural-number), so computable enumerability and immunity apply to sets of strings.

##### Counting binary strings with bounded ones

↑ **Parent:** [Binary string](#binary-string)

A [binary string](#binary-string) with $n$ zeroes and $j$ ones is determined by its $j$ one-positions, giving $\binom{n+j}j$ possibilities. Sum for $0\le j\le m$ and apply the [hockey-stick identity](combinatorics.md#hockey-stick-identity). Equivalently, distribute at most $m$ ones among the $n+1$ gaps around the zeroes and add a slack count; [stars and bars](combinatorics.md#stars-and-bars-combinatorics) counts $n+2$ nonnegative counts summing to $m$.

##### Self-delimiting binary code

↑ **Parent:** [Binary string](#binary-string)

A self-delimiting code permits a decoder to identify the end of a code without an external length marker. Encoding a binary word of length $\ell$ by $\ell$ ones, a zero and the word uses $2\ell+1$ bits. This yields an $O(\log n)$ description of a [natural number](arithmetic.md#natural-number) in an incompressibility proof.

#### Concatenation of formal languages

↑ **Parent:** [Formal language](#formal-language)

For [formal languages](#formal-language) $L,M$ over the same [alphabet](information-theory.md#alphabet), concatenate each [word over an alphabet](foundations-of-mathematics.md#string) in $L$ with each [word over an alphabet](foundations-of-mathematics.md#string) in $M$. This operation is associative, has identity $\{\varepsilon\}$ and absorbing element the [empty language](#empty-language).

#### Empty language

↑ **Parent:** [Formal language](#formal-language)

The [formal language](#formal-language) containing no [words over an alphabet](foundations-of-mathematics.md#string). It differs from the language containing only the [empty word](foundations-of-mathematics.md#empty-word), which is a multiplicative identity for [concatenation of formal languages](#concatenation-of-formal-languages).

### Turing machine

↑ **Parent:** [Theoretical computer science](#theoretical-computer-science)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Turing_machine)

A Turing machine is an abstract computational model with a finite control, an unbounded tape and a head that reads, writes and moves on the tape.

#### Instantaneous description of a Turing machine

↑ **Parent:** [Turing machine](#turing-machine)

An instantaneous description records the current control state, head position, and tape contents. For a tape blank outside a finite window, a word $h\,u\,q\,v\,h$ records the symbols $u$ to the left of the head and $v$ from the scanned cell rightward, with unrecorded cells blank. If $v$ is empty, the head scans an implicit blank. Extra outer blanks can represent the same infinite tape. The [instruction of a Turing machine](#instruction-of-a-turing-machine) determines its successor description.

#### Instruction of a Turing machine

↑ **Parent:** [Turing machine](#turing-machine)

For a deterministic single-tape [Turing machine](#turing-machine), an instruction reads a state $q$ and scanned tape symbol $a$, writes $b$, changes state to $p$, and moves the head one cell left, one cell right, or not at all according to $D$. The state and tape alphabets are finite; an undefined transition halts. A dedicated terminal state can be introduced by directing undefined transitions to it without changing whether computation halts.

#### Two-stack encoding of a Turing tape

↑ **Parent:** [Turing machine](#turing-machine)

Encode the cells immediately left of the head in a reversed positional stack $L$, and the current and right cells in $R$. Quotient and remainder by the alphabet base read and remove cells; multiplication by that base pushes a cell. The resulting local tape transitions are [primitive recursive](foundations-of-mathematics.md#primitive-recursive-function), which makes them directly implementable on [Church numerals](foundations-of-mathematics.md#church-numeral).

#### Modular machine

↑ **Parent:** [Turing machine](#turing-machine)

A modular machine of modulus $m>1$ acts on pairs in $\mathbb N^2$. Each instruction $(a,b,c,R)$ or $(a,b,c,L)$ has $0\le a,b<m$ and $0\le c<m^2$, and at most one instruction is assigned to each residue pair $(a,b)$. The two transition types are $(mu+a,mv+b)\mapsto(m^2u+c,v)$ and $(mu+a,mv+b)\mapsto(u,m^2v+c)$. These finite arithmetic operations can encode a [Turing machine](#turing-machine); a designated terminal configuration can have a nonrecursive [halting set](foundations-of-mathematics.md#halting-set).

##### Group encoding of a modular machine

↑ **Parent:** [Modular machine](#modular-machine)

A [modular machine](#modular-machine) can be encoded by [HNN extensions](geometric-group-theory.md#hnn-extension) of $K=\mathbb Z^2*\langle t\rangle$. The kernel of $K\to\mathbb Z^2$ has a [free basis of a group](geometric-group-theory.md#free-basis-of-a-group) $t(r,s)=x^{-r}y^{-s}tx^ry^s$. Associated-subgroup maps send these basis elements according to the two arithmetic transition types. In the resulting group, membership of $t(r,s)$ in the subgroup generated by $t$ and the instruction stable letters is equivalent to $(r,s)\in H_0(\mathcal M)$. One more [HNN extension](geometric-group-theory.md#hnn-extension) centralizes that finitely generated subgroup, converting membership to equality and hence to the [word problem for a group](geometric-group-theory.md#word-problem-for-groups).

##### Halting set at a designated terminal configuration

↑ **Parent:** [Modular machine](#modular-machine)

For a [modular machine](#modular-machine) whose $(0,0)$ is terminal, $H_0(\mathcal M)$ is the set of configurations whose forward computation reaches exactly $(0,0)$, including the zero-step computation there. It may differ from the set of configurations stopping at any terminal configuration. Determinism makes membership invariant along each instruction edge.

#### Deterministic computation

↑ **Parent:** [Turing machine](#turing-machine)

In a deterministic computation, every configuration and input symbol determine at most one next configuration.

#### Reversible computation

↑ **Parent:** [Turing machine](#turing-machine)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reversible_computation)

A reversible computation has an injective transition function, so its preceding configuration can be recovered from its current configuration. Any finite classical computation can be simulated reversibly while retaining enough workspace to [uncompute](quantum-theory.md#uncomputation) its temporary results.

##### Reversible circuit

↑ **Parent:** [Reversible computation](#reversible-computation)

A reversible circuit is composed of bijective gates. The [Toffoli gate](quantum-theory.md#toffoli-gate) is universal for reversible Boolean computation when ancillary bits are available.

#### Nondeterministic Turing machine

↑ **Parent:** [Turing machine](#turing-machine)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nondeterministic_Turing_machine)

A nondeterministic computation may have several possible next configurations and accepts when at least one computation path accepts.

#### Oracle machine

↑ **Parent:** [Turing machine](#turing-machine)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Oracle_machine)

An oracle machine may query membership in a fixed language in one computation step.

##### Relativization (complexity theory)

↑ **Parent:** [Oracle machine](#oracle-machine)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Relativization_(complexity_theory))

A relativized complexity class $\mathcal C^A$ allows every machine defining $\mathcal C$ to query the same oracle $A$.

### Boolean operation

↑ **Parent:** [Theoretical computer science](#theoretical-computer-science)

A Boolean operation maps one or more bits to a bit and supplies the concrete operations used to interpret a [Boolean algebra](mathematical-logic.md#boolean-algebra).

#### Exclusive or

↑ **Parent:** [Boolean operation](#boolean-operation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exclusive_or)

Exclusive or returns one exactly when its two input bits differ. It is addition modulo two and is written $x\mathbin\oplus y$.

#### Negation

↑ **Parent:** [Boolean operation](#boolean-operation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Negation)

Logical negation exchanges zero and one.

<h4 id="de-morgan-s-laws">De Morgan's laws</h4>

↑ **Parent:** [Boolean operation](#boolean-operation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/De_Morgan's_laws)

De Morgan's laws state

$$
\neg(P\wedge Q)=(\neg P)\vee(\neg Q),
\qquad
\neg(P\vee Q)=(\neg P)\wedge(\neg Q).
$$

### Computational complexity theory

↑ **Parent:** [Theoretical computer science](#theoretical-computer-science)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Computational_complexity_theory)

Computational complexity theory classifies [computational problems](#computational-problem) by the resources needed to solve them.

#### Communication complexity

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Communication_complexity)

Communication complexity studies how much information distributed parties must exchange to compute a function of their separately held inputs. Local computation is free; the resource being counted is communicated bits or qubits, with the allowed shared randomness, [quantum entanglement](bell-state.md#entangled-state) or other correlations specified separately. For a [Boolean function](combinatorics.md#boolean-function) $f(x,y)$, a one-way exact protocol has the receiver output $f$ correctly for every input after a single message. [One-bit computation using Popescu–Rohrlich boxes](quantum-theory.md#one-bit-computation-using-popescu-rohrlich-boxes) shows that this resource measure changes drastically if ideal superquantum boxes are available.

#### Promise problem

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)

A [promise problem](#promise-problem) consists of disjoint sets of YES and NO instances. An algorithm or verifier must obey its correctness guarantees only on their union. Energy problems with separated thresholds are naturally [promise problems](#promise-problem) because intermediate-energy instances require no prescribed answer.

#### Quantum complexity theory

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_complexity_theory)

Quantum complexity theory studies resources needed by [quantum circuits](quantum-circuit.md) and quantum algorithms, including time, workspace, and [quantum query complexity](#quantum-query-complexity). Its models specify which input oracles and gate implementations are available; counting oracle calls is different from counting all elementary gates.

##### BQP

↑ **Parent:** [Quantum complexity theory](#quantum-complexity-theory)

[BQP](#bqp) is the class of [promise problems](#promise-problem) decided by uniform polynomial-size [quantum circuits](quantum-circuit.md) with bounded error. Completeness $2/3$ and soundness $1/3$ are conventional; [BQP error reduction](#bqp-error-reduction) shows that other fixed separated thresholds give the same class.

###### BQP error reduction

↑ **Parent:** [BQP](#bqp)

Independent runs of a [BQP](#bqp) algorithm with fresh [ancilla qubits](quantum-information-theory.md#ancilla-qubit) can be combined by a classical threshold rule. If completeness exceeds soundness by $\gamma$, a [Hoeffding inequality](probability-inequality.md#hoeffding-inequality) bounds the error after $r$ runs by $e^{-r\gamma^2/2}$. Polynomial repetition handles inverse-polynomial gaps. This does not automatically preserve the restricted gate and measurement rules of a [stoquastic circuit](quantum-circuit.md#stoquastic-circuit).

##### Quantum witness

↑ **Parent:** [Quantum complexity theory](#quantum-complexity-theory)

A [quantum witness](#quantum-witness) is a polynomial-size [quantum state](quantum-mechanics.md#quantum-state) supplied to a verifier as evidence for a YES instance. The verifier fixes its own [ancilla qubits](quantum-information-theory.md#ancilla-qubit) independently. Pure [quantum witnesses](#quantum-witness) suffice when maximizing a linear acceptance functional on [density operators](quantum-theory.md#density-matrix). [Quantum witnesses](#quantum-witness) are not generally restricted to basis vectors or product states.

##### StoqMA

↑ **Parent:** [Quantum complexity theory](#quantum-complexity-theory)

[StoqMA](#stoqma) is a restricted quantum-verifier class using [stoquastic circuits](quantum-circuit.md#stoquastic-circuit) and polynomial-size [quantum witnesses](#quantum-witness). A YES instance has a [quantum witness](#quantum-witness) accepted with probability at least $a$; on a NO instance every [quantum witness](#quantum-witness) has acceptance at most $b$, with an inverse-polynomial gap $a-b$. An optimal [quantum witness](#quantum-witness) can be chosen with nonnegative amplitudes, since the [witness acceptance operator](#witness-acceptance-operator) is entrywise nonnegative. The [quantum witness](#quantum-witness) is generally a superposition, rather than a [computational basis](quantum-theory.md#computational-basis) vector. The [stoquastic acceptance floor](quantum-circuit.md#stoquastic-acceptance-floor) explains the lower limit $b\geq1/2$ for a nontrivial soundness promise.

##### QMA

↑ **Parent:** [Quantum complexity theory](#quantum-complexity-theory)

[QMA](#qma) is the class of [promise problems](#promise-problem) with a polynomial-size quantum witness checked by a uniform polynomial-size [quantum circuit](quantum-circuit.md). YES instances have an accepting witness with probability at least $2/3$; NO instances have acceptance at most $1/3$ for every witness, including mixed states. The verifier's acceptance is linear in the witness [density operator](quantum-theory.md#density-matrix). Inverse-polynomial or exponentially small error can be obtained through [QMA error reduction](#qma-error-reduction).

###### Witness acceptance operator

↑ **Parent:** [QMA](#qma)

For [quantum witness](#quantum-witness) embedding $J$, verifier unitary $U$ and accepting projector $\Pi$, the [witness acceptance operator](#witness-acceptance-operator) is the positive contraction $F=J^\dagger U^\dagger\Pi UJ$. The maximum acceptance over normalized [quantum witnesses](#quantum-witness) is $\lambda_{\max}(F)$ by the [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient). Restricting to basis [quantum witnesses](#quantum-witness) only tests its diagonal entries and need not find that maximum.

###### Trace-power witness optimization

↑ **Parent:** [Witness acceptance operator](#witness-acceptance-operator)

For a positive [witness acceptance operator](#witness-acceptance-operator) on dimension $D$, large trace powers approximate its largest [eigenvalue](linear-operator-theory.md#eigenvalue). With an $m$-qubit [QMA](#qma) [quantum witness](#quantum-witness) and $d=2m+2$, the usual NO instances give $\operatorname{Tr}(F^d)<2^{-d}$ and YES instances give a value above $2^{-d}$. A closed product-index expansion computes the trace by recomputation with polynomial storage, avoiding logarithms and roots in a real-arithmetic implementation.

###### QMA error reduction

↑ **Parent:** [QMA](#qma)

Starting from completeness $2/3$ and soundness $1/3$, run an odd number $r$ of parallel copies and take majority. The [QMA parallel repetition with entangled witnesses](#qma-parallel-repetition-with-entangled-witnesses) argument proves soundness for arbitrary repeated witnesses. Exponential [Markov's inequality](probability-inequality.md#markov-inequality) gives majority error at most $(2\sqrt2/3)^r$. Hence $O(\log(1/\epsilon))$ copies suffice for error $\epsilon$, with polynomial overhead when the target error is inverse-polynomial or exponentially small in input length.

###### QMA parallel repetition with entangled witnesses

↑ **Parent:** [QMA](#qma)

Independent verifier circuits on $r$ witness registers induce a threshold acceptance effect built from tensor products of $M$ and $I-M$, where $M$ is the [quantum verifier acceptance operator](#quantum-verifier-acceptance-operator). In a product eigenbasis of $M$, the effect's [eigenvalues](linear-operator-theory.md#eigenvalue) are threshold probabilities for independent [Bernoulli random variables](discrete-probability-distribution.md#bernoulli-distribution) with parameters given by the selected eigenvalues of $M$. Bounding every parameter on a NO instance bounds the effect's [operator norm](continuous-dual-space.md#operator-norm), even if the actual submitted witness is entangled. Independence is used only for the spectral calculation, not assumed for the witness.

###### Quantum verifier acceptance operator

↑ **Parent:** [QMA](#qma)

A verifier with clean ancillas and a designated output measurement induces an effect $0\leq M\leq I$ on the witness register. Its acceptance probability is $\operatorname{Tr}(M\rho)$, and the largest possible acceptance is $\|M\|$. Spectral bounds on $M$ make the soundness quantifier over all witnesses, including entangled repeated witnesses, explicit.

##### Quantum query complexity

↑ **Parent:** [Quantum complexity theory](#quantum-complexity-theory)

The quantum query complexity of a task counts uses of an input oracle by a [quantum circuit](quantum-circuit.md), for a specified success probability. Known gates and workspace operations are not counted as oracle queries, although they contribute to the circuit's full runtime. An efficient query bound therefore need not, by itself, be an efficient gate bound.

###### Polynomial method for quantum query lower bounds

↑ **Parent:** [Quantum query complexity](#quantum-query-complexity)

After $T$ input-bit queries, every [probability amplitude](quantum-mechanics.md#probability-amplitude) is a [polynomial](polynomial.md) of degree at most $T$, because the bit-query matrix entries are affine in the input bits. An acceptance [probability](probability-theory.md#probability) is a sum of squared absolute amplitudes and has [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $2T$. [Multilinear reduction on the Boolean cube](polynomial.md#multilinear-reduction-on-the-boolean-cube) does not increase degree. Exact acceptance therefore implies $Q_E(f)\ge\lceil\deg(f)/2\rceil$. For bounded error the acceptance polynomial only approximates the [Boolean function](combinatorics.md#boolean-function); its exact representing degree is not the relevant bound.

###### Exact quantum query complexity

↑ **Parent:** [Quantum query complexity](#quantum-query-complexity)

The least worst-case number of input-oracle calls made by a [quantum circuit](quantum-circuit.md) that computes a [Boolean function](combinatorics.md#boolean-function) with zero error on every input. Known [unitary gates](quantum-circuit.md#quantum-logic-gate) and classical processing do not count toward this quantity; their runtime is a separate cost.

###### Exact two-query majority algorithm

↑ **Parent:** [Exact quantum query complexity](#exact-quantum-query-complexity)

One exact parity query determines whether the first two bits agree. If they agree, a second query reads one of them; otherwise it reads the third bit. Those values respectively determine the three-bit [majority function](#majority-function). The matching lower bound follows from its degree-three [multilinear polynomial](polynomial.md#multilinear-polynomial).

###### Quantum collision finding

↑ **Parent:** [Quantum query complexity](#quantum-query-complexity)

Given a [function](function.md) $f$ with an $m$-bit output, accessed through the [unitary operator](vector-space.md#unitary-operator) $U_f|x\rangle|y\rangle=|x\rangle|y\mathbin\oplus f(x)\rangle$, quantum collision finding asks for distinct inputs with equal outputs. Here $\oplus$ is bitwise [exclusive or](#exclusive-or) on the $m$-bit answer [quantum register](quantum-circuit.md#quantum-register). The distinctness requirement excludes the uninformative pair $(x,x)$. For a two-to-one function on $N$ inputs, [Grover search algorithm](quantum-theory.md#grover-s-algorithm) methods yield a cube-root [quantum query complexity](#quantum-query-complexity), despite a square-root cost for finding a partner of just one preselected input.

<h6 id="brassard-hoyer-tapp-collision-algorithm">Brassard–Høyer–Tapp collision algorithm</h6>

↑ **Parent:** [Quantum collision finding](#quantum-collision-finding)

Query a known set of $m$ inputs and store its output table. If no [function collision](function.md#function-collision) occurs there, each of its $m$ distinct outputs has exactly one partner in the complement, for a two-to-one function. A [compute-phase-uncompute construction](quantum-theory.md#compute-phase-uncompute-construction) marks those partners using two function queries and reversible table comparison. [Known-subset Grover search](quantum-theory.md#known-subset-grover-search) then uses $O(\sqrt{(N-m)/m})$ such phase queries. Including table preparation and a final verification query gives

$$
T(m)=m+O\!\left(\sqrt{\frac{N-m}{m}}\right)+1.
$$

Choosing $m\asymp N^{1/3}$ balances both terms and gives $T(m)=O(N^{1/3})$. The [Grover rotation angle](quantum-theory.md#grover-rotation-angle) rounding bound gives success tending to one. This is a query bound; it does not make reversible table lookup free in a gate or physical-memory cost model.

#### Decision tree model

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Decision_tree_model)

The decision tree model computes a function by adaptively querying input coordinates.

##### Decision tree

↑ **Parent:** [Decision tree model](#decision-tree-model)

A decision tree adaptively reveals input coordinates until their observed values determine the output. Its revealment for a coordinate is the probability that the coordinate is inspected.

###### Decision-tree depth

↑ **Parent:** [Decision tree](#decision-tree)

The decision-tree depth $D(f)$ of a [Boolean function](combinatorics.md#boolean-function) $f$ is the smallest possible maximum number of input coordinates queried along any root-to-leaf path of a decision tree computing $f$.

###### Certificate complexity of a Boolean function

↑ **Parent:** [Decision-tree depth](#decision-tree-depth)

A [query certificate](#query-certificate) fixes some input coordinates to their values in a chosen input and must force the output for every completion. The smallest such size is $C(f,x)$; maximizing over accepted or rejected inputs gives $C_1(f)$ or $C_0(f)$, and maximizing both gives $C(f)$. A one-sided maximum over an empty output class is defined as zero. This is [query certificate](#query-certificate) complexity, distinct from polynomial verification of a witness in [NP](#np-complexity).

###### Query certificate

↑ **Parent:** [Certificate complexity of a Boolean function](#certificate-complexity-of-a-boolean-function)

For a [Boolean function](combinatorics.md#boolean-function) $f$ and a chosen input $x$, a set of coordinates $S$ is a [query certificate](#query-certificate) if every $y$ agreeing with $x$ on $S$ has $f(y)=f(x)$. It fixes actual input bits rather than supplying an independently guessed [certificate](#certificate-complexity) to an NP verifier. Minimizing its size at each input and then maximizing gives [query certificate complexity](#certificate-complexity-of-a-boolean-function).

###### Evasive Boolean function

↑ **Parent:** [Decision-tree depth](#decision-tree-depth)

A [Boolean function](combinatorics.md#boolean-function) is evasive when every deterministic [decision tree](#decision-tree) computing it has a worst-case path that queries all input bits. The [alternating-sum criterion for decision-tree evasiveness](#alternating-sum-criterion-for-decision-tree-evasiveness) is one sufficient method for proving this lower bound.

###### Alternating-sum criterion for decision-tree evasiveness

↑ **Parent:** [Evasive Boolean function](#evasive-boolean-function)

A leaf reached before all $n$ input bits are queried leaves at least one coordinate free. Flipping that coordinate pairs its inputs with opposite alternating signs and equal output. Thus every such leaf contributes zero. If the total alternating sum is nonzero, a depth below $n$ is impossible.

###### Decision-tree adversary for a threshold function

↑ **Parent:** [Decision-tree depth](#decision-tree-depth)

To prove that a threshold function requires every input bit in the worst case, an adversary answers queries while keeping completions on both sides of the threshold possible. If this remains true until the final unqueried bit, every decision tree has depth equal to the number of variables.

#### Computational problem

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Computational_problem)

A computational problem specifies the required [output](#output-computing) for every permitted [input](#input-computer-science).

##### Input (computer science)

↑ **Parent:** [Computational problem](#computational-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Input_(computer_science))

An input is the finite data supplied to a computation.

##### Output (computing)

↑ **Parent:** [Computational problem](#computational-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Output_(computing))

An output is the data produced by a computation.

##### Decision problem

↑ **Parent:** [Computational problem](#computational-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Decision_problem)

A decision problem asks for one of two answers, conventionally encoded as zero and one. Equivalently, it asks whether an input belongs to a [formal language](#formal-language).

##### Search problem

↑ **Parent:** [Computational problem](#computational-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Search_problem)

A search problem asks for a witness satisfying a specified relation rather than only whether one exists.

###### Search-to-decision reduction

↑ **Parent:** [Search problem](#search-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Search-to-decision_reduction)

A search-to-decision reduction reconstructs a witness by making queries that only decide whether a suitable witness exists.

#### Complexity class

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complexity_class)

A complexity class is a collection of [computational problems](#computational-problem) sharing specified resource bounds and a computational model.

##### Time complexity

↑ **Parent:** [Complexity class](#complexity-class)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Time_complexity)

The time complexity of an [algorithm](#algorithm) bounds its number of computation steps as a function of its input length.

###### Amortized analysis

↑ **Parent:** [Time complexity](#time-complexity)

Bounds the total cost of a sequence of operations, rather than a probability-weighted average. If a nonnegative potential $\Phi$ assigns stored credit to states, define $\widehat c_i=c_i+\Phi_i-\Phi_{i-1}$. Then $\sum c_i=\sum\widehat c_i+\Phi_0-\Phi_m$. Starting with zero potential, constant amortized costs imply linear total cost.

// Destination: computer-science.bigb

###### Polynomial time

↑ **Parent:** [Time complexity](#time-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_time)

An algorithm runs in polynomial time when its running time is at most $O(n^k)$ for some constant $k$, where $n$ is the input length.

###### Polynomial-time algorithm

↑ **Parent:** [Polynomial time](#polynomial-time)

An algorithm runs in polynomial time if its worst-case running time is bounded by a fixed polynomial in the input length. Arithmetic with fixed-degree algebraic numbers also needs polynomial bit cost when used in such a guarantee. The [Edmonds–Karp algorithm](graph-theory.md#edmonds-karp-algorithm) and the [method of conditional probabilities](#method-of-conditional-probabilities) with efficiently computable [clause](#clause-of-a-boolean-formula) expectations are examples.

###### P (complexity)

↑ **Parent:** [Polynomial time](#polynomial-time)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/P_(complexity))

$\mathbf P$ is the class of [decision problems](#decision-problem) decidable by a [deterministic computation](#deterministic-computation) in [polynomial time](#polynomial-time).

###### P-completeness

↑ **Parent:** [P (complexity)](#p-complexity)

A language in [P](#p-complexity) to which every P language has a [logspace many-one reduction](#logspace-many-one-reduction). The reduction strength matters: using arbitrary polynomial-time reductions instead would make completeness trivial for nontrivial P decision problems.

###### NP (complexity)

↑ **Parent:** [Polynomial time](#polynomial-time)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/NP_(complexity))

$\mathbf{NP}$ is the class of [decision problems](#decision-problem) whose positive instances have polynomial-length [certificates](#certificate-complexity) verifiable in [polynomial time](#polynomial-time). Equivalently, it is polynomial time on a [nondeterministic computation](#nondeterministic-turing-machine).

###### Certificate (complexity)

↑ **Parent:** [NP (complexity)](#np-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Certificate_(complexity))

A certificate for a positive instance is a polynomial-length string that makes a polynomial-time verifier accept that instance.

##### Space complexity

↑ **Parent:** [Complexity class](#complexity-class)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Space_complexity)

The space complexity of an algorithm bounds the amount of working memory it uses as a function of input length.

###### Polynomial space

↑ **Parent:** [Space complexity](#space-complexity)

An algorithm uses polynomial space if its working memory is bounded by a fixed polynomial in the input length. Exponentially many possibilities can still be searched when each candidate and the search counter need polynomial space and storage is reused. The decision problems with deterministic polynomial-space algorithms form [PSPACE](#pspace).

###### Nondeterministic space complexity class

↑ **Parent:** [Space complexity](#space-complexity)

Languages accepted by [Nondeterministic Turing machines](#nondeterministic-turing-machine) using $O(s(n))$ work space on every computation path, with acceptance defined by existence of an accepting path. Bounded-space loops do not prevent the reachability interpretation in the finite [configuration graph](#configuration-graph).

<h6 id="savitch-s-theorem">Savitch's theorem</h6>

↑ **Parent:** [Nondeterministic space complexity class](#nondeterministic-space-complexity-class)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Savitch's_theorem)

Reachability within $2^k$ steps can be tested by enumerating a midpoint and recursively testing two half-paths. Configurations have $O(s)$ bits and recursion depth $O(s)$, yielding deterministic space $O(s^2)$. The [space-bound discovery by exit reachability](#space-bound-discovery-by-exit-reachability) permits this simulation without assuming that the supplied function $s$ is constructible.

###### Space-bound discovery by exit reachability

↑ **Parent:** [Savitch's theorem](#savitch-s-theorem)

For a bounded-space machine, start with a logarithmic work budget and test accepting reachability and reachability of a transition leaving the budget. Accept if acceptance is found, double the budget if an exit is reachable, and otherwise reject. If all paths use at most $Cs(n)$ space, doubling stops at $O(s(n))$. Each budget test uses the [Savitch theorem](#savitch-s-theorem) recursion and the storage is reused. The method discovers a sufficient bound without computing $s(n)$.

###### Deterministic space complexity class

↑ **Parent:** [Space complexity](#space-complexity)

Languages decidable by deterministic [Turing machines](#turing-machine) using $O(s(n))$ work-tape cells with a read-only input. Input-head addresses take $O(\log n)$ bits, while the input itself is not charged to work space. The definition does not require the bound to be computed by the deciding machine.

###### PSPACE

↑ **Parent:** [Deterministic space complexity class](#deterministic-space-complexity-class)

PSPACE consists of decision problems solvable using a polynomial amount of work space. Running time may be exponential. Enumerating all polynomial-length relation encodings and reusing working storage preserves this bound, as does complementation. In particular fixed-sentence [second-order logic](mathematical-logic.md#second-order-logic) model checking lies in PSPACE.

###### Polynomial-register real-arithmetic computation

↑ **Parent:** [Space complexity](#space-complexity)

A [polynomial-register real-arithmetic computation](#polynomial-register-real-arithmetic-computation) stores polynomially many real numbers and may use arbitrarily many additions, subtractions and multiplications, with comparison tests for decisions. Register count does not bound precision or time. Fixed gate constants or sufficiently accurate computable approximations must be specified. This resource model is distinct from ordinary bit-cost computation.

###### Logarithmic space

↑ **Parent:** [Space complexity](#space-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Logarithmic_space)

A logarithmic-space computation uses $O(\!\log n)$ work-tape cells on inputs of length $n$.

###### L (complexity)

↑ **Parent:** [Logarithmic space](#logarithmic-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/L_(complexity))

$\mathbf L$ consists of decision problems solvable by a deterministic [logarithmic space](#logarithmic-space) computation.

###### NL (complexity)

↑ **Parent:** [Logarithmic space](#logarithmic-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/NL_(complexity))

$\mathbf{NL}$ consists of decision problems solvable by a nondeterministic [logarithmic space](#logarithmic-space) computation.

###### NL-complete

↑ **Parent:** [NL (complexity)](#nl-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/NL-complete)

A decision problem is NL-complete when it belongs to [NL](#nl-complexity) and every problem in NL reduces to it by a deterministic logarithmic-space many-one reduction.

###### Directed cycle detection

↑ **Parent:** [NL-complete](#nl-complete)

Decide whether a [directed graph](graph-theory.md#directed-graph) has a nonempty directed cycle; self-loops count. This problem is [NL-complete](#nl-complete). Membership guesses a returning walk of at most the vertex count. For hardness, layer a reachability instance into $N+1$ layers with wait arcs, then add only the backward edge from the target in the last layer to the source in the first. The otherwise acyclic layering has a cycle exactly when the original target is reachable. Zero-length paths must not be treated as cycles.

###### ST-connectivity

↑ **Parent:** [NL-complete](#nl-complete)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/ST-connectivity)

The directed graph reachability problem asks whether a directed graph contains a directed path from a specified vertex $s$ to a specified vertex $t$. It is NL-complete.

###### Configuration graph

↑ **Parent:** [ST-connectivity](#st-connectivity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Configuration_graph)

The configuration graph of a machine on a fixed input has one vertex for each machine configuration and a directed edge for each valid computation step.

###### co-NL

↑ **Parent:** [NL (complexity)](#nl-complexity)

$\mathbf{co\text{-}NL}$ consists of complements of languages in [NL](#nl-complexity).

<h6 id="immerman-szelepcsenyi-theorem">Immerman–Szelepcsényi theorem</h6>

↑ **Parent:** [co-NL](#co-nl)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Immerman–Szelepcsényi_theorem)

The Immerman–Szelepcsényi theorem states that $\mathbf{NL}=\mathbf{co\text{-}NL}$. Its proof uses [inductive counting](#inductive-counting) of reachable configurations.

###### Inductive counting

↑ **Parent:** [Immerman–Szelepcsényi theorem](#immerman-szelepcsenyi-theorem)

Inductive counting certifies the number of vertices reachable within successively larger path-length bounds. Knowing the exact earlier count lets a logarithmic-space nondeterministic machine certify that no reachable predecessor has been omitted.

#### Polynomial-time reduction

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial-time_reduction)

A polynomial-time reduction transforms instances of one computational problem into instances of another using a polynomial-time algorithm.

##### Polynomial-time many-one reduction

↑ **Parent:** [Polynomial-time reduction](#polynomial-time-reduction)

A polynomial-time many-one reduction from a [decision problem](#decision-problem) $A$ to a decision problem $B$ is a polynomial-time computable function $r$ satisfying $x\in A$ exactly when $r(x)\in B$.

###### Logspace many-one reduction

↑ **Parent:** [Polynomial-time many-one reduction](#polynomial-time-many-one-reduction)

A total mapping $f$ with $x\in A$ exactly when $f(x)\in B$, computed by a deterministic logarithmic-work-space transducer with read-only input and write-only output. Such reductions compose, and are used for [NL-completeness](#nl-complete) and [P-completeness](#p-completeness). The output can be polynomially larger than the work storage.

###### NP-hardness

↑ **Parent:** [Polynomial-time many-one reduction](#polynomial-time-many-one-reduction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/NP-hardness)

A decision problem is NP-hard when every problem in [NP](#np-complexity) polynomial-time many-one reduces to it.

###### NP-completeness

↑ **Parent:** [NP-hardness](#np-hardness)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/NP-completeness)

A decision problem is NP-complete when it is both in [NP](#np-complexity) and [NP-hard](#np-hardness).

###### Set cover problem

↑ **Parent:** [NP-completeness](#np-completeness)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Set_cover_problem)

Given subsets $S_1,\ldots,S_m$ of a finite universe, the decision problem asks whether at most $k$ of them cover the universe. It is [NP-complete](#np-completeness). If $k<m$, existence of a cover by at most $k$ subsets is equivalent to existence of a cover by exactly $k$, by adding unused subsets. The promise that every element occurs in some subset loses no hardness: an uncovered element can be detected in polynomial time and mapped to a fixed negative instance.

// Target: mathematical-optimization.bigb

###### Set cover reduction to equilibrium support

↑ **Parent:** [Set cover problem](#set-cover-problem)

Assume $2\leq k<m$ and $\bigcup_iS_i=S$. Construct a two-player game with row $i$ for $S_i$ and columns $0,1,\ldots,n$. Column $0$ pays both players one; column $j>0$ pays $(1,0)$ when $j\in S_i$, and $(0,k/(k-1))$ otherwise. There is a [Nash equilibrium](game-theory.md#nash-equilibrium) whose row player's [support of a mixed strategy](game-theory.md#support-of-a-mixed-strategy) has size $k$ exactly when $k$ rows cover the universe. A uniform mixture on a cover makes column $0$ a [best response](game-theory.md#best-response). Conversely, if some element is uncovered by the support, the column player's [best responses](game-theory.md#best-response) are uncovered elements and the row player's current payoff is zero. The union promise provides a profitable row deviation. Without the union promise the equivalence is false: a globally uncovered element is a [best response](game-theory.md#best-response) against every row mixture.

// Target: mathematical-optimization.bigb

###### Cook-Levin theorem

↑ **Parent:** [NP-completeness](#np-completeness)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cook–Levin_theorem)

Every [NP](#np-complexity) verifier can be compiled into a polynomial-size [Boolean circuit](#boolean-circuit) whose inputs encode its [certificate](#certificate-complexity), and then into an equisatisfiable [conjunctive normal form](#conjunctive-normal-form) by a [Tseitin transformation](#tseytin-transformation). This gives a [polynomial-time many-one reduction](#polynomial-time-many-one-reduction) from every [NP](#np-complexity) language to [SAT](#boolean-satisfiability-problem). Checking a guessed assignment proves membership, so [SAT](#boolean-satisfiability-problem) is [NP-complete](#np-completeness).

###### Subset sum problem

↑ **Parent:** [NP-completeness](#np-completeness)

Given finitely encoded nonnegative integers $s_i$ and target $t$, the subset sum problem asks whether some subset sums to $t$. Taking equal item weights and profits reduces it to testing whether a [0-1 knapsack problem](mathematical-optimization.md#0-1-knapsack-problem) with capacity $t$ attains value $t$.

###### Boolean satisfiability problem

↑ **Parent:** [NP-completeness](#np-completeness)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boolean_satisfiability_problem)

The Boolean satisfiability problem asks whether a Boolean formula has an assignment making it true.

###### Integer programming formulation of satisfiability

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)

Encode each truth value by $t_k\in\{0,1\}$. A positive [Boolean literal](#boolean-literal) has value $t_k$ and its negation has value $1-t_k$. The sum of literal values in a clause is at least one exactly when that clause is true. Thus the displayed inequalities, with objective zero, express [Boolean satisfiability](#boolean-satisfiability-problem) as a binary [integer programming](mathematical-optimization.md#integer-programming) feasibility problem. For [maximum satisfiability](#maximum-satisfiability), introduce $q_i\in\{0,1\}$ with $q_i\leq\sum_{\ell\in C_i}L_\ell(t)$ and maximize $\sum_iq_i$. False clauses force zero indicators; true clauses permit indicators one, and maximization selects all of them. Hence the optimal objective equals the maximum number of true clauses.

###### Maximum satisfiability

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)

Maximum satisfiability asks for a truth assignment maximizing the number of true clauses of a [conjunctive normal form](#conjunctive-normal-form) formula. The [Boolean satisfiability problem](#boolean-satisfiability-problem) asks whether all its clauses can be made true. Binary clause indicators give an [integer programming](mathematical-optimization.md#integer-programming) formulation, and the [literal-frequency greedy approximation for MAX-SAT](#literal-frequency-greedy-approximation-for-max-sat) guarantees at least half the optimum. Counts of clauses, rather than multiplicities of repeated literals within one clause, are relevant to this objective.

###### Literal-frequency greedy approximation for MAX-SAT

↑ **Parent:** [Maximum satisfiability](#maximum-satisfiability)

In the residual unsatisfied formula, choose a [Boolean literal](#boolean-literal) contained in the largest number $a$ of clauses and make it true. Its opposite occurs in at most $a$ clauses, since it too was an eligible literal. The step permanently satisfies $a$ clauses; only clauses containing the opposite can become empty, so it loses at most $a$ clauses. Delete satisfied clauses and false literals and repeat. No satisfied clause or newly empty clause is counted twice. Summing gives total lost nonempty clauses at most total satisfied clauses $G$. All initially nonempty clauses are eventually in one of these classes, so $G\geq N_+/2\geq\operatorname{OPT}/2$. Initial empty clauses can never be satisfied and are excluded from $N_+$. This proves the [approximation algorithm](mathematical-optimization.md#approximation-algorithm) guarantee even with tautological clauses or repeated literals.

###### 2UN-SAT

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)

Satisfiability of [conjunctive normal form](#conjunctive-normal-form) formulas whose [clauses](#clause-of-a-boolean-formula) have at most two unnegated variables. It is [NP-complete](#np-completeness): binary AND/OR and unary NOT gate equivalences in a [Tseitin transformation](#tseytin-transformation) already satisfy that restriction. [Clauses](#clause-of-a-boolean-formula) may contain arbitrarily many negative [literals](#boolean-literal); the total [clause](#clause-of-a-boolean-formula) width is not restricted to two.

###### Maximum 2-satisfiability

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)

Maximum 2-satisfiability asks for an assignment satisfying as many [clause](#clause-of-a-boolean-formula) occurrences as possible when every nonempty [clause](#clause-of-a-boolean-formula) has at most two [literals](#boolean-literal). Occurrences are counted even when a [clause](#clause-of-a-boolean-formula) is repeated. Its decision problem is [NP-complete](#np-completeness) by the [seven-clause gadget for MAX-2SAT](#seven-clause-gadget-for-max-2sat), while the [method of conditional probabilities](#method-of-conditional-probabilities) gives a polynomial-time half approximation.

###### Golden ratio approximation for MAX-2SAT

↑ **Parent:** [Maximum 2-satisfiability](#maximum-2-satisfiability)

When each variable appears in at most one normalized singleton [clause](#clause-of-a-boolean-formula), satisfy that favored [literal](#boolean-literal) with [probability](probability-theory.md#probability) $p>1/2$ and choose independent variables. Every proper binary [clause](#clause-of-a-boolean-formula) is then satisfied with [probability](probability-theory.md#probability) at least $1-p^2$, and every singleton with [probability](probability-theory.md#probability) $p$. Maximize the common lower bound by $p=1-p^2$, giving the reciprocal of the [golden ratio](algebra.md#golden-ratio). The [method of conditional probabilities](#method-of-conditional-probabilities) derandomizes the construction, obtaining [approximation ratio](mathematical-optimization.md#approximation-ratio) $p$. Tautologies are harmless; the singleton restriction must be applied after removing repeated [literals](#boolean-literal) within [clauses](#clause-of-a-boolean-formula).

###### Seven-clause gadget for MAX-2SAT

↑ **Parent:** [Maximum 2-satisfiability](#maximum-2-satisfiability)

A three-[literal](#boolean-literal) disjunction can be represented by ten unit or two-[literal](#boolean-literal) [clause](#clause-of-a-boolean-formula) occurrences with one fresh auxiliary variable. If the number $r$ of true input [literals](#boolean-literal) is zero, the best auxiliary choice satisfies six; for $r=1,2,3$, the best count is seven. Applying separate gadgets to all [clauses](#clause-of-a-boolean-formula) of a [3-SAT](#3-sat) instance gives target seven times the original [clause](#clause-of-a-boolean-formula) count, proving [NP-completeness](#np-completeness) of the decision form of [MAX-2SAT](#maximum-2-satisfiability). The local counting argument is essential: no gadget may exceed seven and compensate for an unsatisfied input [clause](#clause-of-a-boolean-formula).

###### Boolean formula

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)

A Boolean formula is a finite expression built from [Boolean variables](#boolean-variable) and [Boolean operations](#boolean-operation). A choice of truth values determines its value. The [Boolean satisfiability problem](#boolean-satisfiability-problem) asks whether some choice makes it true.

###### Disjunctive normal form

↑ **Parent:** [Boolean formula](#boolean-formula)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Disjunctive_normal_form)

A [Boolean formula](#boolean-formula) is in disjunctive normal form when it is a disjunction of conjunctions of [Boolean literals](#boolean-literal). Width bounds the number of literals in each conjunction, not the number of conjunctions. A depth-$s$ [decision tree](#decision-tree) gives such a formula of width at most $s$ by taking the disjunction of its accepting leaf conditions; rejecting leaves give the dual [conjunctive normal form](#conjunctive-normal-form).

###### Conjunctive normal form

↑ **Parent:** [Boolean formula](#boolean-formula)

A [Boolean formula](#boolean-formula) is in conjunctive normal form when it is a conjunction of [Boolean clauses](#clause-of-a-boolean-formula). It is true precisely when every clause is true; an empty conjunction is true. [3-SAT](#3-sat) restricts each clause to at most three [Boolean literals](#boolean-literal).

###### Tseytin transformation

↑ **Parent:** [Conjunctive normal form](#conjunctive-normal-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tseytin_transformation)

Introduce a [Boolean variable](#boolean-variable) for each gate output and impose its equivalence to the gate's input function with a constant number of [clauses](#clause-of-a-boolean-formula). A final unit [clause](#clause-of-a-boolean-formula) forces acceptance. For a bounded-fan-in [Boolean circuit](#boolean-circuit), the formula size is linear in the gate count and it is satisfiable exactly when some input makes the [Boolean circuit](#boolean-circuit) output one. Auxiliary variables extend the satisfying assignments; this is equisatisfiability, not equality as functions of the enlarged variable set.

###### Clause of a Boolean formula

↑ **Parent:** [Boolean formula](#boolean-formula)

A clause is an expression $\ell_1\lor\cdots\lor\ell_k$ formed from [Boolean literals](#boolean-literal), true when at least one literal is true. The empty clause is false. Repeating a literal does not change the truth value. A [conjunctive normal form](#conjunctive-normal-form) formula is a conjunction of these clauses.

###### Boolean literal

↑ **Parent:** [Boolean formula](#boolean-formula)

A Boolean literal is a [Boolean variable](#boolean-variable) $u$ or its negation $\neg u$. The two literals have opposite truth values. A [Boolean clause](#clause-of-a-boolean-formula) combines literals, and a [Boolean-pair colouring gadget](graph-theory.md#boolean-pair-colouring-gadget) represents a variable and its negation by two vertices with opposite Boolean colours.

###### Boolean variable

↑ **Parent:** [Boolean formula](#boolean-formula)

A Boolean variable takes one of two truth values. It is an input to a [Boolean formula](#boolean-formula); a [Boolean literal](#boolean-literal) uses the variable either positively or negated.

###### 3-SAT

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)

3-SAT is the [Boolean satisfiability problem](#boolean-satisfiability-problem) restricted to [Boolean formulas](#boolean-formula) in [conjunctive normal form](#conjunctive-normal-form) with at most three [Boolean literals](#boolean-literal) per [Boolean clause](#clause-of-a-boolean-formula). It is [NP-complete](#np-completeness). A nonempty short [Boolean clause](#clause-of-a-boolean-formula) can be padded to three positions by repeating a [Boolean literal](#boolean-literal), without changing satisfiability.

###### Horn clause

↑ **Parent:** [Boolean satisfiability problem](#boolean-satisfiability-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Horn_clause)

A Horn clause is a disjunction of literals containing at most one positive literal. It can be read as an implication whose antecedent is a conjunction of variables.

###### Horn-SAT

↑ **Parent:** [Horn clause](#horn-clause)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Horn-SAT)

Horn-SAT asks whether a conjunction of [Horn clauses](#horn-clause) is satisfiable.

###### Horn-SAT forward-chaining algorithm

↑ **Parent:** [Horn-SAT](#horn-sat)

The Horn-SAT forward-chaining algorithm starts with every variable false and repeatedly makes the conclusion of any enabled implication true. It reports failure if it enables a clause with no positive conclusion; otherwise the fixed point is the least satisfying assignment.

###### Quadratic-equation satisfiability over F2

↑ **Parent:** [NP-completeness](#np-completeness)

Quadratic-equation satisfiability over $\mathbb F_2$ asks whether a finite system of polynomial equations of degree at most two over the [finite field](algebra.md#finite-field) $\mathbb F_2$ has a common solution.

<h6 id="ladner-s-theorem">Ladner's theorem</h6>

↑ **Parent:** [NP-completeness](#np-completeness)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ladner's_theorem)

If $\mathbf P\ne\mathbf{NP}$, then [NP](#np-complexity) contains a decision problem that is neither in [P](#p-complexity) nor [NP-complete](#np-completeness).

#### Circuit complexity

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Circuit_complexity)

Circuit complexity studies the size and depth of circuits computing finite-input functions.

##### NC1

↑ **Parent:** [Circuit complexity](#circuit-complexity)

Languages computable by polynomial-size [Boolean circuit](#boolean-circuit) families of bounded fan-in and depth $O(\log n)$. One can specify the nonuniform or logspace-uniform convention explicitly. Balanced constant-size operations give examples such as the [MOD3 binary divisibility problem](#mod3-binary-divisibility-problem) without nonuniform advice.

###### MOD3 binary divisibility problem

↑ **Parent:** [NC1](#nc1)

For a binary numeral, its remainder is the sum of its bits weighted alternately by $+1$ and $-1$ from the least significant position. A [balanced finite-monoid reduction circuit](#balanced-finite-monoid-reduction-circuit) adds these residues modulo three in two-bit encodings. A final zero test gives a uniform linear-size logarithmic-depth [Boolean circuit](#boolean-circuit), proving membership in [NC1](#nc1).

###### Balanced finite-monoid reduction circuit

↑ **Parent:** [NC1](#nc1)

A fixed finite [monoid](algebra.md#monoid) operation has a constant-size Boolean truth-table [Boolean circuit](#boolean-circuit) on its constant-bit encodings. Reduce $n$ elements in a balanced binary tree to get linear size and logarithmic depth. Associativity ensures that tree grouping does not change the product. [MOD3](#mod3-binary-divisibility-problem) uses addition in the three-element residue group, with input-position signs handled at the leaves.

##### Boolean circuit

↑ **Parent:** [Circuit complexity](#circuit-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boolean_circuit)

A Boolean circuit is a finite directed acyclic graph of [Boolean gates](#boolean-operation) with designated inputs and outputs.

###### Circuit size

↑ **Parent:** [Boolean circuit](#boolean-circuit)

The size of a [Boolean circuit](#boolean-circuit) counts its gates, or in another common convention its wires. The convention must be fixed when stating quantitative bounds. In switching arguments, new clauses created from a [decision tree](#decision-tree) are not separate original gates to be charged in the failure union bound.

###### Depth of a Boolean circuit

↑ **Parent:** [Boolean circuit](#boolean-circuit)

Circuit depth is the largest number of counted gates on any input-to-output path in the [Boolean circuit](#boolean-circuit). For an AND/OR circuit with negations on input literals, only the AND/OR gates are counted. This convention makes the restriction argument for the [Linial-Mansour-Nisan theorem](#linial-mansour-nisan-theorem) precise.

###### Circuit value problem

↑ **Parent:** [Boolean circuit](#boolean-circuit)

Given a finite acyclic [Boolean circuit](#boolean-circuit) and its input assignment, determine the output bit. Topological gate evaluation places the problem in [P](#p-complexity); it is a standard [P-complete](#p-completeness) problem under [logspace many-one reductions](#logspace-many-one-reduction). [Boolean circuit](#boolean-circuit) evaluation is different from [Circuit satisfiability problem](#circuit-satisfiability-problem), which asks whether some assignment succeeds.

###### AND-NOT circuit value problem

↑ **Parent:** [Circuit value problem](#circuit-value-problem)

The [circuit value problem](#circuit-value-problem) restricted to AND and NOT gates remains [P-complete](#p-completeness). Replace each OR by $\neg(\neg x\wedge\neg y)$, using a constant-size gadget. Gate indices and gadget positions can be emitted in [logarithmic space](#logarithmic-space), and assignments are preserved. Constants, when needed, can be represented by fixed-valued input nodes.

###### Circuit satisfiability problem

↑ **Parent:** [Boolean circuit](#boolean-circuit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Circuit_satisfiability_problem)

The circuit satisfiability problem asks whether a [Boolean circuit](#boolean-circuit) has an input on which its designated output is one. It is [NP-complete](#np-completeness).

###### Threshold function

↑ **Parent:** [Boolean circuit](#boolean-circuit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Threshold_function)

A threshold Boolean function outputs one exactly when a weighted sum of its input bits reaches a specified threshold. The unweighted threshold function $f_{n,r}$ tests whether at least $r$ of its $n$ inputs are one.

###### Majority function

↑ **Parent:** [Threshold function](#threshold-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Majority_function)

A majority [Boolean function](combinatorics.md#boolean-function) outputs one when more than half its input bits are one. An odd number of inputs avoids a tie convention. For three bits its unique [multilinear polynomial](polynomial.md#multilinear-polynomial) is $x_1x_2+x_1x_3+x_2x_3-2x_1x_2x_3$, so the [polynomial method for quantum query lower bounds](#polynomial-method-for-quantum-query-lower-bounds) requires at least two exact queries.

###### Block conjunction of three-bit majorities

↑ **Parent:** [Majority function](#majority-function)

Its $n$ disjoint triples give a product of degree-three [multilinear polynomials](polynomial.md#multilinear-polynomial), with all-variable coefficient $(-2)^n$. Hence its degree is $3n$ and its [exact quantum query complexity](#exact-quantum-query-complexity) is at least $\lceil3n/2\rceil$. At the input consisting of repeated $110$ triples, each of the $2n$ one bits is a disjoint sensitive singleton. Thus [block sensitivity](combinatorics.md#block-sensitivity) is at least $2n$, implying a bounded-error [quantum query complexity](#quantum-query-complexity) lower bound $\Omega(\sqrt n)$.

###### Dual Boolean function

↑ **Parent:** [Boolean circuit](#boolean-circuit)

The dual of a Boolean function $f$ is $f^*(x)=\neg f(\neg x)$. Swapping AND with OR and zero with one in a monotone circuit for $f$ produces a circuit for $f^*$ by [De Morgan's laws](#de-morgan-s-laws).

##### Circuit family

↑ **Parent:** [Circuit complexity](#circuit-complexity)

A circuit family $(C_n)$ contains one circuit for each input length $n$. The circuit for one length may be chosen independently of those for other lengths, so a family is a nonuniform model of computation.

###### Circuit size class

↑ **Parent:** [Circuit family](#circuit-family)

The languages whose length-$n$ [indicator functions](measure-theory.md#indicator-function) have [Boolean circuits](#boolean-circuit) with at most $T(n)$ gates for sufficiently large $n$, over a fixed bounded-fan-in complete basis. The family need not be constructible by one algorithm. Polynomial-size bounds give [P/poly](#p-poly); the [truth-table upper bound for circuit size](#truth-table-upper-bound-for-circuit-size) applies even to [undecidable](foundations-of-mathematics.md#undecidable-decision-problem) languages.

###### Truth-table upper bound for circuit size

↑ **Parent:** [Circuit size class](#circuit-size-class)

OR together one minterm for each accepted length-$n$ input. Each minterm is an AND of the appropriate [Boolean literals](#boolean-literal). There are at most $2^n$ minterms, and their negated input wires can be shared, giving $O(n2^n)$ bounded-fan-in gates. This is a nonuniform existence statement, not an algorithm for determining an [undecidable](foundations-of-mathematics.md#undecidable-decision-problem) truth table.

###### Polynomial-size circuit family

↑ **Parent:** [Circuit family](#circuit-family)

A circuit family has polynomial size when $C_n$ has at most $n^{O(1)}$ gates.

###### Undecidable unary languages with linear-size circuits

↑ **Parent:** [Polynomial-size circuit family](#polynomial-size-circuit-family)

For any set of lengths $A$, choose at length $n$ a constant-zero [Boolean circuit](#boolean-circuit) when $n\notin A$, and an AND of all inputs when $n\in A$. This uses $O(n+1)$ gates. If $A$ is [undecidable](foundations-of-mathematics.md#undecidable-decision-problem), so is $U_A$, yet it belongs to [P/poly](#p-poly). Since all [NP](#np-complexity) languages are decidable by certificate enumeration, this proves [P/poly](#p-poly) is not equal to [NP](#np-complexity); it does not resolve containment in the other direction.

<h6 id="p-poly">P/poly</h6>

↑ **Parent:** [Polynomial-size circuit family](#polynomial-size-circuit-family)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/P/poly)

$\mathbf P/\mathrm{poly}$ is the class of [decision problems](#decision-problem) decided by [polynomial-size circuit families](#polynomial-size-circuit-family).

##### Constant-depth circuit complexity

↑ **Parent:** [Circuit complexity](#circuit-complexity)

Constant-depth circuit complexity studies circuit families whose depth is bounded independently of the input length.

<h6 id="hastad-switching-lemma">Håstad switching lemma</h6>

↑ **Parent:** [Constant-depth circuit complexity](#constant-depth-circuit-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Håstad_switching_lemma)

The Håstad switching lemma says that a small-width DNF or CNF becomes representable by a shallow [decision tree](#decision-tree) with high probability under a sufficiently sparse random restriction. Iterating it is a central method for proving lower bounds against constant-depth circuits.

###### Switching-lemma depth reduction

↑ **Parent:** [Håstad switching lemma](#hastad-switching-lemma)

Switching-lemma depth reduction applies the [Håstad switching lemma](#hastad-switching-lemma) to every bottom-layer gate, replaces each restricted gate by a shallow decision tree, and merges adjacent layers of the same gate type. Repetition reduces a constant-depth circuit to a bounded-depth decision tree while retaining many live variables.

##### Monotone circuit complexity

↑ **Parent:** [Circuit complexity](#circuit-complexity)

Monotone circuit complexity studies Boolean circuits built only from AND and OR gates, without negations. Such circuits compute [monotone Boolean functions](combinatorics.md#monotone-boolean-function), but some monotone functions require much larger monotone circuits than unrestricted circuits.

###### Monotone circuit

↑ **Parent:** [Monotone circuit complexity](#monotone-circuit-complexity)

A monotone [Boolean circuit](#boolean-circuit) uses only AND and OR gates, variables, and optional constants. It computes a [monotone Boolean function](combinatorics.md#monotone-boolean-function); negation gates are excluded.

###### Superpolynomial monotone clique lower bound

↑ **Parent:** [Monotone circuit complexity](#monotone-circuit-complexity)

In the [finite lattice approximation for monotone clique circuits](#finite-lattice-approximation-for-monotone-clique-circuits), set $m=r=\lfloor n^{1/4}\rfloor$ and $\ell=\lfloor\log_2n\rfloor$. A nonuniversal output accepts at most $\sum_{s=2}^\ell s!(r-1)^s(m/n)^s\leq2(\ell rm/n)^2$ of uniform positive [cliques](graph-theory.md#clique-graph-theory). Its missing positives require the circuit size times the [positive clique error of a truncated lattice meet](#positive-clique-error-of-a-truncated-lattice-meet) to be bounded below. A universal output accepts every negative colouring input; those errors require the circuit size times the [negative colouring error of a forced-set closure](#negative-colouring-error-of-a-forced-set-closure) to be at least one. Both alternatives imply the displayed superpolynomial bound by the [Razborov gate-by-gate approximation lemma](#razborov-gate-by-gate-approximation-lemma).

###### Razborov approximation method

↑ **Parent:** [Monotone circuit complexity](#monotone-circuit-complexity)

The Razborov approximation method replaces the AND and OR operations of a monotone circuit by tractable lattice operations. If each gate introduces only a controlled set of positive or negative errors, a small circuit cannot separate all positive inputs from all negative inputs.

###### Finite lattice approximation for monotone clique circuits

↑ **Parent:** [Razborov approximation method](#razborov-approximation-method)

Take upward-closed [set families](extremal-set-theory.md#set-family) of subsets of $[n]$ of size at most $\ell$, closed under the forcing rule in [Razborov closure](#razborov-closure). Normalize any family containing a set of size at most one to the full family, since its clique predicate is identically true. Intersection is the [meet in a lattice](mathematical-logic.md#meet-in-a-lattice); closure of the union is the [join in a lattice](mathematical-logic.md#join-in-a-lattice). A family represents the [graphs](graph.md) containing a [clique](graph-theory.md#clique-graph-theory) on at least one of its members. The approximate meet can lose positive inputs and the approximate join can acquire negative inputs. The [Razborov gate-by-gate approximation lemma](#razborov-gate-by-gate-approximation-lemma) charges output errors to those local errors.

###### Negative colouring error of a forced-set closure

↑ **Parent:** [Finite lattice approximation for monotone clique circuits](#finite-lattice-approximation-for-monotone-clique-circuits)

Independently colour each [vertex](graph.md#vertex-graph-theory) with one of $m-1$ colours and join differently coloured [vertices](graph.md#vertex-graph-theory). This [complete multipartite graph](graph-theory.md#complete-multipartite-graph) has no $m$-[clique](graph-theory.md#clique-graph-theory). If a forced set $W$ is rainbow but its $r$ witnesses are not, condition on the colours of $W$. The disjoint petals make those failure events [conditionally independent](random-variable.md#conditional-independence). For each witness of size at most $\ell$, the probability of a colour collision is at most $\binom{\ell}{2}/(m-1)$. If this is at most $1/2$, one closure step causes an error with probability at most $2^{-r}$. There are at most $n^{\ell+1}$ possible steps; apply the [union bound](probability-inequality.md#boole-s-inequality).

###### Positive clique error of a truncated lattice meet

↑ **Parent:** [Finite lattice approximation for monotone clique circuits](#finite-lattice-approximation-for-monotone-clique-circuits)

Choose a uniform $m$-subset $Z$ and the [graph](graph.md) consisting only of its [clique](graph-theory.md#clique-graph-theory). Acceptance by two approximating [set families](extremal-set-theory.md#set-family) but rejection by their intersection requires two minimal witnesses whose union has size greater than $\ell$. At least one has size greater than $\ell/2$. The [sunflower bound for minimal members of a Razborov-closed family](#sunflower-bound-for-minimal-members-of-a-razborov-closed-family) and $\mathbb P(W\subseteq Z)\leq(m/n)^{|W|}$ give $2\sum_{s>\ell/2}s!(r-1)^s(m/n)^s\leq4q^{\ell/2}$.

###### Razborov closure

↑ **Parent:** [Razborov approximation method](#razborov-approximation-method)

Fix integers $r$ and $l$. The Razborov closure of a family of vertex sets of size at most $l$ repeatedly adjoins a set $W$ whenever there are $r$ existing sets $W_1,\ldots,W_r$ whose pairwise intersections are contained in $W$. A family equal to its closure is called $r$-closed.

###### Sunflower bound for minimal members of a Razborov-closed family

↑ **Parent:** [Razborov closure](#razborov-closure)

An inclusion-minimal $s$-set in an upward-closed family cannot belong to an $r$-member [delta-system](set-theory.md#delta-system) of such minimal sets: its proper core would be adjoined by [Razborov closure](#razborov-closure), violating minimality. The [Erdős–Rado sunflower lemma](set-theory.md#erdos-rado-sunflower-lemma) therefore bounds the number $a_s$ of minimal $s$-sets. This weaker factorial bound is sufficient for the [superpolynomial monotone clique lower bound](#superpolynomial-monotone-clique-lower-bound).

###### Minimal-member bound for a Razborov-closed family

↑ **Parent:** [Razborov closure](#razborov-closure)

An $r$-closed family has at most $(r-1)^k$ inclusion-minimal members of cardinality $k$. This limits the number of cliques accepted by a proper closed approximation.

###### Razborov gate-by-gate approximation lemma

↑ **Parent:** [Razborov approximation method](#razborov-approximation-method)

The Razborov gate-by-gate approximation lemma compares a monotone circuit with the lattice computation obtained by replacing each gate by an approximate meet or join. Every disagreement at the output is charged to an error introduced by one of the circuit's gates.

##### Natural proof

↑ **Parent:** [Circuit complexity](#circuit-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Natural_proof)

A natural proof lower bound is based on a property of Boolean functions that is simultaneously [constructive](#constructive-property-of-boolean-functions), [large](#large-property-of-boolean-functions), and [useful](#useful-property-against-a-circuit-class) against the circuit class being bounded.

###### Constructive property of Boolean functions

↑ **Parent:** [Natural proof](#natural-proof)

A property of $n$-variable Boolean functions is constructive when membership can be decided from a $2^n$-bit truth table in time polynomial in $2^n$.

###### Large property of Boolean functions

↑ **Parent:** [Natural proof](#natural-proof)

A property of Boolean functions is large when it contains a nonnegligible fraction, customarily at least $2^{-O(n)}$, of all $n$-variable Boolean functions.

###### Useful property against a circuit class

↑ **Parent:** [Natural proof](#natural-proof)

A property is useful against a circuit class when it contains functions at infinitely many input lengths but eventually excludes every function family computed by circuits of the target size in that class.

<h6 id="razborov-rudich-natural-proofs-barrier">Razborov–Rudich natural-proofs barrier</h6>

↑ **Parent:** [Natural proof](#natural-proof)

The Razborov–Rudich natural-proofs barrier says that the existence of sufficiently secure [pseudorandom function families](#pseudorandom-function-family) rules out constructive, large properties useful against the associated circuit class.

##### Pseudorandom function family

↑ **Parent:** [Circuit complexity](#circuit-complexity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pseudorandom_function_family)

A pseudorandom function family is an efficiently computable keyed family whose oracle behavior cannot be distinguished from that of a uniformly random function by the specified class of resource-bounded algorithms.

#### Counting complexity

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Counting_complexity)

Counting complexity studies the resources needed to count witnesses, paths, assignments, or other combinatorial objects rather than merely decide whether one exists.

<h5 id="valiant-s-permanent-reduction">Valiant's permanent reduction</h5>

↑ **Parent:** [Counting complexity](#counting-complexity)

Valiant's permanent reduction encodes satisfying assignments as [cycle covers](graph-theory.md#cycle-cover-of-a-directed-graph) so that their weighted sum is the [permanent of a matrix](linear-algebra.md#permanent-mathematics). Local gadgets enforce variable consistency and clause satisfaction, while signed contributions cancel invalid covers.

<h6 id="variable-gadget-in-valiant-s-permanent-reduction">Variable gadget in Valiant's permanent reduction</h6>

↑ **Parent:** [Valiant's permanent reduction](#valiant-s-permanent-reduction)

The variable gadget has two relevant cycle-cover states, representing the two truth values, and exposes ports that transmit the chosen value to occurrences of the variable.

<h6 id="clause-gadget-in-valiant-s-permanent-reduction">Clause gadget in Valiant's permanent reduction</h6>

↑ **Parent:** [Valiant's permanent reduction](#valiant-s-permanent-reduction)

The clause gadget contributes the required fixed weight precisely when at least one incident literal port represents a satisfying value.

<h6 id="exclusive-or-gadget-in-valiant-s-permanent-reduction">Exclusive-or gadget in Valiant's permanent reduction</h6>

↑ **Parent:** [Valiant's permanent reduction](#valiant-s-permanent-reduction)

The exclusive-or gadget connects two ports while allowing exactly one corresponding external edge to participate. Signed edge weights pair and cancel unwanted cycle covers.

###### Binary path-counting gadget

↑ **Parent:** [Valiant's permanent reduction](#valiant-s-permanent-reduction)

A binary path-counting gadget replaces an edge of nonnegative integer weight $w$ by a zero-one directed graph with exactly $w$ routes from its entrance to its exit. Repeated doubling and conditional addition follow the binary expansion of $w$ using only linearly many vertices in its bit length.

##### Balanced number 3-SAT

↑ **Parent:** [Counting complexity](#counting-complexity)

Balanced number 3-SAT is the counting version of 3-SAT under a promise that every variable has equally many positive and negative occurrences.

#### Polynomial hierarchy

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_hierarchy)

The polynomial hierarchy consists of decision problems described by a constant number of alternating polynomially bounded existential and universal quantifiers with a polynomial-time predicate.

##### Second level of the polynomial hierarchy

↑ **Parent:** [Polynomial hierarchy](#polynomial-hierarchy)

A language is in $\Sigma_2^{\mathbf P}$ when membership has the form $\exists u\,\forall v\,R(x,u,v)$ for a polynomial-time predicate $R$ and polynomially bounded strings. Reversing the quantifiers defines $\Pi_2^{\mathbf P}$.

<h5 id="karp-lipton-theorem">Karp–Lipton theorem</h5>

↑ **Parent:** [Polynomial hierarchy](#polynomial-hierarchy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Karp–Lipton_theorem)

The Karp–Lipton theorem states that $\mathbf{NP}\subseteq\mathbf P/\mathrm{poly}$ implies that the [polynomial hierarchy](#polynomial-hierarchy) collapses to its second level.

#### Primality testing

↑ **Parent:** [Computational complexity theory](#computational-complexity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Primality_testing)

Primality testing is the decision problem of determining whether an input integer is a [prime number](number-theory.md#prime-number).

##### Miller-Rabin primality test

↑ **Parent:** [Primality testing](#primality-testing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Miller–Rabin_primality_test)

For an odd candidate $n>3$, write $n-1=2^s d$ with $d$ odd. A base $a$ passes when $a^d\equiv1\pmod n$ or $a^{2^jd}\equiv-1\pmod n$ for some $0\le j<s$; a nontrivial common divisor of $a,n$ or failure of these conditions proves compositeness. A prime passes every base, while an odd composite passes at most one quarter of possible bases. Independent rounds give a false probable-prime probability at most $4^{-r}$. A passing composite is a [strong pseudoprime](number-theory.md#strong-pseudoprime), stronger than a [Fermat pseudoprime](number-theory.md#fermat-pseudoprime).

##### Fermat primality test

↑ **Parent:** [Primality testing](#primality-testing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fermat_primality_test)

The Fermat test looks for a coprime base $a$ with $a^{N-1}\not\equiv1\pmod N$. Such a witness proves compositeness by the [Fermat little theorem](number-theory.md#fermat-little-theorem), but [Carmichael numbers](number-theory.md#carmichael-number) pass for every coprime base.

##### Pseudoprime base

↑ **Parent:** [Primality testing](#primality-testing)

A base $b$ coprime to the tested odd composite $N$ for which a specified probable-prime criterion passes. The sets of passing bases depend on the criterion and need not be subgroups.

<h5 id="agrawal-biswas-primality-test">Agrawal–Biswas primality test</h5>

↑ **Parent:** [Primality testing](#primality-testing)

The Agrawal–Biswas primality test checks the identity $(X+1)^n=X^n+1$ modulo $n$ and a random low-degree monic polynomial. Prime inputs always pass, while a composite input that is not a prime power fails with inverse-polynomial probability per trial.

## ↑ Ancestors (1)

1. [Codex Wiki](README.md)

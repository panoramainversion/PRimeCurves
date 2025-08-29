# Multivalued Functions, Multivalued Identities, and Branch Parameterization Theory

## Chapter 1: Multivalued Functions and Problem Introduction

Functions in real analysis are single-valued, while in complex analysis, functions often exhibit multivaluedness due to the multivalued nature of the complex argument:

### Definition 1.1 (Multivalued Function)

Let $D \subset \mathbb{C}$ be a domain. A multivalued function $F: D \to \mathbb{C}$ maps each $z \in D$ to a set of values $\\{w_1, w_2, \dots\\}$ (not single-valued).

Examples: $z^{1/2}$ (two-valued), $\log(z)$ (infinitely many-valued).

### Core Issue of Multivalued Identities

Identities in the real number field (such as $\sqrt{z} \cdot \sqrt{w} = \sqrt{zw}$) need to be reinterpreted in the complex field: they hold when both sides are considered as sets of values, rather than for arbitrary single-valued branches.

### Definition 1.2 (Multivalued Identity)

When both sides of the equation take all possible sets of values of their respective functions, each value on the left-hand side corresponds to some value on the right-hand side (and vice versa).

Example: The sets of values of $\sqrt{z} \cdot \sqrt{w}$ and $\sqrt{zw}$ are the same, so this is a multivalued identity (it may not hold when single-valued branches are chosen arbitrarily).

## Chapter 2: Branch Parameterization Theory — A Systematic Approach

By introducing **branch parameters**, multivalued functions are decomposed into families of single-valued branches, converting multivaluedness into parameter dependence.

### Theorem 2.1 (Core Identity of Branch Parameterization)

For a complex number $z$ and branch parameters $\varepsilon, \delta \in \\{0, 1\\}$, the identity holds:

$(z_\varepsilon + z_\delta^{-1})^2 = z^2 + z^{-2} + 2 + \Delta(\varepsilon, \delta)$

where the correction term is  
$\Delta(\varepsilon, \delta) = 2(z_\varepsilon z_\delta^{-1} - 1)$.

### Key Conclusions



*   $z_\varepsilon$ and $z_\delta^{-1}$ are **single-valued branches** specified by parameters, and $z^2$ and $z^{-2}$ are treated as single-valued functions.

*   Branch Compatibility ($\varepsilon = \delta$): $\Delta = 0$, which degenerates to a perfect square: $(z_\varepsilon + z_\varepsilon^{-1})^2 = z^2 + z^{-2} + 2$.

*   Branch Incompatibility ($\varepsilon \neq \delta$): $\Delta \neq 0$, the correction term compensates for branch confusion, ensuring the identity holds strictly.

This theory constructs a **unified and rigorous framework**: multivaluedness is transformed into a parameter-manageable object, supporting rigorous deductions under arbitrary branches.

## Chapter 3: Theoretical Applications and Analysis

Take the square root identity $s + s^{-1} = \pm \sqrt{s^2 + s^{-2} + 2}$ as an example:

### Identification of Multivaluedness

The square root $\sqrt{(\cdot)}$ on the right-hand side is a **two-valued multivalued function** (implied by the $\pm$ symbol).

### Connection to the Core Identity

This identity is a **corollary** of **Theorem 2.1** under branch compatibility ($\varepsilon = \delta$):

Taking the square root of both sides of $(s_\varepsilon + s_\varepsilon^{-1})^2 = s^2 + s^{-2} + 2$, we obtain $s_\varepsilon + s_\varepsilon^{-1} = \pm \sqrt{s^2 + s^{-2} + 2}$.

### Conclusions



*   The left-hand side $s_\varepsilon + s_\varepsilon^{-1}$ is **single-valued under a specific branch**, while the right-hand side is the two-valued set of the square root.

*   This equation is a **multivalued identity**: each branch value on the left-hand side must correspond to some value on the right-hand side (either positive or negative).

The branch parameterization theory **systematizes the study of multivalued functions**, enabling precise deductions through parameters and correction terms, and serves as a core paradigm for addressing multivalued problems.

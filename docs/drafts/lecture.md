# Lecture 1: A Lore Dump

*An Introduction to the cov vs. pp Problem*  
Todd Eisworth

[Original slides](https://toddeisworth.github.io/lecture1-background.pdf)

## Vocabulary

### Ideal language

Let $J$ be an ideal over a set $A$.

- $J^+=\{X\subseteq A:X\notin J\}$ is the collection of $J$-positive subsets of $A$.
- $J^*=\{X\subseteq A:A\setminus X\in J\}$ denotes the dual filter.
- $J\mathbin{\upharpoonright}B=\{X\subseteq A:X\cap B\in J\}$.
- $J+B=J\mathbin{\upharpoonright}(A\setminus B)$.

### Comparisons modulo an ideal

For ordinal-valued functions with domain $A$,

$$
\begin{aligned}
f<_J g &\iff \{a\in A:g(a)\le f(a)\}\in J,\\
f\le_J g &\iff \{a\in A:g(a)<f(a)\}\in J.
\end{aligned}
$$

The definitions of $=_J$ and $\ne_J$ are similar.

### Reduced products

Our basic object of study will be reduced products $\prod A/J$ for $A$ a set of regular cardinals and $J$ an ideal on $A$. We usually assume that $A$ is *progressive*, which means $|A|<|\min(A)|$.

We may also consider indexed products $\prod_{i\in\Gamma}\lambda_i$, where $\Gamma$ is some index set and $\lambda_i$ is a regular cardinal. The reduced product makes sense if $J$ is an ideal on $\Gamma$, and we say that this is a *small product* if

$$
|\Gamma|<\min\{\lambda_i:i\in\Gamma\}.
$$

These approaches are equivalent.

### True cofinality

Let $A$ be a progressive set of regular cardinals, and let $J$ be a proper ideal on $A$. We say

$$
\operatorname{tcf}\left(\prod A/J\right)=\kappa
$$

if $\kappa$ is regular and there is a sequence $\langle f_\alpha:\alpha<\kappa\rangle\subseteq\prod A$ such that

$$
\alpha<\beta<\kappa\implies f_\alpha<_J f_\beta,
$$

and the sequence is cofinal:

$$
(\forall g\in\prod A)(\exists\alpha<\kappa)\quad g<_J f_\alpha.
$$

### Possible cofinalities

If $A$ is a progressive set of regular cardinals, then $\operatorname{pcf}(A)$ is the set of all cardinals $\operatorname{tcf}(\prod A/J)$ where $J$ is an ideal on $A$ and the true cofinality exists. There are many ways of defining the same set of cardinals.

Most important for us is that $\max\operatorname{pcf}(A)$ always exists, and it is equal to the cofinality of $(\prod A,<)$.

### Big picture

If $\lambda$ is singular, there is a connection between

$$
[\lambda]^{<\lambda}
\qquad\text{and}\qquad
\prod(\lambda\cap\operatorname{Reg}).
$$

Questions about the former structure can be translated into questions about the latter, where pcf theory can be used to analyze the situation. How about an example?

## Pseudopowers

### Representability

Let $\lambda$ be a singular cardinal. A cardinal $\kappa$ is *representable at $\lambda$* if there are a set $A$ and an ideal $J$ such that

$$
\begin{aligned}
&A\text{ is cofinal in }\lambda\cap\operatorname{Reg},\\
&|A|=\operatorname{cf}(\lambda),\\
&J\text{ is an ideal on }A\text{ extending }J_A^{\mathrm{bd}},\\
&\kappa=\operatorname{tcf}\left(\prod A/J\right).
\end{aligned}
$$

### The pseudopower function

Put

$$
\begin{aligned}
\operatorname{PP}(\lambda)&=\{\kappa:\kappa\text{ is representable at }\lambda\},\\
\operatorname{pp}(\lambda)&=\sup\operatorname{PP}(\lambda).
\end{aligned}
$$

- Why is $\lambda^+$ representable at $\lambda$?
- If $A=\{\aleph_n:1\le n<\omega\}$, show that

    $$
    \operatorname{PP}(\aleph_\omega)=\operatorname{pcf}(A)\setminus A
    \quad\text{and}\quad
    \operatorname{pp}(\aleph_\omega)=\max\operatorname{pcf}(A).
    $$

### A question

What does the cardinal $\operatorname{pp}(\lambda)$ really mean?

There is some $\delta<\lambda$ such that $\operatorname{pp}(\lambda)$ is the least cardinal $\eta$ with the property that, whenever $A\subseteq(\delta,\lambda)\cap\operatorname{Reg}$ and $|A|=\operatorname{cf}(\lambda)$, we have $\max\operatorname{pcf}(A)\le\eta$.

Can we prove it?

### Note

If $\lambda$ is not a fixed point, then for all sufficiently large $\delta<\lambda$ the set $A=(\delta,\lambda)\cap\operatorname{Reg}$ is a progressive interval of regular cardinals, and we can apply pcf analysis in this setting. This is one reason we know so much more about cardinal arithmetic at non-fixed points, and why getting information when $\lambda=\aleph_\lambda$ is more difficult.

### Restricting the ideals

Assume $\aleph_0\le\sigma=\operatorname{cf}(\sigma)\le\operatorname{cf}(\mu)<\theta<\mu$.

- $\Gamma(\theta,\sigma)$ is the class of proper $\sigma$-complete ideals on sets of cardinality $<\theta$.
- $\operatorname{PP}_{\Gamma(\theta,\sigma)}(\mu)$ consists of all regular cardinals $\kappa$ such that

    $$
    \kappa=\operatorname{tcf}\left(\prod A/J\right),
    $$

    where

    $$
    A\subseteq\mu\cap\operatorname{Reg},\qquad \sup A=\mu,\qquad |A|<\theta,
    $$

    and $J\in\Gamma(\theta,\sigma)$ is an ideal on $A$ extending $J_A^{\mathrm{bd}}$.

## Covering numbers

The covering number $\operatorname{cov}(\lambda,\kappa,\theta,\sigma)$ is the least size of a family

$$
\mathcal X\subseteq[\lambda]^{<\kappa}
$$

such that every $a\in[\lambda]^{<\theta}$ is contained in the union of fewer than $\sigma$ members of $\mathcal X$.

### Easy facts

For fixed values of the other parameters,

- $\operatorname{cov}(\lambda,\kappa,\theta,\sigma)$ is weakly decreasing as $\kappa$ or $\sigma$ increases;
- $\operatorname{cov}(\lambda,\kappa,\theta,\sigma)$ is weakly increasing as $\lambda$ or $\theta$ increases.

### Identities and a pcf bound

Two easy observations:

$$
\begin{aligned}
\operatorname{cov}(\lambda,\kappa,\theta,\aleph_0)
&=\operatorname{cov}(\lambda,\kappa,\theta,2),\\
\operatorname{cov}(\lambda,\kappa^+,\kappa^+,2)
&=\operatorname{cof}\bigl([\lambda]^\kappa,\subseteq\bigr).
\end{aligned}
$$

One not as easy: if $\aleph_0\le\sigma\le\operatorname{cf}(\lambda)<\theta<\lambda$, then

$$
\operatorname{pp}_{\Gamma(\theta,\sigma)}(\lambda)
\le\operatorname{cov}(\lambda,\lambda,\theta,\sigma).
$$

### The cov vs. pp theorem

If $\aleph_0<\sigma=\operatorname{cf}(\sigma)\le\operatorname{cf}(\lambda)<\theta<\lambda$, then

$$
\operatorname{pp}_{\Gamma(\theta,\sigma)}(\lambda)
=\operatorname{cov}(\lambda,\lambda,\theta,\sigma).
$$

### The general cov vs. pp theorem

Suppose as usual $\lambda\ge\kappa\ge\theta>\sigma>\aleph_0$, where $\sigma$ is regular, and put $\Gamma=\Gamma(\theta,\sigma)$.

**Theorem (Shelah).**

$$
\operatorname{cov}(\lambda,\kappa,\theta,\sigma)+\lambda
=\sup_{\substack{\kappa\le\mu\le\lambda\\\sigma\le\operatorname{cf}(\mu)<\theta}}
\operatorname{pp}_\Gamma(\mu)+\lambda.
$$

If $\kappa<\lambda$, then the $+\lambda$ on the left can be omitted.

### Non-fixed points

If $\lambda$ is singular and $\lambda<\aleph_\lambda$, then for every $\kappa$ with $\operatorname{cf}(\lambda)\le\kappa<\lambda$ we have

$$
\operatorname{pp}_\kappa(\lambda)\mathrel{=^{+}}\operatorname{cov}(\lambda,\lambda,\kappa^+,2).
$$

In particular,

$$
\begin{gathered}
\lambda\text{ singular with }\lambda<\aleph_\lambda\\
\implies
\operatorname{pp}(\lambda)\mathrel{=^{+}}\operatorname{cov}(\lambda,\lambda,(\operatorname{cf}\lambda)^+,2).
\end{gathered}
$$

### The problem

Suppose $\lambda$ is singular of countable cofinality. Is

$$
\operatorname{pp}(\lambda)=\operatorname{cov}(\lambda,\lambda,\aleph_1,2)?
$$

The simplest open case is where $\lambda$ is a singular fixed point of countable cofinality and $\operatorname{pp}(\lambda)=\lambda^+$. Is $\operatorname{cov}(\lambda,\lambda,\aleph_1,2)=\lambda^+$?

Moti showed us that the answer to these questions is yes below 0-pistol.

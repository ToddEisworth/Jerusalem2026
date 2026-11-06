# Pseudopowers

The preceding results suggest that, for a singular cardinal $\lambda$, we should study the regular cardinals above $\lambda$ which can occur as true cofinalities of reduced products of regular cardinals converging to $\lambda$ modulo an ideal.

## The spectrum $\operatorname{PP}_\Gamma(\lambda)$

Let $\Gamma$ be a class of proper ideals. For a singular cardinal $\lambda$, define

$$
\operatorname{PP}_\Gamma(\lambda)
$$

to be the set of regular cardinals $\theta$ for which there are:

- an ideal $I\in\Gamma$;
- a sequence $\langle \lambda_i:i\in\operatorname{Dom}(I)\rangle$ of regular cardinals below $\lambda$;

such that

$$
\operatorname{tlim}_I\lambda_i=\lambda
$$

and

$$
\operatorname{tcf}\left(
\prod_{i\in\operatorname{Dom}(I)}\lambda_i,
<_I
\right)=\theta.
$$

Thus

$$
\operatorname{PP}_\Gamma(\lambda)
=
\left\{
\operatorname{tcf}\left(
\prod_{i\in\operatorname{Dom}(I)}\lambda_i,
<_I
\right):
\begin{array}{l}
I\in\Gamma,\\
\lambda_i<\lambda\text{ regular},\\
\operatorname{tlim}_I\lambda_i=\lambda
\end{array}
\right\}.
$$

The set $\operatorname{PP}_\Gamma(\lambda)$ records the regular cardinals above $\lambda$ which can be represented as true cofinalities of reduced products of regular cardinals converging to $\lambda$ modulo an ideal in $\Gamma$.

This is analogous to $\operatorname{pcf}(\mathfrak a)$: instead of fixing a set $\mathfrak a$ of regular cardinals, we fix the singular limit $\lambda$ and allow the sequence of regular cardinals below $\lambda$ to vary.

## Pseudopower

The corresponding **pseudopower** is

$$
\operatorname{pp}_\Gamma(\lambda)
=
\sup \operatorname{PP}_\Gamma(\lambda).
$$

Thus $\operatorname{pp}_\Gamma(\lambda)$ measures how large a regular cardinal can be represented as the true cofinality of a reduced product of regular cardinals with $I$-limit $\lambda$.

For a cardinal $\kappa$, let

$$
\operatorname{PP}_\kappa(\lambda)
$$

denote the spectrum obtained by allowing proper ideals whose domains have cardinality at most $\kappa$, and put

$$
\operatorname{pp}_\kappa(\lambda)
=
\sup\operatorname{PP}_\kappa(\lambda).
$$

The basic pseudopower of a singular cardinal $\lambda$ is

$$
\operatorname{pp}(\lambda)
=
\operatorname{pp}_{\operatorname{cf}(\lambda)}(\lambda).
$$

Shelah introduces $\operatorname{pp}$ as a replacement for cardinal exponentiation adapted to singular cardinals and reduced products.

## Attainment

The supremum defining $\operatorname{pp}_\Gamma(\lambda)$ need not itself belong to
$\operatorname{PP}_\Gamma(\lambda)$.

We write

$$
\theta\leq^+\operatorname{pp}_\Gamma(\lambda)
$$

to mean that either

$$
\theta<\operatorname{pp}_\Gamma(\lambda),
$$

or

$$
\theta=\operatorname{pp}_\Gamma(\lambda)
\quad\text{and}\quad
\theta\in\operatorname{PP}_\Gamma(\lambda).
$$

Thus the notation $\leq^+$ remembers whether the supremum is attained.

## No Holes

The Black Box implies that these spectra contain no gaps.

!!! theorem "No Holes"

    Suppose $\Gamma$ is closed under restriction. If

    $$
    \theta_1\in\operatorname{PP}_\Gamma(\lambda)
    $$

    and $\theta_0$ is regular with

    $$
    \lambda<\theta_0<\theta_1,
    $$

    then

    $$
    \theta_0\in\operatorname{PP}_\Gamma(\lambda).
    $$

Consequently, $\operatorname{PP}_\Gamma(\lambda)$ is an interval of regular cardinals above $\lambda$:

$$
\operatorname{PP}_\Gamma(\lambda)
=
\left\{
\theta:
\lambda<\theta=\operatorname{cf}(\theta)
\text{ and }
\theta\leq^+\operatorname{pp}_\Gamma(\lambda)
\right\}.
$$

Thus, once No Holes is known, the spectrum $\operatorname{PP}_\Gamma(\lambda)$ is determined by its supremum together with whether that supremum is attained.

This is why $\operatorname{pp}_\Gamma(\lambda)$, rather than the entire set
$\operatorname{PP}_\Gamma(\lambda)$, becomes the central invariant.

## Standard classes of ideals

An important family of examples is obtained as follows.

For cardinals $\sigma<\theta$, let

$$
\Gamma(\theta,\sigma)
=
\left\{
I:
I\text{ is a }\sigma\text{-complete ideal on a set of cardinality }<\theta
\right\}.
$$

When $\tau$ is regular, write

$$
\Gamma(\tau)
=
\Gamma(\tau^+,\tau).
$$

We then have the corresponding spectra and pseudopowers

$$
\operatorname{PP}_{\Gamma(\theta,\sigma)}(\lambda)
$$

and

$$
\operatorname{pp}_{\Gamma(\theta,\sigma)}(\lambda).
$$

These classes are particularly useful because suitable closure properties of $\Gamma$ allow the basic structural results about pseudopowers to be applied uniformly.
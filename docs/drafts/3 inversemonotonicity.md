# Closure Properties of the spectrum

The interval $\operatorname{PP}_\Gamma(\lambda)$ is closed under taking true cofinalities of reduced products whose factors lie in $\operatorname{PP}_\Gamma(\lambda)$. The relevant hypothesis on $\Gamma$ is closure under Fubini sums.

## Closure under Fubini sums

Let $I$ be an ideal on $X$, and for each $x\in X$, let $I_x$ be an ideal on $Y_x$. Their **Fubini sum**

$$
J=\sum_I I_x
$$

is the ideal on

$$
Y=\bigsqcup_{x\in X}\bigl(\{x\}\times Y_x\bigr)
$$

defined by

$$
A\in J
$$

if and only if

$$
\{x\in X:A_x\notin I_x\}\in I,
$$

where

$$
A_x=\{y\in Y_x:(x,y)\in A\}.
$$

!!! definition "Closure under Fubini sums"

    A class of ideals $\Gamma$ is **closed under Fubini sums** if, whenever

    $$
    I\in\Gamma
    \qquad\text{and}\qquad
    I_x\in\Gamma
    \quad(x\in X),
    $$

    there is some $B\in J^+$ such that

    $$
    J\upharpoonright B
    $$

    is isomorphic to a member of $\Gamma$, where

    $$
    J=\sum_I I_x.
    $$

This is the weak form of closure under sums used in the applications to pseudopowers.

## Closure of $\operatorname{PP}_\Gamma(\lambda)$

!!! theorem "Closure under $\Gamma$-reduced products"

    Suppose that $\Gamma$ is invariant under isomorphism, closed under restriction, and closed under Fubini sums. Let $\lambda$ be singular.

    Suppose that:

    - $I\in\Gamma$ is an ideal on $X$;
    - $\langle\theta_x:x\in X\rangle$ is a sequence of regular cardinals;
    - for $I$-almost every $x\in X$,

    $$
    \theta_x\in\operatorname{PP}_\Gamma(\lambda);
    $$

    - and

    $$
    \chi=
    \operatorname{tcf}\left(
    \prod_{x\in X}\theta_x,
    <_I
    \right).
    $$

    Then

    $$
    \chi\in\operatorname{PP}_\Gamma(\lambda).
    $$

Thus $\operatorname{PP}_\Gamma(\lambda)$ is closed under true cofinalities of $\Gamma$-reduced products concentrated on $\operatorname{PP}_\Gamma(\lambda)$.

In compact notation, this can be expressed as

$$
\operatorname{pcf}_\Gamma
\bigl(\operatorname{PP}_\Gamma(\lambda)\bigr)
\subseteq
\operatorname{PP}_\Gamma(\lambda).
$$

### Proof

After restricting $I$ to an $I$-large set, we may assume that

$$
\theta_x\in\operatorname{PP}_\Gamma(\lambda)
$$

for every $x\in X$.

For each $x\in X$, choose an ideal $I_x\in\Gamma$ on a set $Y_x$ and regular cardinals

$$
\langle\lambda_{x,y}:y\in Y_x\rangle
$$

such that

$$
\operatorname{tlim}_{I_x}\lambda_{x,y}=\lambda
$$

and

$$
\operatorname{tcf}\left(
\prod_{y\in Y_x}\lambda_{x,y},
<_ {I_x}
\right)=\theta_x.
$$

Let

$$
J=\sum_I I_x.
$$

Flattening the iterated reduced product gives

$$
\prod_{(x,y)\in Y}\lambda_{x,y}/J
\cong
\prod_{x\in X}
\left(
\prod_{y\in Y_x}\lambda_{x,y}/I_x
\right)/I.
$$

Consequently,

$$
\operatorname{tcf}\left(
\prod_{(x,y)\in Y}\lambda_{x,y},
<_J
\right)=\chi.
$$

Moreover,

$$
\operatorname{tlim}_J\lambda_{x,y}=\lambda.
$$

By closure under Fubini sums, there is some $B\in J^+$ such that

$$
J\upharpoonright B
$$

is isomorphic to a member of $\Gamma$.

The restricted product still has true cofinality $\chi$. Indeed, restriction maps the original product cofinally onto the restricted product. The restricted product is also $\chi$-directed, so its true cofinality cannot be less than $\chi$.

Therefore,

$$
\operatorname{tcf}\left(
\prod_{(x,y)\in Y}\lambda_{x,y},
<_{J\upharpoonright B}
\right)=\chi,
$$

and

$$
\operatorname{tlim}_{J\upharpoonright B}\lambda_{x,y}=\lambda.
$$

Hence

$$
\chi\in\operatorname{PP}_\Gamma(\lambda).
$$

## Closure at singular limit points

The preceding theorem gives a closure property of the interval $\operatorname{PP}_\Gamma(\lambda)$ itself.

!!! corollary "Closure at singular limit points"

    Suppose that $\operatorname{PP}_\Gamma(\lambda)$ has no holes, and let $\mu>\lambda$ be singular. If

    $$
    \mu
    =
    \sup\bigl(
    \operatorname{PP}_\Gamma(\lambda)\cap\mu
    \bigr),
    $$

    then

    $$
    \operatorname{PP}_\Gamma(\mu)
    \subseteq
    \operatorname{PP}_\Gamma(\lambda).
    $$

### Proof

Let

$$
\chi\in\operatorname{PP}_\Gamma(\mu).
$$

Choose $I\in\Gamma$ and regular cardinals

$$
\langle\theta_x:x\in X\rangle
$$

such that

$$
\operatorname{tlim}_I\theta_x=\mu
$$

and

$$
\chi=
\operatorname{tcf}\left(
\prod_{x\in X}\theta_x,
<_I
\right).
$$

Since $\operatorname{PP}_\Gamma(\lambda)$ is an interval cofinal in $\mu$, all sufficiently large regular cardinals below $\mu$ belong to $\operatorname{PP}_\Gamma(\lambda)$. Therefore,

$$
\{x\in X:
\theta_x\in\operatorname{PP}_\Gamma(\lambda)\}
$$

is $I$-large.

The closure theorem now gives

$$
\chi\in\operatorname{PP}_\Gamma(\lambda).
$$

Thus

$$
\operatorname{PP}_\Gamma(\mu)
\subseteq
\operatorname{PP}_\Gamma(\lambda).
$$

## Inverse monotonicity

Taking suprema in the preceding inclusion gives

$$
\operatorname{pp}_\Gamma(\mu)
\leq
\operatorname{pp}_\Gamma(\lambda),
$$

with the corresponding refinement when endpoint attainment is recorded using $\leq^+$.

Thus inverse monotonicity is the endpoint form of the closure property

$$
\operatorname{PP}_\Gamma(\mu)
\subseteq
\operatorname{PP}_\Gamma(\lambda).
$$
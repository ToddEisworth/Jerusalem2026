#No Holes

!!! theorem "Black Box"

    Suppose $\lambda$ is singular, $I$ is a proper ideal on $\kappa$, where

    $$
    \operatorname{cf}(\lambda)\leq\kappa<\lambda,
    $$

    and $\langle \lambda_i : i<\kappa\rangle$ is a sequence of regular cardinals from the interval $(\kappa,\lambda)$ satisfying

    $$
    \operatorname{tlim}_I\lambda_i=\lambda.
    $$

    If $\lambda<\theta=\operatorname{cf}(\theta)$ and

    $$
    \left(\prod_{i<\kappa}\lambda_i,<_{I}\right)
    $$

    is $\theta$-directed, then at least one of the following options must hold:

    1. For some $B\in I^+$,

        $$
        \operatorname{tcf}\left(
        \prod_{i\in B}\lambda_i,
        <_{I\restriction B}
        \right)=\theta.
        $$

    2. There are regular cardinals $\mu_i<\lambda_i$ for $i<\kappa$ such that

        $$
        \operatorname{tlim}_I\mu_i=\lambda
        $$

        and

        $$
        \operatorname{tcf}\left(
        \prod_{i<\kappa}\mu_i,
        <_I
        \right)=\theta.
        $$

    If $\left(\prod_{i<\kappa}\lambda_i,<_{I}\right)$ is $\theta^+$-directed, then the first option is impossible, so the second option holds automatically.

!!! corollary "No Holes"

    Suppose $\lambda$ is singular, $I$ is a proper ideal on $\kappa$, where

    $$
    \operatorname{cf}(\lambda)\leq\kappa<\lambda,
    $$

    and $\langle \lambda_i : i<\kappa\rangle$ is a sequence of regular cardinals in $(\kappa,\lambda)$ such that

    $$
    \operatorname{tlim}_I\lambda_i=\lambda
    $$

    and

    $$
    \operatorname{tcf}\left(
    \prod_{i<\kappa}\lambda_i,
    <_I
    \right)=\theta^*.
    $$

    Then for every regular cardinal $\theta$ satisfying

    $$
    \lambda<\theta\leq\theta^*,
    $$

    there is an $I$-positive set $B$ and a sequence
    $\langle \mu_i : i<\kappa\rangle$ of regular cardinals satisfying
    $\mu_i\leq\lambda_i$ such that

    $$
    \operatorname{tlim}_{I\upharpoonright B}\mu_i=\lambda
    $$

    and

    $$
    \operatorname{tcf}\left(
    \prod_{i<\kappa}\mu_i,
    <_{I\upharpoonright B}
    \right)=\theta.
    $$

!!! corollary "Existence of Scales"

    Suppose $\lambda$ is singular of cofinality $\kappa$. There is a strictly increasing sequence
    $\langle \lambda_i : i<\kappa\rangle$ of regular cardinals cofinal in $\lambda$ such that

    $$
    \operatorname{tcf}\left(
    \prod_{i<\kappa}\lambda_i,
    <_{J^{\mathrm{bd}}_\kappa}
    \right)=\lambda^+.
    $$

    Thus, every singular cardinal $\lambda$ carries a scale of length $\lambda^+$ modulo the bounded ideal.
# Exercise Set 1 for the Financial Markets Course

1. Prove proposition
   
If $\succsim$ is rational, then

i) $\succ$ is both irreflexive and transitive.

Since $\succsim$ is rational, we have $x \sim x \ \Rightarrow \ x \succsim x \ \text{and} \ x \precsim x$. Then we have $x \precsim x \ \Rightarrow \ x \nsucc x$. By transitivity of $\succsim$ and the assumptions $x \succ y, y \succ z$, we have $x succ y \ \Rightarrow \ x \succsim y \ \text{and not} \ x \precsim y$ and $y succ z \ \Rightarrow \ x \succsim y \ \text{and not} \ y \precsim z$, then by trasitivity of $\succsim$ we have $x \succsim z \ \text{and not} \ x \precsim z \ \Leftrightarrow \ x \succ z$.

ii) $\sim$ is reflexive, transitive and symmetric.

Since $x \succsim x$ is reflexive we have $\forall x \in X : x \succsim x \ \text{and} \ x \succsim x \ \Leftrightarrow \ x \sim x$. To prove transitivity assume $x \sim y \ \text{and} \ y \sim x$. By reationality of $\succsim$ we have $x \sim y \ \Leftrightarrow \ x \succsim y \ \text{and} \ x \precsim y$ (similarly for $y$ and $z$), and hence $x \succsim z \ \text{and} \ x \precsim z \ \Leftrightarrow \ x \sim z$. Lastly $x \sim y \ \Leftrightarrow \ x \succsim y \wedge x \precsim y \ \Leftrightarrow \ y \succsim x \wedge y \precsim x \ \Leftrightarrow \ y \sim x$.

iii) if $x \succ y \succsim z$ then $x \succ z$.

By the previous properties we have $x \succ y \succsim z \ \Rightarrow \ (x \succsim y \wedge \neg (x \precsim y)) \wedge y \succsim z \ \Rightarrow \ x \succ z$.

2. Consider the lexicographic preference relation $\succsim$ over $\mathbb{R}^2$ defined by $(x_1 > y_1) \vee (x_1 = y_1 \wedge x_2 > y_2) \Rightarrow (x_1, x_2) \succsim (y_1, y_2)$.

i) Show that $\succsim$ is transitive.

Assume $(x_1, x_2) \succsim (y_1, y_2)$ and $(y_1, y_2) \succsim (z_1, z_2)$ by the utilityfunction we have $(x_1 > y_2) \vee (x_1 = y_1 \wedge x_2 > y_2)$, and similarly $(y_1 > z_2) \vee (y_1 = <_1 \wedge y_2 > z_2)$. Therefore $x_1 > z_1 \vee (x_1 = z_1 \wedge x_2 > z_2)$. Hence $(x_1, x_2) \succsim (z_1, z_2)$.

ii) Show that it is not continuous.

Let $x^{(n)}$ be a sequence of bundles defined by $x^{(n)} = (1/n, 0)$ and define $y = (1, 0)$, then for all $n \in \mathbb{N}$ we have $x^{(n)} \succ y$, but in limit as n approaches $\infty$ we have $\lim_{n \to \infty} x^{(n)} \prec y$.

3. Suppose that in a two commodity world, the consumer's utility function takes the form $U(x) = (\alpha_1 x_1^{\rho} + \alpha_2 x_2^{\rho})^{1/\rho}$. This utility function is known as the constant elasticity (or CES) utility function.

i) Show that when $\rho = 1$ indifference curves become linear.

$U(x) = (\alpha_1 x_1^{\rho} + \alpha_2 x_2^{\rho})^{1/\rho} = \alpha_1 x_1 + \alpha_2 x_2$. One could show that this respects the super position principle.

ii) Show that as $\rho \to 0$, this utility function comes to represent the same preferences as the (generalized) cobb-douglas utility function $U(x) = x_1^{\alpha_1}x_2^{\alpha2}$.

Since $U(x)$ is always positive for a positive $\alpha_1, \alpha_2, x_1, x_2$, the monotonic transformation $f(x) = x^p$ is applied. And hence we have $\bar{U}(x) = \alpha_1 x_1^{\rho} + \alpha_2 x_2^{\rho}$ 

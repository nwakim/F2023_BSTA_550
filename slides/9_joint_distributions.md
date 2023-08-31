# Chapter 9: Independence and Conditioning - or, Joint Distributions {#chapter-9-independence-and-conditioning---or-joint-distributions .unnumbered}

::: definition
**Definition 1**. *The **joint pmf** of a pair of discrete r.v.'s $X$
and $Y$ is
$$p_{X,Y}(x,y) = \mathbb{P}(X=x\ and\ Y=y) = \mathbb{P}(X=x, Y=y)$$*
:::

::: {#DrawsBox .example}
**Example 2**. *Let $X$ and $Y$ be two random draws from a box
containing balls labelled 1, 2, and 3 without replacement.*

1.  *Find $p_{X,Y}(x,y)$.*

2.  *Find $\mathbb{P}(X+Y=3).$*

3.  *Find $\mathbb{P}(Y = 1).$*

4.  *Find $\mathbb{P}(Y \leq 2).$*
:::

**Solution:**

**Remarks:** Some properties of joint pmf's:

-   A joint pmf $p_{X,Y}(x,y)$ must satisfy the following properties:

    -   $p_{X,Y}(x,y)\geq 0$ for all $x, y$.

    -   $\sum \limits_{\{all\ x\}} \sum \limits_{\{all\ y\}} p_{X,Y}(x,y)=1$.

-   Marginal pmf's:

    -   $p_X(x) = \sum \limits_{\{all\ y\}} p_{X,Y}(x,y)$

    -   $p_Y(y) = \sum \limits_{\{all\ x\}} p_{X,Y}(x,y)$

::: definition
**Definition 3**. *The **joint cdf** of a pair of discrete r.v.'s $X$
and $Y$ is
$$F_{X,Y}(x,y) = \mathbb{P}(X \leq x\ and\ Y \leq y) = \mathbb{P}(X \leq x, Y \leq y)$$*
:::

------------------------------------------------------------------------

::: {#DrawsBoxCDF .example}
**Example 4**. *Find the joint cdf $F_{X,Y}(x,y)$ for the joint pmf
$p_{X,Y}(x,y)$ in Example [2](#DrawsBox){reference-type="ref"
reference="DrawsBox"}.*
:::

**Solution:**

::: example
**Example 5**. *Find the marginal cdfs $F_{X}(x)$ and $F_{Y}(y)$ for
Example [4](#DrawsBoxCDF){reference-type="ref"
reference="DrawsBoxCDF"}.*
:::

**Solution:**

------------------------------------------------------------------------

**Remark:** Some properties of joint cdf's:

**Independence and Conditioning**

Recall that for *events* $A$ and $B$,

-   $\mathbb{P}(A|B) = \frac{\mathbb{P}(A \cap B)}{\mathbb{P}(B)}$

-   $A$ and $B$ are independent if and only if

    -   $\mathbb{P}(A|B) = \mathbb{P}(A)$

    -   $\mathbb{P}(A \cap B) = \mathbb{P}(A)\cdot\mathbb{P}(B)$

Independence and conditioning are defined similarly for r.v.'s, since
$$p_X(x) = \mathbb{P}(X=x)\ \mathrm{and}\ \ p_{X,Y}(x,y) = \mathbb{P}(X = x ,Y = y).$$

::: definition
**Definition 6**. *The **conditional pmf** of a pair of discrete r.v.'s
$X$ and $Y$ is defined as
$$p_{X|Y}(x|y) = \mathbb{P}(X = x |Y = y) = \frac{\mathbb{P}(X = x\ and\ Y = y)}{\mathbb{P}(Y = y)}
=\frac{p_{X,Y}(x,y) }{p_{Y}(y) }$$ if $p_{Y}(y)  > 0$.*
:::

**Remark:** The following properties follow from the conditional pmf
definition:

::: example
**Example 7**. *Using $X$ and $Y$ from Example
[2](#DrawsBox){reference-type="ref" reference="DrawsBox"}:*

1.  *Find $p_{X|Y}(x|y)$.*

2.  *Are $X$ and $Y$ independent? Why or why not?*
:::

**Solution:**

------------------------------------------------------------------------

**Remark:**

-   To show that $X$ and $Y$ are *not* independent, we just need to find
    one counterexample.

-   However, to show that they are independent, we need to verify this
    for all possible pairs of $x$ and $y$.

::: {#Die4sided .example}
**Example 8**. ***Hypothetical 4-sided die***

-   *Suppose you have a 4-sided die, and you roll the 4-sided die until
    the first 4 appears.*

-   *Let $X$ be the number of rolls required until (and including) the
    first 4.*

-   *After the first 4, you keep rolling it again until you roll a 3.*

-   *Let $Y$ be the number of rolls, after the first 4, required until
    (and including) the 3.*

1.  *Find $p_{X,Y}(x,y)$.*

2.  *Using $p_{X,Y}(x,y)$, find $p_{Y}(y)$.*

3.  *Find $p_{X}(x)$.*

4.  *Are $X$ and $Y$ are independent? Why or why not?*

5.  *Find $F_{X,Y}(x,y)$.*
:::

**Solution:**

Example [8](#Die4sided){reference-type="ref" reference="Die4sided"}
cont'd.

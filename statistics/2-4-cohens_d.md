[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

Using the following Python code that computes Cohen's *d*:

```python
def CohenEffectSize(group1, group2):
    diff = group1.mean() - group2.mean()
    var1 = group1.var()
    var2 = group2.var()
    n1, n2 = len(group1), len(group2)
    28 Chapter 2. Distributions
    pooled_var = (n1 * var1 + n2 * var2) / (n1 + n2)
    d = diff / math.sqrt(pooled_var)
    return d
```

```python
CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb)
```
returns a difference in means of -0.088672927072602 standard deviations, which is small.  It is usually considered a small effect when the absolute value of Cohen's *d* is between 0 between 0.20 standard deviations.  A medium effect is between 0.20 to 0.50 standard deviations, and a large effect is anything over 0.50 standard deviations.  This shows that first babies are lighter than other babies, but although the difference is small, the absolute value is larger than the difference in pregnancy length between first babies and other babies (0.029).


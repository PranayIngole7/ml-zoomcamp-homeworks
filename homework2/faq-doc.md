### Q6 FAQ — Why does my calculated RMSE not match the answer options?

For Question 6, the assignment asks us to:

* split the dataset using seed `9`
* combine train and validation
* fill missing values with `0`
* train regularized linear regression with `r = 0.001`
* calculate test RMSE

Using the official 2026 splitting approach with:

```python
rng = np.random.RandomState(9)
rng.shuffle(idx)
```

the calculated result is:

```text
Test RMSE: 2.2775888434918823
Rounded Test RMSE: 2.278
```

However, the published answer options are:

```text
0.236
2.236
22.10
221.0
```

Therefore, **2.278 does not appear among the published options**.

The important learning point is: **do not choose a merely close option just to match the multiple-choice list.** The calculated RMSE should be trusted when the implementation follows the assignment instructions.

This also demonstrates why reproducibility matters in machine learning: the exact dataset, split method, random seed implementation, preprocessing, and model implementation can all affect the result.

**Conclusion:** My calculated Q6 answer is **2.278**, even though the published options currently do not contain it.

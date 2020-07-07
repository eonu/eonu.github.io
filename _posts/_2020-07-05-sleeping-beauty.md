---
layout: post
title: Test
date: 2016-05-28 15:46
comments: true
external-url:
categories: Mathematics
abstract: Test.
---

```python
class CustomTransform(Transform):
    def __init__(self, *params, p=1., random_state=None):
        super().__init__(p, random_state)
        # 1. Validate and set your parameters as instance variables here

    def _transform(self, X, sr):
        X = self._val.signal(X)

        # 2. Validate the sample rate if it is required for your transformation
        sr = self._val.restricted_integer(sr, 'sr (sample rate)', lambda x: x > 0, 'positive')

        # 3. Sample values for your parameters here
        # 4. Apply the transformation to the signal here
        return X
```
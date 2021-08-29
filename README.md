# Machine Learning Prediction of Clinical Trial Operational Efficiency



This repository contains the weights and parameters for models train to predict six efficiency metrics, from a collaborative project between Stanford and Genentech, a part of the Roche group.

<dt>Efficiency Metrics</dt>
  <dl>Screen Failure Ratio</dl>
  <dl>Dropout Ratio</dl>
  <dl>Pre-enrollment Duration</dl>
  <dl>Enrollment Duration</dl>
  <dl>Trial Duration</dl>
  <dl>Total Enrollment</dl>

The models are implemented in [Light GBM](https://github.com/microsoft/LightGBM) and can be loaded easily:

```python
import lightgbm as lgb

model = lgb.Booster(model_file=MODEL_PATH)
```

The features used in each model can be extracted from the model using `model.feature_name()`, and can be used in inference with `model.predict()`.



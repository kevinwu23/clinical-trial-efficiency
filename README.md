# Machine Learning Prediction of Clinical Trial Operational Efficiency



This repository contains the weights and parameters for models train to predict six efficiency metrics, from a collaborative project between Stanford and Genentech, a part of the Roche group.

<dt>Screen Failure Ratio</dt>
<dt>Dropout Ratio</dt>
<dt>Pre-enrollment Duration</dt>
<dt>Enrollment Duration</dt>
<dt>Trial Duration</dt>
<dt>Total Enrollment</dt>

The models are implemented in [Light GBM](https://github.com/microsoft/LightGBM) and can be loaded easily:

```python
import lightgbm as lgb

model = lgb.Booster(model_file=MODEL_PATH)
```

The features used in each model can be extracted from the model using `model.feature_name()`, and can be used in inference with `model.predict()`.



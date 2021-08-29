# Machine Learning Prediction of Clinical Trial Operational Efficiency

Authors: Kevin Wu, Eric Wu, Michael DAndrea, Nandini Chitale, Melody Lim, Marek Dabrowski, Klaudia Kantor, Hanoor Rangi, Ruishan Liu, Marius Garmhausen, Navdeep Pal, Christopher Harbron, Shemra Rizzo, Ryan Copping, James Zou

This repository contains models from a collaborative project between Stanford and Genentech.

The files found in /models contain the weights and parameters for models train to predict six efficiency metrics, listed below:

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

For any questions or comments, please email kevinywu@stanford.edu



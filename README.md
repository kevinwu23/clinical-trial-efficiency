# Machine Learning Prediction of Clinical Trial Operational Efficiency

This repository contains the model weights and parameters for six efficiency metrics.
The models are implemented in (https://github.com/microsoft/LightGBM "LightGBM") and can be loaded easily:

```python
import lightgbm as lgb

model = lgb.Booster(model_file=MODEL_PATH)
```

The features used in each model can be extracted from the model using `model.feature_name()`, and can be used in inference with `model.predict()`.



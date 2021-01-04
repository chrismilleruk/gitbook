# LightGBM

利用我们的回调函数，只需要一行代码就可以把LightGBM的表现可视化。

```python
from wandb.lightgbm import wandb_callback
import lightgbm as lgb

....

gbm = lgb.train(params,
                lgb_train,
                num_boost_round=20,
                valid_sets=lgb_eval,
                valid_names=('validation'),
                callbacks=[wandb_callback()])
```

See a complete code example in our [examples repo](https://github.com/wandb/examples/tree/master/examples/boosting-algorithms/lightgbm-regression), or as a [colab](https://colab.research.google.com/drive/1R6_vcVM90Ephyu0HDFlPAZa0SgEC_3bE) notebook. 
若要查看完整代码范例，请进入我们的[`范例库`](https://github.com/wandb/examples/tree/master/examples/boosting-algorithms/lightgbm-regression)，或者用[Colab](https://colab.research.google.com/drive/1R6_vcVM90Ephyu0HDFlPAZa0SgEC_3bE)笔记本。

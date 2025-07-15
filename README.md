## Style imitator

팀원 : [허명범](https://github.com/MyungBeomHer)

### 프로젝트 주제 (연세대학교 인공지능 수업)
AI기반 문체 모방기

### 프로젝트 언어 및 환경
프로젝트 언어 : Tensorflow

### Run 
```bash
AI_based_문체모방기.ipynb
```

### Model
<p align="center">
  <img src="/figure/model.png" width=100%> <br>
</p>

```
model = keras.Sequential([
tf.keras.layers.GRU(128, return_sequences=True, input_shape=[None, max_id],
                     dropout=0.2), 
tf.keras.layers.LSTM(128, return_sequences=True, input_shape=[None, max_id]),

tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(max_id,
                                                    activation="softmax"))
])
```
[AI_based_문체모방기.ipynb](AI_based_문체모방기.ipynb)

## Result
### Overall Accuracy 
<p align="center">
  <img src="/figure/overall_accuracy.png" width=100%> <br>
</p>

### Style litmitation Result
<p align="center">
  <img src="/figure/result.png" width=100%> <br>
</p>


# NP_TE

The models are based on the implementation at: [website](https://yanaiela.github.io/TNE).

# How to train:

## for span_right_left model:
* add the model code tne_span_right_left.py to /tne/modeling/models folder
* add config file span_right_left.jsonnet to /tne/modeling/configs
* run: 
```bash
!sudo allennlp train tne/modeling/configs/span_right_left.jsonnet \
         --include-package tne \
         -s models/coupled_large_10_spans_right_left
```

## for span_right model:
* add the model code tne_span_right.py to /tne/modeling/models folder
* add config file span_right.jsonnet to /tne/modeling/configs
* run: 
```bash
!sudo allennlp train tne/modeling/configs/span_right.jsonnet \
         --include-package tne \
         -s models/coupled_large_10_spans_right
```

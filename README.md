# NP_TE

The models are based on the implementation at: [website](https://yanaiela.github.io/TNE).

# How to train:

## for span_right_left model:
* add the model code tne_span_right_left.py to /tne/modeling/models folder
* add config file span_right_left.jsonnet to /tne/modeling/configs
* run: 
```bash
sudo allennlp train tne/modeling/configs/span_right_left.jsonnet \
         --include-package tne \
         -s models/coupled_large_10_spans_right_left
```

## for span_right model:
* add the model code tne_span_right.py to /tne/modeling/models folder
* add config file span_right.jsonnet to /tne/modeling/configs
* run: 
```bash
sudo allennlp train tne/modeling/configs/span_right.jsonnet \
         --include-package tne \
         -s models/coupled_large_10_spans_right
```

## for 4_layer_deeep_model:
* add config file deep4_link_pred.jsonnet to /tne/modeling/configs
* run: 
```bash
sudo allennlp train tne/modeling/configs/deep4_link_pred.jsonnet \
         --include-package tne \
         -s models/coupled_large_10_spans_deep4
```

## for 6_layer_deeep_model:
* add config file deep6_link_pred.jsonnet to /tne/modeling/configs
* run: 
```bash
sudo allennlp train tne/modeling/configs/deep6_link_pred.jsonnet \
         --include-package tne \
         -s models/coupled_large_10_spans_deep6
```

## for convolution_deeep_model:
* add the model code convolutional_link_pred.py to /tne/modeling/models folder
* add config file convolutional_link_pred.jsonnet to /tne/modeling/configs
* run: 
```bash
sudo allennlp train tne/modeling/configs/convolutional_link_pred.jsonnet \
         --include-package tne \
         -s models/coupled_large_10_spans_convolutional
```

# NLP
# Named Entity Recognition (NER) - BILSTM - CRF


## <img src="https://img.icons8.com/external-smashingstocks-flat-smashing-stocks/64/000000/external-manager-hotel-smashingstocks-flat-smashing-stocks-2.png"/> **`Slamet Riyanto S.Kom., M.M.S.I.`**

## <img src="https://img.icons8.com/external-fauzidea-flat-fauzidea/64/undefined/external-man-avatar-avatar-fauzidea-flat-fauzidea.png"/> **`Dimas Dwi Putra`**

## Architecture
<img src="NER-BILSTM-CRF%20Architecture.png" WIDTH="3900">

## Dataset
| Sentence #  | Word        | POS | Tag       |
| ----------- | ----------- | --- | --------- |
| Sentence: 0 | studies     | NNS | O         |
| Sentence: 0 | on          | IN  | O         |
| Sentence: 0 | magnesium   | NN  | O         |
| Sentence: 0 | s           | NN  | O         |
| Sentence: 0 | mechanism   | NN  | O         |
| Sentence: 0 | of          | IN  | O         |
| Sentence: 0 | action      | NN  | O         |
| Sentence: 0 | in          | IN  | O         |
| Sentence: 0 | digitalis   | NN  | B-plant   |
| Sentence: 0 | induced     | VBD | O         |
| Sentence: 0 | arrhythmias | NNS | B-disease |
...

## Eval
| Entities     | precision | recall   | f1-score | support | excecution time | processor | ram  | model | batch size | epochs | embedding | Length | Uji |
| ------------ | --------- | -------- | -------- | ------- | --------------- | --------- | ---- | ----- | ---------- | ------ | --------- | ------ | --- |
| PAD          | 1,000000  | 1,000000 | 1,000000 | 131     | 2.27.31         | cpu       | high | 1     | 16         | 20     | 128       | 3000   | 6   |
| Disease      | 0,660870  | 0,542857 | 0,596078 | 140     |                 |           |      |       |            |        |           |        |     |
| Plant        | 0,861314  | 0,874074 | 0,867647 | 135     |                 |           |      |       |            |        |           |        |     |
| micro avg    | 0,848564  | 0,800493 | 0,823828 | 406     |                 |           |      |       |            |        |           |        |     |
| macro avg    | 0,840728  | 0,805644 | 0,821242 | 406     |                 |           |      |       |            |        |           |        |     |
| weighted avg | 0,836944  | 0,800493 | 0,816708 | 406     |                 |           |      |       |            |        |           |        |     |
| F-1 Scores   |           |          | 82,4%    |         |                 |           |      |       |            |        |           |        |     |
| PAD          | 1,000000  | 1,000000 | 1,000000 | 131     | 4.49.57         | cpu       | high | 2     | 16         | 40     | 128       | 3000   | 7   |
| Disease      | 0,774775  | 0,623188 | 0,690763 | 140     |                 |           |      |       |            |        |           |        |     |
| Plant        | 0,892857  | 0,892857 | 0,892857 | 135     |                 |           |      |       |            |        |           |        |     |
| micro avg    | 0,895288  | 0,836186 | 0,864728 | 406     |                 |           |      |       |            |        |           |        |     |
| macro avg    | 0,889211  | 0,838682 | 0,861207 | 406     |                 |           |      |       |            |        |           |        |     |
| weighted avg | 0,887332  | 0,836186 | 0,858986 | 406     |                 |           |      |       |            |        |           |        |     |
| F-1 Scores   |           |          | 86,5%    |         |                 |           |      |       |            |        |           |        |     |

## Predict
```yaml
Word           ||True ||Pred
==============================
the            : O     O
mutagen        : O     O
sensitivity    : O     O
assay          : O     O
msa            : O     O
a              : O     O
phenotypic     : O     O
marker         : O     O
of             : O     O
dna            : O     O
damage         : O     O
response       : O     O
and            : O     O
repair         : O     O
capacity       : O     O
has            : O     O
been           : O     O
consistently   : O     O
shown          : O     O
to             : O     O
associate      : O     O
with           : O     O
risk           : O     O
tobacco        : plant plant
related        : O     O
cancers        : disease disease
```

## Output
## [Model.hdf5](output/uji%207)
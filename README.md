# kartya-voice-models

Os modelos de voz da carta de pronúncia do Kartya. O app
os baixa na primeira vez e reconhece a voz no próprio aparelho, com o
[sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx): nada do que a pessoa diz
sai do celular.

Este repositório não tem código. Cada versão de modelo é uma release:

| Tag | Idioma | Modelo |
|---|---|---|
| `en-zipformer-2023-06-26-v1` | inglês | zipformer streaming, int8, 72,7 MB |

Cada release traz os arquivos soltos e um `SHA256SUMS`. O app confere o sha256
de cada arquivo antes de usar, e as releases são imutáveis: modelo novo é tag
nova.

Origem e licença de cada modelo estão no `NOTICE`. Os modelos são redistribuídos
sem modificação, sob a Apache License 2.0.



## Google用の音声変換パラメータサンプル

```
sox -V3  cip_solo01_small.aif --encoding signed-integer --bits 16 --channels 1 --rate 16000  cip_solo01_small.wav
```

## 変換

10MB以内なら直接

```
python ./transcribe_async_from_storage.py path/to/wav
```

大きい時は一旦ストレージに。


```
python ./transcribe_async_from_storage.py gs://bucket/key
```

# fizz-few-shot-retriever

**Fizz** (AITuber system in [Almide](https://github.com/almide/almide)) — §3 brain 部品。

着弾コメントに似た過去 Q/A を上位 k 件取得 (文字 bigram の Jaccard)。`select(query, corpus, k)`。

責務は一行で、入力 → 出力が型で言い切れる単位 (openaituber `docs/almide-component-breakdown.md` §3)。

## Install

```toml
[dependencies]
fizz_few_shot_retriever = { git = "https://github.com/aiviecast/fizz-few-shot-retriever", tag = "v0.1.0" }
```

## Tests

```bash
almide test
```

純ロジックなのでネットワーク・API キー不要でテストできる。

# ext

`ext` は，外延性(extensionality)を使うタクティクです．外延性とは，「同じものから作られているものは同じである」という主張のことです．たとえば

* 集合 `A, B ⊂ α` について `A = B` は `x ∈ A ↔ x ∈ B` と同じ
* 2つの写像 `f g : A → B` があるとき `f = g` は `∀ a ∈ A, f a = g a` と同じ

といったことを指します．

`@[ext]` で登録されたルールを使用するため，集合の等式 `A = B` を示すときは `Mathlib.Data.SetLike.Basic` も必要です．

```lean
{{#include ../Examples/Ext.lean}}
```

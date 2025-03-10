@def title = "Seis.jlの紹介"

# Seis.jl の紹介

```!
#hideall
using Pkg; Pkg.activate(".")
```

<!--```julia:./intro_seisjl/releasedate
#hideall
using Dates
today = Dates.today()
println("$(today) 現在、工事中です")
```

\textoutput{./intro_seisjl/releasedate}
-->

現在、工事中です。

\toc

## インストール

以下ではJulia1.10.2を使用しています。Julia の REPL で `]` を押すと Pkg モードに切り替わるので
```julia
julia> ]
(@v1.11) pkg> add https://github.com/anowacki/Geodesics.jl https://github.com/anowacki/Seis.jl
```
と入力して実行します。少しするとパッケージのインストールが完了します。今後は REPL で
```julia
julia> using Seis
```
を実行すると Seis.jl を使えるようになります。

## 波形を読み込む

サンプルデータを読み込みます。
```!
using Seis # hide
```
```>
t = sample_data()
```

`Seis.Trace` というのは Seis.jl における波形データの型であり、以下の field を持ちます。
- 開始時刻 `b`
- サンプリング間隔 `delta`
- 時系列データ `t`
- イベント情報 `evt`
- 観測点情報 `sta`
- ピック `pick`
- メタデータ `meta`

```>
fieldnames(Trace)
```

`Seis.Trace` 型のオブジェクトの property は `t.property` でアクセスできます。例えば
```>
t.b
t.delta
```

<!--なお、`b` は `evt.time` に対するオフセットであり、`Trace` の時刻は `evt.time` に対して `b` だけずれた相対時刻となります。今の場合、`evt.time` が `1981-03-29T10:38:14` なので `Trace` は `1981-03-29T10:39:06.660` から始まることになります。`starttime(t)` で `t.b` を、`startdate(t)` で 絶対的な開始時刻を得られます。

```>
starttime(t)
```
-->

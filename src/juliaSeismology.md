@def title = "Julia Seismology"

# Julia で地震学する

Julia 言語で地震波形データの解析をする際の日本語の参考資料 ⇒ [Qiita](https://qiita.com/ytseis) に書こうと思っています。

## パッケージなど

Julia で書かれた地震学関係のパッケージを私が知っている範囲でまとめます。他にもあれば教えてください。

- [Andy Nowacki](https://github.com/anowacki) さん
  - [SeisTau.jl](https://github.com/anowacki/SeisTau.jl): Seis.Traceにピックを追加、走時の計算
  - [SeisSplit.jl](https://github.com/anowacki/SeisSplit.jl): S波スプリッティング解析ができるらしい
  - [Beamforming.jl](https://github.com/anowacki/Beamforming.jl): beamformingとslowness vespagram
  - [SeisRequests.jl](https://github.com/anowacki/SeisRequests.jl): FDSNやIRISのデータリクエスト
  - [StationXML.jl](https://github.com/anowacki/StationXML.jl): StationXMLの読み書き
  - [QuakeML.jl](https://github.com/anowacki/QuakeML.jl): QuakeMLの読み書き
  - [SeisModels.jl](https://github.com/anowacki/SeisModels.jl): 地球・他の惑星の物性の1次元モデル

- [SeismicJulia](https://github.com/SeismicJulia)
  - [SeisMain.jl](https://github.com/SeismicJulia/SeisMain.jl): Main package for SeismicJulia
  - [SeisAcoustic.jl](https://github.com/SeismicJulia/SeisAcoustic.jl)
  - [SeisMakie.jl](https://github.com/SeismicJulia/SeisMakie.jl.git)
  - [SeisPlot.jl](https://github.com/SeismicJulia/SeisPlot.jl)
  - [SeisProcessing.jl](https://github.com/SeismicJulia/SeisProcessing.jl)
  - [SeisReconstruction.jl](https://github.com/SeismicJulia/SeisReconstruction.jl)
  - [SeisImaging.jl](https://github.com/SeismicJulia/SeisImaging.jl)
  - [SeisOptimization.jl](https://github.com/SeismicJulia/SeisOptimization.jl)
  - ([Seismic.jl](https://github.com/SeismicJulia/Seismic.jl)): Julia0.6で止まっているので非推奨


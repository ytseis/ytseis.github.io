@def title = "Julia Seismology"

# Julia で地震学する

Julia 言語で地震波形データの解析をする際の日本語の参考資料 ⇒ [Qiita](https://qiita.com/ytseis) に書こうと思っています。

## パッケージなど

Julia で書かれた地震学関係のパッケージを私が知っている範囲でまとめます。他にもあれば教えてください。

Data Request Tools
- [SeisRequests.jl]
- [SeisDownload.jl]

Seismic Data Format Conversion
- [Seis.jl]
- [SeisConvert.jl]
- [SeisMain.jl]

Seismic Data Processing

Plotting

Visualization

Traveltime and Ray Tracing

Synthetic Seismograms

- [Andy Nowacki](https://github.com/anowacki) さん
  - [Seis.jl](https://github.com/anowacki/Seis.jl): SAC・miniSEED の読み書きと基本的な処理
  - [SeisTau.jl](https://github.com/anowacki/SeisTau.jl): 走時の計算、ピックの追加
  - [SeisSplit.jl](https://github.com/anowacki/SeisSplit.jl): S波スプリッティング解析ができるらしい
  - [Beamforming.jl](https://github.com/anowacki/Beamforming.jl): beamformingとslowness vespagram
  - [SeisRequests.jl](https://github.com/anowacki/SeisRequests.jl): FDSN や IRIS のデータリクエスト
  - [StationXML.jl](https://github.com/anowacki/StationXML.jl): StationXML の読み書き
  - [QuakeML.jl](https://github.com/anowacki/QuakeML.jl): QuakeML の読み書き
  - [SeisModels.jl](https://github.com/anowacki/SeisModels.jl): 地球や他の惑星の物性の1次元モデル

- [SeismicJulia](https://github.com/SeismicJulia)（あまりわかっていないです）
  - [SeisMain.jl](https://github.com/SeismicJulia/SeisMain.jl): SEGY・Seismic Unixの読み書きなど
  - [SeisAcoustic.jl](https://github.com/SeismicJulia/SeisAcoustic.jl)
  - [SeisMakie.jl](https://github.com/SeismicJulia/SeisMakie.jl.git)
  - [SeisPlot.jl](https://github.com/SeismicJulia/SeisPlot.jl)
  - [SeisProcessing.jl](https://github.com/SeismicJulia/SeisProcessing.jl)
  - [SeisReconstruction.jl](https://github.com/SeismicJulia/SeisReconstruction.jl)
  - [SeisImaging.jl](https://github.com/SeismicJulia/SeisImaging.jl)
  - [SeisOptimization.jl](https://github.com/SeismicJulia/SeisOptimization.jl)
  - ([Seismic.jl](https://github.com/SeismicJulia/Seismic.jl)): Julia0.6で止まっているので非推奨

- [JuliaSeismo](https://github.com/JuliaSeismo)
  - [SeisBase.jl](https://github.com/JuliaSeismo/SeisBase.jl): follow up from [SeisIO.jl](https://github.com/jpjones76/SeisIO.jl)
  - [SeisNoise.jl](https://github.com/JuliaSeismo/SeisNoise.jl): ambient noise cross-correlation

- [大久保 蔵馬](https://kura-okubo.github.io/index_ja.html) さん
  - [SeisMonitoring.jl](https://github.com/kura-okubo/SeisMonitoring.jl): [SeisMonitoring Example](https://github.com/kura-okubo/SeisMonitoring_Example)
  - [SeisDvv.jl](https://github.com/kura-okubo/SeisDvv.jl?tab=readme-ov-file): dv/v の計算
  - [SeisPGVPGA.jl](https://github.com/kura-okubo/SeisPGVPGA.jl): PGV、PGA の計算
  - [MASW.jl](https://github.com/kura-okubo/MASW.jl): Multichannel Analysis of Surface Waves
  - [SeisXcorrelation.jl](https://github.com/jaredbryan881/SeisXcorrelation.jl?tab=readme-ov-file): cross-correlation の計算
  - [SeisRemoveEQ.jl](https://github.com/kura-okubo/SeisRemoveEQ.jl)
  - [SeisDownload.jl](https://github.com/kura-okubo/SeisDownload.jl)
  - [NoiseJul.jl](https://github.com/kura-okubo/NoiseJul.jl): SeisIO、SeisNoise、SeisDownload、SeisConvert、SeisXcorrelation、SeisRemoveEQ、~SeisBeamforming~

- Xiaotao Yang
  - [SeicConvert.jl](https://github.com/xtyangpsp/SeisConvert.jl): SAC/SEGY -> JLD2 -> SAC



- [SPEAR](https://github.com/thehalfspace/Spear): SPectral element based EARthquake cycle simulator
- [SeismicWaves.jl](https://github.com/GinvLab/SeismicWaves.jl)
- [SAC.jl](https://github.com/kura-okubo/SAC.jl)
- [FWI.jl](https://github.com/JuliaInv/FWI.jl)

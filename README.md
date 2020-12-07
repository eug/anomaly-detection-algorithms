# Anomaly Detection Algorithms

This repository aims to provide easy access to any [anomaly detection](https://en.wikipedia.org/wiki/Anomaly_detection) implementation available. The implementations are listed and tagged according to their approaches in a convenient way. It allows researchers and practitioners to easily find the solutions that better suit their needs (i.e. benchmarking, analysis, learning or deployment). Suggestions and improvements for this repository are welcome, just make sure to read the [contribution guidelines](CONTRIBUTING.md). In case you are interested in additional resources about anomaly detection you might find these alternative repositories useful:

- [anomaly-detection-resources](https://github.com/yzhao062/anomaly-detection-resources) - Recent papers, journals/conferences, courses, datasets and libraries.
- [awesome-anomaly-detection](https://github.com/hoya012/awesome-anomaly-detection) - Recent papers on time series and image anomaly detection.
- [awesome-TS-anomaly-detection](https://github.com/rob-med/awesome-TS-anomaly-detection) - Tools and datasets for anomaly detection on time-series data.




### Contents

* [Angle-based](#angle-based)
* [Cluster-based](#cluster-based)
* [Density-based](#density-based)
* [Distance-based](#distance-based)
* [Ensemble](#ensemble)
* [Frequent Pattern](#frequent-pattern)
* [Linear Model](#linear-model)
* [Neural Network and Deep Learning](#neural-network-and-deep-learning)
* [Spatial](#spatial)
* [Statistical](#statistical)
* [Streams](#streams)
* [Subspace](#subspace)
* [Time Series](#time-series)
* [Miscellaneous](#miscellaneous)

--------------------------------------------------------------------------------------------------------------------------------

### Angle-based

| Name | Source Code                              | Tags    |
| ---- | ---------------------------------------- | ------- |
| [ABOD](https://imada.sdu.dk/~zimek/publications/KDD2008/KDD08-ABOD.pdf) | [PyOD](https://github.com/yzhao062/pyod) • [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/anglebased/ABOD.html) • [ADT](http://dsmi-lab-ntust.github.io/AnomalyDetectionToolbox/) | Angle|
| [FastABOD](https://imada.sdu.dk/~zimek/publications/KDD2008/KDD08-ABOD.pdf) | [PyOD](https://github.com/yzhao062/pyod) • [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/anglebased/FastABOD.html) • [ADT](http://dsmi-lab-ntust.github.io/AnomalyDetectionToolbox/) | Angle |
| [LBABOD](https://imada.sdu.dk/~zimek/publications/KDD2008/KDD08-ABOD.pdf) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/anglebased/LBABOD.html) | Angle |


### Cluster-based

| Name | Source Code                              | Tags    |
| ---- | ---------------------------------------- | ------- |
| EMOutlier | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/clustering/EMOutlier.html) | Cluster |
| KMeans* | [ELKI](https://elki-project.github.io/algorithms) | Cluster |
| [OPTICS-OF](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.46.6586&rep=rep1&type=pdf) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/OPTICSOF.html) | Density,Cluster |
| [SilhouetteOutlier](https://pdfs.semanticscholar.org/f168/41e022038e94a59f7e0a82002102b78d79a4.pdf) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/clustering/SilhouetteOutlierDetection.html) | Cluster |


### Density-based

| Name | Source Code                              | Tags    |
| ---- | ---------------------------------------- | ------- |
| [CBLOF](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.20.4242&rep=rep1&type=pdf) | [PyOD](https://github.com/yzhao062/pyod) • [RapidMiner](https://github.com/Markus-Go/rapidminer-anomalydetection) | Density |
| [COF](https://www.researchgate.net/profile/Natasa_Reljin/publication/220847891_Incremental_Connectivity-Based_Outlier_Factor_Algorithm/links/541e18a80cf241a65a189f99/Incremental-Connectivity-Based-Outlier-Factor-Algorithm.pdf)  | [RapidMiner](https://github.com/Markus-Go/rapidminer-anomalydetection) • [ELKI](https://elki-project.github.io/algorithms) • [ADT](http://dsmi-lab-ntust.github.io/AnomalyDetectionToolbox/) • [DDOutlier](https://github.com/jhmadsen/DDoutlier/blob/master/R/OutlierFunctionLibrary.R) | Density |
| [DWOF](https://link.springer.com/chapter/10.1007/978-3-642-38628-2_61) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/DWOF.html) | Density |
| [INFLO](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.66.9380&rep=rep1&type=pdf) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/lof/INFLO.html) • [DDOutlier](https://github.com/jhmadsen/DDoutlier/blob/master/R/OutlierFunctionLibrary.R) | Density |
| [KDEOS](https://epubs.siam.org/doi/pdf/10.1137/1.9781611973440.63) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/lof/KDEOS.html) • [DDOutlier](https://github.com/jhmadsen/DDoutlier/blob/master/R/OutlierFunctionLibrary.R#L559) | Density |
| [LDF](https://pdfs.semanticscholar.org/be49/dbac8e395dba3e8f918924ffe4a55dec34ca.pdf) | [DDOutlier](https://github.com/jhmadsen/DDoutlier/blob/master/R/OutlierFunctionLibrary.R) • [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/lof/LDF.html) | Density |
| [LDF](https://pdfs.semanticscholar.org/be49/dbac8e395dba3e8f918924ffe4a55dec34ca.pdf) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/lof/LDF.html) | Density |
| [LOCI](https://bitquill.net/pdf/loci_icde03.pdf) | [PyOD](https://github.com/yzhao062/pyod) • [RapidMiner](https://github.com/Markus-Go/rapidminer-anomalydetection) • [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/lof/LOCI.html) • [DDOutlier](https://github.com/jhmadsen/DDoutlier/blob/master/R/OutlierFunctionLibrary.R) | Density |
| [LOF](http://www.dbs.ifi.lmu.de/Publikationen/Papers/LOF.pdf)  | [PyOD](https://github.com/yzhao062/pyod) • [RapidMiner](https://github.com/Markus-Go/rapidminer-anomalydetection) • [ELKI](https://elki-project.github.io/algorithms) • [Scikit](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.LocalOutlierFactor.html#sklearn.neighbors.LocalOutlierFactor) • [DDOutlier](https://github.com/jhmadsen/DDoutlier/blob/master/R/OutlierFunctionLibrary.R)  | Density |
| [LoOP](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.161.6229&rep=rep1&type=pdf) | [RapidMiner](https://github.com/Markus-Go/rapidminer-anomalydetection) • [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/lof/LoOP.html) • [DDOutlier](https://github.com/jhmadsen/DDoutlier/blob/master/R/OutlierFunctionLibrary.R) • [PyNomaly](https://github.com/vc1492a/PyNomaly)| Density |
| [OPTICSOF](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.46.6586&rep=rep1&type=pdf) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/OPTICSOF.html) | Density,Cluster |
| [RDOS](https://arxiv.org/abs/1606.08538) | [DDOutlier](https://github.com/jhmadsen/DDoutlier/blob/master/R/OutlierFunctionLibrary.R) | Density |
| [RKOF](http://www.nlpr.ia.ac.cn/2011papers/gjhy/gh116.pdf) | [DDOutlier](https://github.com/jhmadsen/DDoutlier/blob/master/R/OutlierFunctionLibrary.R) | Density, Kernel |
| [TROAD](http://dm.kaist.ac.kr/jaegil/papers/icde08.pdf) | [Trajectory](https://github.com/hansenrl/trajectory) | Distance,Density |


### Distance-based

| Name | Source Code                              | Tags    |
| ---- | ---------------------------------------- | ------- |
| [DB-Out](http://ftp.cse.buffalo.edu/users/azhang/disc/disc01/cd1/out/papers/vldbj/8.34.237.pdf) | [ELKI](https://elki-project.github.io/algorithms) • [DDOutlier](https://github.com/jhmadsen/DDoutlier/blob/master/R/OutlierFunctionLibrary.R) | Distance |
| [Hil-Out](https://www.researchgate.net/profile/Clara_Pizzuti/publication/220699183_Fast_Outlier_Detection_in_High_Dimensional_Spaces/links/542ea6a60cf27e39fa9635c6.pdf) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/distance/HilOut.html) | Distance |
| [kNN](https://dl.acm.org/citation.cfm?id=335437) | [PyOD](https://github.com/yzhao062/pyod) • [RapidMiner](https://github.com/Markus-Go/rapidminer-anomalydetection) • [ELKI](https://elki-project.github.io/algorithms) • [DDOutlier](https://github.com/jhmadsen/DDoutlier/blob/master/R/OutlierFunctionLibrary.R)| Distance |
| [LDOF](http://www.hutter1.net/ai/ldof.pdf) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/lof/LDOF.html) • [ADT](http://dsmi-lab-ntust.github.io/AnomalyDetectionToolbox/) [DDOutlier](https://github.com/jhmadsen/DDoutlier/blob/master/R/OutlierFunctionLibrary.R) | Distance |
| [ODIN](http://cs.joensuu.fi/~villeh/icpr2004.pdf) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/distance/ODIN.html) | Distance |
| [SOS](https://www.tilburguniversity.edu/upload/b7bac5b2-9b00-402a-9261-7849aa019fbb_sostr.pdf) | [PyOD](https://github.com/yzhao062/pyod) • [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/distance/SOS.html) | Distance |
| [TROAD](http://dm.kaist.ac.kr/jaegil/papers/icde08.pdf) | [Trajectory](https://github.com/hansenrl/trajectory) | Distance,Density |
|[Mahalanobis](https://docs.seldon.io/projects/alibi-detect/en/latest/methods/mahalanobis.html)|[alibi-detect](https://github.com/SeldonIO/alibi-detect)|Distance|

### Ensemble

| Name | Source Code                              | Tags    |
| ---- | ---------------------------------------- | ------- |
| [Average Combination](https://www.kdd.org/exploration_files/Article4.pdf) | [PyOD](https://github.com/yzhao062/pyod) | Ensemble |
| [Average of Maximum Combination](https://www.kdd.org/exploration_files/Article4.pdf) | [PyOD](https://github.com/yzhao062/pyod) | Ensemble |
| [Bagging](https://dl.acm.org/citation.cfm?id=1081891) | [PyOD](https://github.com/yzhao062/pyod) • [OutlierDectionToolbox](https://github.com/gokererdogan/OutlierDetectionToolbox) | Ensemble |
| [HiCS](https://ieeexplore.ieee.org/document/6228154) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/meta/HiCS.html) | Ensemble,Subspace |
| [iForest](https://cs.nju.edu.cn/zhouzh/zhouzh.files/publication/icdm08b.pdf) | [PyOD](https://github.com/yzhao062/pyod) • [ADT](http://dsmi-lab-ntust.github.io/AnomalyDetectionToolbox/) • [Scikit](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.IsolationForest.html#sklearn.ensemble.IsolationForest) • [alibi-detect](https://docs.seldon.io/projects/alibi-detect/en/latest/methods/iforest.html) | Ensemble |
| [LSCP](https://arxiv.org/abs/1812.01528) | [PyOD](https://github.com/yzhao062/pyod) | Ensemble |
| [Maximization Combination](https://www.kdd.org/exploration_files/Article4.pdf) | [PyOD](https://github.com/yzhao062/pyod) | Ensemble |
| [Maximization of Average Combination](https://www.kdd.org/exploration_files/Article4.pdf) | [PyOD](https://github.com/yzhao062/pyod)  | Ensemble |
| [PartialLeastSquares](https://onlinelibrary.wiley.com/doi/epdf/10.1002/cem.2922) | [enpls](https://github.com/road2stat/enpls/blob/master/R/enpls.od.R) | Ensemble |
| [Weighted Average Combination](https://www.kdd.org/exploration_files/Article4.pdf) | [PyOD](https://github.com/yzhao062/pyod) | Ensemble |
| [XGBOD](https://ieeexplore.ieee.org/document/8489605) | [PyOD](https://github.com/yzhao062/pyod) | Ensemble |


### Frequent Pattern

| Name | Source Code                              | Tags    |
| ---- | ---------------------------------------- | ------- |
| [FPCOF](https://ieeexplore.ieee.org/document/5363123) | [fpmoutliers](https://github.com/jaroslav-kuchar/fpmoutliers) | Frequent Pattern |
| [FPI](http://proceedings.mlr.press/v71/kuchar18a/kuchar18a.pdf) | [fpmoutliers](https://github.com/jaroslav-kuchar/fpmoutliers) | Frequent Pattern |
| [FPOF](https://pdfs.semanticscholar.org/5f79/d24667a5fc9584c3687569b3b2a75c4f22a7.pdf) | [fpmoutliers](https://github.com/jaroslav-kuchar/fpmoutliers) | Frequent Pattern |
| [LFPOF](https://ieeexplore.ieee.org/document/5571194) | [fpmoutliers](https://github.com/jaroslav-kuchar/fpmoutliers) | Frequent Pattern |
| [MFPOF](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.592.2752&rep=rep1&type=pdf) | [fpmoutliers](https://github.com/jaroslav-kuchar/fpmoutliers) | Frequent Pattern |
| [WCFPOF](https://ieeexplore.ieee.org/document/5376341) | [fpmoutliers](https://github.com/jaroslav-kuchar/fpmoutliers) | Frequent Pattern |
| [WFPOF](http://en.cnki.com.cn/Article_en/CJFDTOTAL-RJXB200704015.htm) | [fpmoutliers](https://github.com/jaroslav-kuchar/fpmoutliers) | Frequent Pattern |


### Linear Model

| Name | Source Code                              | Tags    |
| ---- | ---------------------------------------- | ------- |
| [OCSVM](http://www1.cs.columbia.edu/~kmsvore/ocsvm.pdf) | [PyOD](https://github.com/yzhao062/pyod) • [Scikit](https://scikit-learn.org/stable/modules/generated/sklearn.svm.OneClassSVM.html) | Linear Model |
| [OnlinePCA](http://mml.citi.sinica.edu.tw/papers/TKDE_Yeh.pdf) | [ADT](http://dsmi-lab-ntust.github.io/AnomalyDetectionToolbox/) | Linear Model |
| PCA | [MOA](https://github.com/Waikato/moa) | Linear Model |


### Neural Network and Deep Learning

| Name | Source Code                              | Tags    |
| ---- | ---------------------------------------- | ------- |
| [MO_GAAL](https://arxiv.org/abs/1809.10816) | [PyOD](https://github.com/yzhao062/pyod) • [GAAL-based](https://github.com/leibinghe/GAAL-based-outlier-detection) | Deep Learning |
| [OE](https://arxiv.org/abs/1812.04606) | [outlier-exposure](https://github.com/hendrycks/outlier-exposure) | Deep Learning |
| [SO_GAAL](https://arxiv.org/abs/1809.10816) | [PyOD](https://github.com/yzhao062/pyod) • [GAAL-based](https://github.com/leibinghe/GAAL-based-outlier-detection) | Deep Learning |
| [Likelihood Ratios](https://docs.seldon.io/projects/alibi-detect/en/latest/methods/llr.html) | [alibi-detect](https://github.com/SeldonIO/alibi-detect) | Deep Learning |
| [VAE](https://docs.seldon.io/projects/alibi-detect/en/latest/methods/vae.html) | [alibi-detect](https://github.com/SeldonIO/alibi-detect) | Deep Learning |
| [VAEGMM](https://docs.seldon.io/projects/alibi-detect/en/latest/methods/vaegmm.html) | [alibi-detect](https://github.com/SeldonIO/alibi-detect) | Deep Learning |
| [Auto-Encoder](https://docs.seldon.io/projects/alibi-detect/en/latest/methods/ae.html) | [PyOD](https://github.com/yzhao062/pyod) • [alibi-detect](https://github.com/SeldonIO/alibi-detect) | Deep Learning |
| [AEGMM](https://docs.seldon.io/projects/alibi-detect/en/latest/methods/aegmm.html) | [alibi-detect](https://github.com/SeldonIO/alibi-detect) | Deep Learning |
| [Seq2Seq](https://docs.seldon.io/projects/alibi-detect/en/latest/methods/seq2seq.html) | [alibi-detect](https://github.com/SeldonIO/alibi-detect) | Deep Learning |

### Spatial

| Name | Source Code                              | Tags    |
| ---- | ---------------------------------------- | ------- |
| [SLOM](https://link.springer.com/article/10.1007/s10115-005-0200-2) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/spatial/SLOM.html) | Spatial |
| [SOF](https://ieeexplore.ieee.org/document/1410505) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/spatial/SOF.html) | Spatial |
| CTLu* | [ELKI](https://elki-project.github.io/algorithms) | Spatial |


### Statistical

| Name | Source Code                              | Tags    |
| ---- | ---------------------------------------- | ------- |
| [ChiSquare](https://projecteuclid.org/download/pdf_1/euclid.aoms/1177729747) | [CRAN]( https://cran.r-project.org/web/packages/outliers/index.html) | Statistical |
| [Cochran](https://onlinelibrary.wiley.com/doi/pdf/10.1111/j.1469-1809.1941.tb02271.x) | [CRAN]( https://cran.r-project.org/web/packages/outliers/index.html) | Statistical |
| [Dixon](http://depa.fquim.unam.mx/amyd/archivero/ac1951_23_636_13353.pdf) |  [CRAN]( https://cran.r-project.org/web/packages/outliers/index.html) | Statistical |
| [Grubbs](https://projecteuclid.org/download/pdf_1/euclid.aoms/1177729885) | [CRAN]( https://cran.r-project.org/web/packages/outliers/index.html) • [Skyline](https://github.com/earthgecko/skyline/blob/master/skyline/analyzer/algorithms.py#L142) • [savanna-outliers](https://github.com/savanna-initiative/savanna-outliers)| Statistical |
| [MCD](https://pdfs.semanticscholar.org/d656/2332ad9257b218e4ddcd73d1962d7d9930da.pdf) | [CerioliOD](https://github.com/christopherggreen/CerioliOutlierDetection/blob/master/R/cerioli10.fsrmcd.test.r) | Statistical |
| StddevFromAvg | [Skyline](https://github.com/earthgecko/skyline/blob/master/skyline/analyzer/algorithms.py#L219) | Statistical |


### Streams

| Name | Source Code                              | Tags    |
| ---- | ---------------------------------------- | ------- |
| [AnyOut](https://link.springer.com/chapter/10.1007/978-3-642-29038-1_18) | [MOA](https://github.com/Waikato/moa/blob/master/moa/src/main/java/moa/clusterers/outliers/AnyOut/AnyOut.java) | Streams |
| [ApproxSTORM](http://delab.csd.auth.gr/~papajim/presentations/files/angiulliCIKM2007Detecting.pdf) | [MOA](https://github.com/Waikato/moa/blob/master/moa/src/main/java/moa/clusterers/outliers/Angiulli/ApproxSTORM.java) | Streams |
| [ExactSTORM](http://delab.csd.auth.gr/~papajim/presentations/files/angiulliCIKM2007Detecting.pdf) | [MOA](https://github.com/Waikato/moa/blob/master/moa/src/main/java/moa/clusterers/outliers/Angiulli/ExactSTORM.java) | Streams |
| [MCOD](https://ieeexplore.ieee.org/document/5767923) | [MOA](https://github.com/Waikato/moa/blob/master/moa/src/main/java/moa/clusterers/outliers/MCOD/MCOD.java) | Streams |
| Gaussian | [dsio](https://github.com/MentatInnovations/datastream.io/blob/master/dsio/anomaly_detectors.py#L71) | Streams |
| Percentile | [dsio](https://github.com/MentatInnovations/datastream.io/blob/master/dsio/anomaly_detectors.py#L116) | Streams |
| SST | [Banpei](https://github.com/tsurubee/banpei) • [singular-spectrum-transformation](https://github.com/statefb/singular-spectrum-transformation) | Streams |


### Subspace

| Name | Source Code                              | Tags    |
| ---- | ---------------------------------------- | ------- |
| [COP](https://ieeexplore.ieee.org/document/6413886) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/COP.html) | Subspace |
| [HiCS](https://ieeexplore.ieee.org/document/6228154) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/meta/HiCS.html) | Subspace,Ensemble |
| [OutRankS1](https://ieeexplore.ieee.org/document/4498387) |  [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/subspace/OutRankS1.html) | Subspace |
| [OUTRES](https://dl.acm.org/citation.cfm?id=1871690) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/subspace/OUTRES.html)| Subspace |
| [SOD](http://www.dbs.ifi.lmu.de/Publikationen/Papers/pakdd09_SOD.pdf) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/subspace/SOD.html)| Subspace |


### Time Series

| Name | Source Code                              | Tags    |
| ---- | ---------------------------------------- | ------- |
| [DC](http://alumni.cs.ucr.edu/~dyankov/publications/ICDM07_DiskawareDiscords.pdf) | [ADT](http://dsmi-lab-ntust.github.io/AnomalyDetectionToolbox/) | Time Series |
| [HOTSAX](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.450.1878&rep=rep1&type=pdf) | [ADT](http://dsmi-lab-ntust.github.io/AnomalyDetectionToolbox/) | Time Series |
| EllipticEnvelope | [Scikit](https://scikit-learn.org/stable/modules/generated/sklearn.covariance.EllipticEnvelope.html#sklearn.covariance.EllipticEnvelope) | Time Series |
| Skyline | [Skyline](https://github.com/earthgecko/skyline/blob/master/skyline/analyzer/algorithms.py) | Time Series |
| [S-H-ESD](https://blog.twitter.com/engineering/en_us/a/2015/introducing-practical-and-robust-anomaly-detection-in-a-time-series.html) | [Twitter](https://github.com/twitter/AnomalyDetection) | Time Series |
| [prophet](https://docs.seldon.io/projects/alibi-detect/en/latest/methods/prophet.html) | [alibi-detect](https://github.com/SeldonIO/alibi-detect) | Time Series |
| [Spectral Residual](https://docs.seldon.io/projects/alibi-detect/en/latest/methods/sr.html) | [alibi-detect](https://github.com/SeldonIO/alibi-detect) | Time Series |


### Miscellaneous

| Name | Source Code                              | Tags    |
| ---- | ---------------------------------------- | ------- |
| [CBRW](https://www.ijcai.org/Proceedings/16/Papers/272.pdf) | [CBRW](https://github.com/dkaslovsky/Coupled-Biased-Random-Walks) | Categorical |
| [HBOS](https://pdfs.semanticscholar.org/5cf8/81d1db19834f123fcfc79ad32097aeafe17f.pdf) | [PyOD](https://github.com/yzhao062/pyod) | Histogram |
| [IDOS](https://www.nii.ac.jp/TechReports/public_html/15-003E.pdf) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/intrinsic/IDOS.html) | Intrinsic Dimensionality |
| [ISOS](https://dbs.ifi.uni-heidelberg.de/files/Team/eschubert/publications/SISAP17-itSNE-authorcopy.pdf) | [ELKI](https://elki-project.github.io/releases/current/javadoc/de/lmu/ifi/dbs/elki/algorithm/outlier/intrinsic/ISOS.html) | Intrinsic Dimensionality |
| [KolmogorovEstimator](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.95.5827&rep=rep1&type=pdf) | [ADT](http://dsmi-lab-ntust.github.io/AnomalyDetectionToolbox/) | |
| [TextOut](https://epubs.siam.org/doi/pdf/10.1137/1.9781611974973.55) | [OutlierNMF](https://github.com/ramkikannan/outliernmf/blob/master/textoutliers.m) | Categorical,Text|
| ActiveOutlier | [OutlierDectionToolbox](https://github.com/gokererdogan/OutlierDetectionToolbox) | |
| DRC | [ADT](http://dsmi-lab-ntust.github.io/AnomalyDetectionToolbox/) | |
| ParzenWindows | [OutlierDectionToolbox](https://github.com/gokererdogan/OutlierDetectionToolbox) | |

# HeartRythmClassification
Task 3 of the AML course at ETHZ. We turn now to the classification of entire time series representing heart rythm into one of 4 classes.

## useful links :
* [ECG Heartbeat Arrhythmia Classification Using Time-Series Augmented Signals and Deep Learning Approach](https://pdf.sciencedirectassets.com/280203/1-s2.0-S1877050920X00093/1-s2.0-S1877050920310231/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEPf%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJIMEYCIQDz9I2Af9gT%2BUSWo21I3FhyfzP%2FrNNKHRbache9D9m87wIhAMGFDrB8AFwXr8p17Vjb%2FN5FkZaJdiBUvhwP15hZHylOKrQDCF8QAxoMMDU5MDAzNTQ2ODY1Igxs5TV9EIW%2BJcJF1mEqkQMBcuMjuhKFXKMNn7ZgWlDECTftzWJD57iYa5RV8CKlSKfDdGo%2FGXJLq5MDhLyQH8p7XBhnMRRuNWZxuGWh2iDozYKGX9A%2FMkBW%2BRwqs5vGC%2FhAkKM3NYsRrZstyzIlwGQpdmffN%2F8XUjYfPibzp%2FLAJfnBbkTtQc4eJ3QwjFEGfhjCyUNazA7jcg0RSnZ6iAk7bnXKZX9BbRosCxYwp%2BWv%2B%2FRQmDK%2FMBCZK6a60dTlZdopyTvtx%2FlHQ33Za8PQxAwMUBr8WD8vx5%2Fa612ODX774tr3sRJ0Et5zq%2Bh5ZnYB2LBV04jX40I2r00AJjGqB%2FFcksef91RwdihSSJCFKLVzai2YiuUbDKTGa1KZlRohd8eIkOmuTKEkyKLHvOMpSMreBvyhKiQUSfxBwbm0JwN2rUr8SZLJ4SP8NTtidlaPaKbaySz28tqTUSCw%2BWZOR2QsiF1qU08FMTOsEyaxEg6hn1T0m%2B5jtz0ln9ggEN2fwUloTmNFE2WL5f%2FwmWlxlqmw3QnhK6yaQhxrlQC1Q0JnnzCAoaX9BTrqAfcDUSWul8DZeQBGKV1rr45Hpk8ucI1vagr%2BqcpBPe5UrLgC36Vi8X%2F1NFU7ajgJ1z2puHlZG9RupnUML%2F890tkejT2fRqf0q9AmMp%2BwynEC0fENTxWBY9XxJpaCLdJphHEyibV2TMz%2B3m%2F114JloKNvN7atLsgqGami3JHnzAc5cPL%2BaPrc2jBZA0D4mwTNFxAesE23hIAO2X4Hxy8VEV7OUdxUslhrl7N4NQso5TV7yfW5bRf4JOqu8iyb4gxrqjo%2BfbcPciADrO%2BMQ5SmLMkwVdFPkgwkpDNJuKG%2FvUvy4O0E7S8qmKEoeA%3D%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20201109T154635Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTY2BA4CUP3%2F20201109%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=edde6d382478fe792b2defac2198dbdc47a5edf39a5e927ea25dc6a24cb61590&hash=20722adf7dea94835f39292677d3a91accbc5533593ec1f891316cc9ddbab23b&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S1877050920310231&tid=spdf-4bafea93-5093-4e2f-88f4-ed5c82490e38&sid=ba686071505c684b964922a-59be9f256935gxrqb&type=client) pre-processing info + neural network achitecture
* [QRS Complex analysis](https://en.wikipedia.org/wiki/QRS_complex) ECG results
* [Multi-class Arrhythmia detection from 12-lead varied-length ECG using Attention-based Time-Incremental Convolutional Neural Network](https://www.sciencedirect.com/science/article/pii/S1566253518307632) pre-processing info + neural network achitecture
* [Improved Regularization of Convolutional Neural Networks with Cutout - MAKSED](https://arxiv.org/abs/1708.04552)
* [Time series classification (simple method)](https://www.analyticsvidhya.com/blog/2019/01/introduction-time-series-classification/)
* [Time series classification (complex method)](https://arxiv.org/pdf/1611.06455.pdf)
## Ideas :
1. Trouver les features qui caracterisent un ECG
2. Pour chacune des times series d'ECG, calculer les features precedement trouver
3. features seclection etc
4. creer un model et le train 
5. predictions

## Data Processing :
1. Strecht or compress signal in order to add noise [here](https://www.sciencedirect.com/science/article/pii/S1566253518307632)
2. Random masking [here](https://arxiv.org/abs/1708.04552)
3. Normalization

## Amelioration:
1. Trouver d'autre maniere de pre-process les data sets (mask, strecht etc.)
2. Modifier Neural Network (cf. paper ATTENTION au computation time)
3. Hyper parameter

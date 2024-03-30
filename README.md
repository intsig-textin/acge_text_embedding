---
pipeline_tag: sentence-similarity
tags:
- mteb
- sentence-transformers
- feature-extraction
- sentence-similarity
model-index:
- name: acge_text_embedding
  results:
  - task:
      type: STS
    dataset:
      type: C-MTEB/AFQMC
      name: MTEB AFQMC
      config: default
      split: validation
      revision: b44c3b011063adb25877c13823db83bb193913c4
    metrics:
    - type: cos_sim_pearson
      value: 54.03434872650919
    - type: cos_sim_spearman
      value: 58.80730796688325
    - type: euclidean_pearson
      value: 57.47231387497989
    - type: euclidean_spearman
      value: 58.80775026351807
    - type: manhattan_pearson
      value: 57.46332720141574
    - type: manhattan_spearman
      value: 58.80196022940078
  - task:
      type: STS
    dataset:
      type: C-MTEB/ATEC
      name: MTEB ATEC
      config: default
      split: test
      revision: 0f319b1142f28d00e055a6770f3f726ae9b7d865
    metrics:
    - type: cos_sim_pearson
      value: 53.52621290548175
    - type: cos_sim_spearman
      value: 57.945227768312144
    - type: euclidean_pearson
      value: 61.17041394151802
    - type: euclidean_spearman
      value: 57.94553287835657
    - type: manhattan_pearson
      value: 61.168327500057885
    - type: manhattan_spearman
      value: 57.94477516925043
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_reviews_multi
      name: MTEB AmazonReviewsClassification (zh)
      config: zh
      split: test
      revision: 1399c76144fd37290681b995c656ef9b2e06e26d
    metrics:
    - type: accuracy
      value: 48.538000000000004
    - type: f1
      value: 46.59920995594044
  - task:
      type: STS
    dataset:
      type: C-MTEB/BQ
      name: MTEB BQ
      config: default
      split: test
      revision: e3dda5e115e487b39ec7e618c0c6a29137052a55
    metrics:
    - type: cos_sim_pearson
      value: 68.27529991817154
    - type: cos_sim_spearman
      value: 70.37095914176643
    - type: euclidean_pearson
      value: 69.42690712802727
    - type: euclidean_spearman
      value: 70.37017971889912
    - type: manhattan_pearson
      value: 69.40264877917839
    - type: manhattan_spearman
      value: 70.34786744049524
  - task:
      type: Clustering
    dataset:
      type: C-MTEB/CLSClusteringP2P
      name: MTEB CLSClusteringP2P
      config: default
      split: test
      revision: 4b6227591c6c1a73bc76b1055f3b7f3588e72476
    metrics:
    - type: v_measure
      value: 47.08027536192709
  - task:
      type: Clustering
    dataset:
      type: C-MTEB/CLSClusteringS2S
      name: MTEB CLSClusteringS2S
      config: default
      split: test
      revision: e458b3f5414b62b7f9f83499ac1f5497ae2e869f
    metrics:
    - type: v_measure
      value: 44.0526024940363
  - task:
      type: Reranking
    dataset:
      type: C-MTEB/CMedQAv1-reranking
      name: MTEB CMedQAv1
      config: default
      split: test
      revision: 8d7f1e942507dac42dc58017c1a001c3717da7df
    metrics:
    - type: map
      value: 88.65974993133156
    - type: mrr
      value: 90.64761904761905
  - task:
      type: Reranking
    dataset:
      type: C-MTEB/CMedQAv2-reranking
      name: MTEB CMedQAv2
      config: default
      split: test
      revision: 23d186750531a14a0357ca22cd92d712fd512ea0
    metrics:
    - type: map
      value: 88.90396838907245
    - type: mrr
      value: 90.90932539682541
  - task:
      type: Retrieval
    dataset:
      type: C-MTEB/CmedqaRetrieval
      name: MTEB CmedqaRetrieval
      config: default
      split: dev
      revision: cd540c506dae1cf9e9a59c3e06f42030d54e7301
    metrics:
    - type: map_at_1
      value: 26.875
    - type: map_at_10
      value: 39.995999999999995
    - type: map_at_100
      value: 41.899
    - type: map_at_1000
      value: 42.0
    - type: map_at_3
      value: 35.414
    - type: map_at_5
      value: 38.019
    - type: mrr_at_1
      value: 40.635
    - type: mrr_at_10
      value: 48.827
    - type: mrr_at_100
      value: 49.805
    - type: mrr_at_1000
      value: 49.845
    - type: mrr_at_3
      value: 46.145
    - type: mrr_at_5
      value: 47.693999999999996
    - type: ndcg_at_1
      value: 40.635
    - type: ndcg_at_10
      value: 46.78
    - type: ndcg_at_100
      value: 53.986999999999995
    - type: ndcg_at_1000
      value: 55.684
    - type: ndcg_at_3
      value: 41.018
    - type: ndcg_at_5
      value: 43.559
    - type: precision_at_1
      value: 40.635
    - type: precision_at_10
      value: 10.427999999999999
    - type: precision_at_100
      value: 1.625
    - type: precision_at_1000
      value: 0.184
    - type: precision_at_3
      value: 23.139000000000003
    - type: precision_at_5
      value: 17.004
    - type: recall_at_1
      value: 26.875
    - type: recall_at_10
      value: 57.887
    - type: recall_at_100
      value: 87.408
    - type: recall_at_1000
      value: 98.721
    - type: recall_at_3
      value: 40.812
    - type: recall_at_5
      value: 48.397
  - task:
      type: PairClassification
    dataset:
      type: C-MTEB/CMNLI
      name: MTEB Cmnli
      config: default
      split: validation
      revision: 41bc36f332156f7adc9e38f53777c959b2ae9766
    metrics:
    - type: cos_sim_accuracy
      value: 83.43956704750451
    - type: cos_sim_ap
      value: 90.49172854352659
    - type: cos_sim_f1
      value: 84.28475486903963
    - type: cos_sim_precision
      value: 80.84603822203135
    - type: cos_sim_recall
      value: 88.02899228431144
    - type: dot_accuracy
      value: 83.43956704750451
    - type: dot_ap
      value: 90.46317132695233
    - type: dot_f1
      value: 84.28794294628929
    - type: dot_precision
      value: 80.51948051948052
    - type: dot_recall
      value: 88.4264671498714
    - type: euclidean_accuracy
      value: 83.43956704750451
    - type: euclidean_ap
      value: 90.49171785256486
    - type: euclidean_f1
      value: 84.28235820561584
    - type: euclidean_precision
      value: 80.8022308022308
    - type: euclidean_recall
      value: 88.07575403320084
    - type: manhattan_accuracy
      value: 83.55983162958509
    - type: manhattan_ap
      value: 90.48046779812815
    - type: manhattan_f1
      value: 84.45354259069714
    - type: manhattan_precision
      value: 82.21877767936226
    - type: manhattan_recall
      value: 86.81318681318682
    - type: max_accuracy
      value: 83.55983162958509
    - type: max_ap
      value: 90.49172854352659
    - type: max_f1
      value: 84.45354259069714
  - task:
      type: Retrieval
    dataset:
      type: C-MTEB/CovidRetrieval
      name: MTEB CovidRetrieval
      config: default
      split: dev
      revision: 1271c7809071a13532e05f25fb53511ffce77117
    metrics:
    - type: map_at_1
      value: 68.54599999999999
    - type: map_at_10
      value: 77.62400000000001
    - type: map_at_100
      value: 77.886
    - type: map_at_1000
      value: 77.89
    - type: map_at_3
      value: 75.966
    - type: map_at_5
      value: 76.995
    - type: mrr_at_1
      value: 68.915
    - type: mrr_at_10
      value: 77.703
    - type: mrr_at_100
      value: 77.958
    - type: mrr_at_1000
      value: 77.962
    - type: mrr_at_3
      value: 76.08
    - type: mrr_at_5
      value: 77.118
    - type: ndcg_at_1
      value: 68.809
    - type: ndcg_at_10
      value: 81.563
    - type: ndcg_at_100
      value: 82.758
    - type: ndcg_at_1000
      value: 82.864
    - type: ndcg_at_3
      value: 78.29
    - type: ndcg_at_5
      value: 80.113
    - type: precision_at_1
      value: 68.809
    - type: precision_at_10
      value: 9.463000000000001
    - type: precision_at_100
      value: 1.001
    - type: precision_at_1000
      value: 0.101
    - type: precision_at_3
      value: 28.486
    - type: precision_at_5
      value: 18.019
    - type: recall_at_1
      value: 68.54599999999999
    - type: recall_at_10
      value: 93.625
    - type: recall_at_100
      value: 99.05199999999999
    - type: recall_at_1000
      value: 99.895
    - type: recall_at_3
      value: 84.879
    - type: recall_at_5
      value: 89.252
  - task:
      type: Retrieval
    dataset:
      type: C-MTEB/DuRetrieval
      name: MTEB DuRetrieval
      config: default
      split: dev
      revision: a1a333e290fe30b10f3f56498e3a0d911a693ced
    metrics:
    - type: map_at_1
      value: 25.653
    - type: map_at_10
      value: 79.105
    - type: map_at_100
      value: 81.902
    - type: map_at_1000
      value: 81.947
    - type: map_at_3
      value: 54.54599999999999
    - type: map_at_5
      value: 69.226
    - type: mrr_at_1
      value: 89.35
    - type: mrr_at_10
      value: 92.69
    - type: mrr_at_100
      value: 92.77
    - type: mrr_at_1000
      value: 92.774
    - type: mrr_at_3
      value: 92.425
    - type: mrr_at_5
      value: 92.575
    - type: ndcg_at_1
      value: 89.35
    - type: ndcg_at_10
      value: 86.55199999999999
    - type: ndcg_at_100
      value: 89.35300000000001
    - type: ndcg_at_1000
      value: 89.782
    - type: ndcg_at_3
      value: 85.392
    - type: ndcg_at_5
      value: 84.5
    - type: precision_at_1
      value: 89.35
    - type: precision_at_10
      value: 41.589999999999996
    - type: precision_at_100
      value: 4.781
    - type: precision_at_1000
      value: 0.488
    - type: precision_at_3
      value: 76.683
    - type: precision_at_5
      value: 65.06
    - type: recall_at_1
      value: 25.653
    - type: recall_at_10
      value: 87.64999999999999
    - type: recall_at_100
      value: 96.858
    - type: recall_at_1000
      value: 99.13300000000001
    - type: recall_at_3
      value: 56.869
    - type: recall_at_5
      value: 74.024
  - task:
      type: Retrieval
    dataset:
      type: C-MTEB/EcomRetrieval
      name: MTEB EcomRetrieval
      config: default
      split: dev
      revision: 687de13dc7294d6fd9be10c6945f9e8fec8166b9
    metrics:
    - type: map_at_1
      value: 52.1
    - type: map_at_10
      value: 62.629999999999995
    - type: map_at_100
      value: 63.117000000000004
    - type: map_at_1000
      value: 63.134
    - type: map_at_3
      value: 60.267
    - type: map_at_5
      value: 61.777
    - type: mrr_at_1
      value: 52.1
    - type: mrr_at_10
      value: 62.629999999999995
    - type: mrr_at_100
      value: 63.117000000000004
    - type: mrr_at_1000
      value: 63.134
    - type: mrr_at_3
      value: 60.267
    - type: mrr_at_5
      value: 61.777
    - type: ndcg_at_1
      value: 52.1
    - type: ndcg_at_10
      value: 67.596
    - type: ndcg_at_100
      value: 69.95
    - type: ndcg_at_1000
      value: 70.33500000000001
    - type: ndcg_at_3
      value: 62.82600000000001
    - type: ndcg_at_5
      value: 65.546
    - type: precision_at_1
      value: 52.1
    - type: precision_at_10
      value: 8.309999999999999
    - type: precision_at_100
      value: 0.941
    - type: precision_at_1000
      value: 0.097
    - type: precision_at_3
      value: 23.400000000000002
    - type: precision_at_5
      value: 15.36
    - type: recall_at_1
      value: 52.1
    - type: recall_at_10
      value: 83.1
    - type: recall_at_100
      value: 94.1
    - type: recall_at_1000
      value: 97.0
    - type: recall_at_3
      value: 70.19999999999999
    - type: recall_at_5
      value: 76.8
  - task:
      type: Classification
    dataset:
      type: C-MTEB/IFlyTek-classification
      name: MTEB IFlyTek
      config: default
      split: validation
      revision: 421605374b29664c5fc098418fe20ada9bd55f8a
    metrics:
    - type: accuracy
      value: 51.773759138130046
    - type: f1
      value: 40.341407912920054
  - task:
      type: Classification
    dataset:
      type: C-MTEB/JDReview-classification
      name: MTEB JDReview
      config: default
      split: test
      revision: b7c64bd89eb87f8ded463478346f76731f07bf8b
    metrics:
    - type: accuracy
      value: 86.69793621013133
    - type: ap
      value: 55.46718958939327
    - type: f1
      value: 81.48228915952436
  - task:
      type: STS
    dataset:
      type: C-MTEB/LCQMC
      name: MTEB LCQMC
      config: default
      split: test
      revision: 17f9b096f80380fce5ed12a9be8be7784b337daf
    metrics:
    - type: cos_sim_pearson
      value: 71.1397780205448
    - type: cos_sim_spearman
      value: 78.17368193033309
    - type: euclidean_pearson
      value: 77.4849177602368
    - type: euclidean_spearman
      value: 78.17369079663212
    - type: manhattan_pearson
      value: 77.47344305182406
    - type: manhattan_spearman
      value: 78.16454335155387
  - task:
      type: Reranking
    dataset:
      type: C-MTEB/Mmarco-reranking
      name: MTEB MMarcoReranking
      config: default
      split: dev
      revision: 8e0c766dbe9e16e1d221116a3f36795fbade07f6
    metrics:
    - type: map
      value: 27.76160559006673
    - type: mrr
      value: 28.02420634920635
  - task:
      type: Retrieval
    dataset:
      type: C-MTEB/MMarcoRetrieval
      name: MTEB MMarcoRetrieval
      config: default
      split: dev
      revision: 539bbde593d947e2a124ba72651aafc09eb33fc2
    metrics:
    - type: map_at_1
      value: 65.661
    - type: map_at_10
      value: 74.752
    - type: map_at_100
      value: 75.091
    - type: map_at_1000
      value: 75.104
    - type: map_at_3
      value: 72.997
    - type: map_at_5
      value: 74.119
    - type: mrr_at_1
      value: 67.923
    - type: mrr_at_10
      value: 75.376
    - type: mrr_at_100
      value: 75.673
    - type: mrr_at_1000
      value: 75.685
    - type: mrr_at_3
      value: 73.856
    - type: mrr_at_5
      value: 74.82799999999999
    - type: ndcg_at_1
      value: 67.923
    - type: ndcg_at_10
      value: 78.424
    - type: ndcg_at_100
      value: 79.95100000000001
    - type: ndcg_at_1000
      value: 80.265
    - type: ndcg_at_3
      value: 75.101
    - type: ndcg_at_5
      value: 76.992
    - type: precision_at_1
      value: 67.923
    - type: precision_at_10
      value: 9.474
    - type: precision_at_100
      value: 1.023
    - type: precision_at_1000
      value: 0.105
    - type: precision_at_3
      value: 28.319
    - type: precision_at_5
      value: 17.986
    - type: recall_at_1
      value: 65.661
    - type: recall_at_10
      value: 89.09899999999999
    - type: recall_at_100
      value: 96.023
    - type: recall_at_1000
      value: 98.455
    - type: recall_at_3
      value: 80.314
    - type: recall_at_5
      value: 84.81
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (zh-CN)
      config: zh-CN
      split: test
      revision: 31efe3c427b0bae9c22cbb560b8f15491cc6bed7
    metrics:
    - type: accuracy
      value: 75.86751849361131
    - type: f1
      value: 73.04918450508
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (zh-CN)
      config: zh-CN
      split: test
      revision: 7d571f92784cd94a019292a1f45445077d0ef634
    metrics:
    - type: accuracy
      value: 78.4364492266308
    - type: f1
      value: 78.120686034844
  - task:
      type: Retrieval
    dataset:
      type: C-MTEB/MedicalRetrieval
      name: MTEB MedicalRetrieval
      config: default
      split: dev
      revision: 2039188fb5800a9803ba5048df7b76e6fb151fc6
    metrics:
    - type: map_at_1
      value: 55.00000000000001
    - type: map_at_10
      value: 61.06399999999999
    - type: map_at_100
      value: 61.622
    - type: map_at_1000
      value: 61.663000000000004
    - type: map_at_3
      value: 59.583
    - type: map_at_5
      value: 60.373
    - type: mrr_at_1
      value: 55.2
    - type: mrr_at_10
      value: 61.168
    - type: mrr_at_100
      value: 61.726000000000006
    - type: mrr_at_1000
      value: 61.767
    - type: mrr_at_3
      value: 59.683
    - type: mrr_at_5
      value: 60.492999999999995
    - type: ndcg_at_1
      value: 55.00000000000001
    - type: ndcg_at_10
      value: 64.098
    - type: ndcg_at_100
      value: 67.05
    - type: ndcg_at_1000
      value: 68.262
    - type: ndcg_at_3
      value: 61.00600000000001
    - type: ndcg_at_5
      value: 62.439
    - type: precision_at_1
      value: 55.00000000000001
    - type: precision_at_10
      value: 7.37
    - type: precision_at_100
      value: 0.881
    - type: precision_at_1000
      value: 0.098
    - type: precision_at_3
      value: 21.7
    - type: precision_at_5
      value: 13.719999999999999
    - type: recall_at_1
      value: 55.00000000000001
    - type: recall_at_10
      value: 73.7
    - type: recall_at_100
      value: 88.1
    - type: recall_at_1000
      value: 97.8
    - type: recall_at_3
      value: 65.10000000000001
    - type: recall_at_5
      value: 68.60000000000001
  - task:
      type: Classification
    dataset:
      type: C-MTEB/MultilingualSentiment-classification
      name: MTEB MultilingualSentiment
      config: default
      split: validation
      revision: 46958b007a63fdbf239b7672c25d0bea67b5ea1a
    metrics:
    - type: accuracy
      value: 77.52666666666667
    - type: f1
      value: 77.49784731367215
  - task:
      type: PairClassification
    dataset:
      type: C-MTEB/OCNLI
      name: MTEB Ocnli
      config: default
      split: validation
      revision: 66e76a618a34d6d565d5538088562851e6daa7ec
    metrics:
    - type: cos_sim_accuracy
      value: 81.10449377368705
    - type: cos_sim_ap
      value: 85.17742765935606
    - type: cos_sim_f1
      value: 83.00094966761633
    - type: cos_sim_precision
      value: 75.40983606557377
    - type: cos_sim_recall
      value: 92.29144667370645
    - type: dot_accuracy
      value: 81.10449377368705
    - type: dot_ap
      value: 85.17143850809614
    - type: dot_f1
      value: 83.01707779886148
    - type: dot_precision
      value: 75.36606373815677
    - type: dot_recall
      value: 92.39704329461456
    - type: euclidean_accuracy
      value: 81.10449377368705
    - type: euclidean_ap
      value: 85.17856775343333
    - type: euclidean_f1
      value: 83.00094966761633
    - type: euclidean_precision
      value: 75.40983606557377
    - type: euclidean_recall
      value: 92.29144667370645
    - type: manhattan_accuracy
      value: 81.05035192203573
    - type: manhattan_ap
      value: 85.14464459395809
    - type: manhattan_f1
      value: 82.96155671570953
    - type: manhattan_precision
      value: 75.3448275862069
    - type: manhattan_recall
      value: 92.29144667370645
    - type: max_accuracy
      value: 81.10449377368705
    - type: max_ap
      value: 85.17856775343333
    - type: max_f1
      value: 83.01707779886148
  - task:
      type: Classification
    dataset:
      type: C-MTEB/OnlineShopping-classification
      name: MTEB OnlineShopping
      config: default
      split: test
      revision: e610f2ebd179a8fda30ae534c3878750a96db120
    metrics:
    - type: accuracy
      value: 93.71000000000001
    - type: ap
      value: 91.83202232349356
    - type: f1
      value: 93.69900560334331
  - task:
      type: STS
    dataset:
      type: C-MTEB/PAWSX
      name: MTEB PAWSX
      config: default
      split: test
      revision: 9c6a90e430ac22b5779fb019a23e820b11a8b5e1
    metrics:
    - type: cos_sim_pearson
      value: 39.175047651512415
    - type: cos_sim_spearman
      value: 45.51434675777896
    - type: euclidean_pearson
      value: 44.864110004132286
    - type: euclidean_spearman
      value: 45.516433048896076
    - type: manhattan_pearson
      value: 44.87153627706517
    - type: manhattan_spearman
      value: 45.52862617925012
  - task:
      type: STS
    dataset:
      type: C-MTEB/QBQTC
      name: MTEB QBQTC
      config: default
      split: test
      revision: 790b0510dc52b1553e8c49f3d2afb48c0e5c48b7
    metrics:
    - type: cos_sim_pearson
      value: 34.249579701429084
    - type: cos_sim_spearman
      value: 37.30903127368978
    - type: euclidean_pearson
      value: 35.129438425253355
    - type: euclidean_spearman
      value: 37.308544018709085
    - type: manhattan_pearson
      value: 35.08936153503652
    - type: manhattan_spearman
      value: 37.25582901077839
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (zh)
      config: zh
      split: test
      revision: eea2b4fe26a775864c896887d910b76a8098ad3f
    metrics:
    - type: cos_sim_pearson
      value: 61.29309637460004
    - type: cos_sim_spearman
      value: 65.85136090376717
    - type: euclidean_pearson
      value: 64.04783990953557
    - type: euclidean_spearman
      value: 65.85036859610366
    - type: manhattan_pearson
      value: 63.995852552712186
    - type: manhattan_spearman
      value: 65.86508416749417
  - task:
      type: STS
    dataset:
      type: C-MTEB/STSB
      name: MTEB STSB
      config: default
      split: test
      revision: 0cde68302b3541bb8b3c340dc0644b0b745b3dc0
    metrics:
    - type: cos_sim_pearson
      value: 81.5595940455587
    - type: cos_sim_spearman
      value: 82.72654634579749
    - type: euclidean_pearson
      value: 82.4892721061365
    - type: euclidean_spearman
      value: 82.72678504228253
    - type: manhattan_pearson
      value: 82.4770861422454
    - type: manhattan_spearman
      value: 82.71137469783162
  - task:
      type: Reranking
    dataset:
      type: C-MTEB/T2Reranking
      name: MTEB T2Reranking
      config: default
      split: dev
      revision: 76631901a18387f85eaa53e5450019b87ad58ef9
    metrics:
    - type: map
      value: 66.6159547610527
    - type: mrr
      value: 76.35739406347057
  - task:
      type: Retrieval
    dataset:
      type: C-MTEB/T2Retrieval
      name: MTEB T2Retrieval
      config: default
      split: dev
      revision: 8731a845f1bf500a4f111cf1070785c793d10e64
    metrics:
    - type: map_at_1
      value: 27.878999999999998
    - type: map_at_10
      value: 77.517
    - type: map_at_100
      value: 81.139
    - type: map_at_1000
      value: 81.204
    - type: map_at_3
      value: 54.728
    - type: map_at_5
      value: 67.128
    - type: mrr_at_1
      value: 90.509
    - type: mrr_at_10
      value: 92.964
    - type: mrr_at_100
      value: 93.045
    - type: mrr_at_1000
      value: 93.048
    - type: mrr_at_3
      value: 92.551
    - type: mrr_at_5
      value: 92.81099999999999
    - type: ndcg_at_1
      value: 90.509
    - type: ndcg_at_10
      value: 85.075
    - type: ndcg_at_100
      value: 88.656
    - type: ndcg_at_1000
      value: 89.25699999999999
    - type: ndcg_at_3
      value: 86.58200000000001
    - type: ndcg_at_5
      value: 85.138
    - type: precision_at_1
      value: 90.509
    - type: precision_at_10
      value: 42.05
    - type: precision_at_100
      value: 5.013999999999999
    - type: precision_at_1000
      value: 0.516
    - type: precision_at_3
      value: 75.551
    - type: precision_at_5
      value: 63.239999999999995
    - type: recall_at_1
      value: 27.878999999999998
    - type: recall_at_10
      value: 83.941
    - type: recall_at_100
      value: 95.568
    - type: recall_at_1000
      value: 98.55000000000001
    - type: recall_at_3
      value: 56.374
    - type: recall_at_5
      value: 70.435
  - task:
      type: Classification
    dataset:
      type: C-MTEB/TNews-classification
      name: MTEB TNews
      config: default
      split: validation
      revision: 317f262bf1e6126357bbe89e875451e4b0938fe4
    metrics:
    - type: accuracy
      value: 53.687
    - type: f1
      value: 51.86911933364655
  - task:
      type: Clustering
    dataset:
      type: C-MTEB/ThuNewsClusteringP2P
      name: MTEB ThuNewsClusteringP2P
      config: default
      split: test
      revision: 5798586b105c0434e4f0fe5e767abe619442cf93
    metrics:
    - type: v_measure
      value: 74.65887489872564
  - task:
      type: Clustering
    dataset:
      type: C-MTEB/ThuNewsClusteringS2S
      name: MTEB ThuNewsClusteringS2S
      config: default
      split: test
      revision: 8a8b2caeda43f39e13c4bc5bea0f8a667896e10d
    metrics:
    - type: v_measure
      value: 69.00410995984436
  - task:
      type: Retrieval
    dataset:
      type: C-MTEB/VideoRetrieval
      name: MTEB VideoRetrieval
      config: default
      split: dev
      revision: 58c2597a5943a2ba48f4668c3b90d796283c5639
    metrics:
    - type: map_at_1
      value: 59.4
    - type: map_at_10
      value: 69.214
    - type: map_at_100
      value: 69.72699999999999
    - type: map_at_1000
      value: 69.743
    - type: map_at_3
      value: 67.717
    - type: map_at_5
      value: 68.782
    - type: mrr_at_1
      value: 59.4
    - type: mrr_at_10
      value: 69.214
    - type: mrr_at_100
      value: 69.72699999999999
    - type: mrr_at_1000
      value: 69.743
    - type: mrr_at_3
      value: 67.717
    - type: mrr_at_5
      value: 68.782
    - type: ndcg_at_1
      value: 59.4
    - type: ndcg_at_10
      value: 73.32300000000001
    - type: ndcg_at_100
      value: 75.591
    - type: ndcg_at_1000
      value: 75.98700000000001
    - type: ndcg_at_3
      value: 70.339
    - type: ndcg_at_5
      value: 72.246
    - type: precision_at_1
      value: 59.4
    - type: precision_at_10
      value: 8.59
    - type: precision_at_100
      value: 0.96
    - type: precision_at_1000
      value: 0.099
    - type: precision_at_3
      value: 25.967000000000002
    - type: precision_at_5
      value: 16.5
    - type: recall_at_1
      value: 59.4
    - type: recall_at_10
      value: 85.9
    - type: recall_at_100
      value: 96.0
    - type: recall_at_1000
      value: 99.1
    - type: recall_at_3
      value: 77.9
    - type: recall_at_5
      value: 82.5
  - task:
      type: Classification
    dataset:
      type: C-MTEB/waimai-classification
      name: MTEB Waimai
      config: default
      split: test
      revision: 339287def212450dcaa9df8c22bf93e9980c7023
    metrics:
    - type: accuracy
      value: 88.53
    - type: ap
      value: 73.56216166534062
    - type: f1
      value: 87.06093694294485
---

<div align="center">
<img src="./img/logo.png" alt="icon" width="300px"/>
</div>



## acge model

acge模型来自于[合合信息](https://www.intsig.com/)技术团队，对外技术试用平台[TextIn](https://www.textin.com/)。合合信息是行业领先的人工智能及大数据科技企业，致力于通过智能文字识别及商业大数据领域的核心技术、C端和B端产品以及行业解决方案为全球企业和个人用户提供创新的数字化、智能化服务。

技术交流请联系<yanhui_he@intsig.net>，商务合作请联系<simon_liu@intsig.net>，可以[点击图片](https://huggingface.co/aspire/acge_text_embedding/blob/main/img/wx.jpg)，扫面二维码来加入我们的微信社群。

acge是一个通用的文本编码模型，是一个可变长度的向量化模型，使用了[Matryoshka Representation Learning](https://arxiv.org/abs/2205.13147)，如图所示：

![matryoshka-small](./img/matryoshka-small.gif)

建议使用的维度为1024或者1792


|     Model Name     | Model Size (GB) | Dimension | Sequence Length | Language | Need instruction for retrieval? |
|:------------------:|:---------------:|:---------:|:---------------:|:--------:|:-------------------------------:|
|  acge-text-embedding   |      0.65       |   [1024, 1792]    |      1024       | Chinese  |               NO               |


## Metric

#### C-MTEB leaderboard (Chinese)

测试的时候因为数据的随机性、显卡、推理的数据类型导致每次推理的结果不一致，我总共测试了4次，不同的显卡(A10 A100)，不同的数据类型，测试结果放在了result文件夹中，选取了一个精度最低的测试作为最终的精度测试。
根据[infgrad](https://huggingface.co/infgrad)的建议，选取不用的输入的长度作为测试，Sequence Length为512时测试最佳。

|     Model Name     | GPU | tensor-type | Model Size (GB) | Dimension | Sequence Length | Average (35) | Classification (9) | Clustering (4) | Pair Classification (2) | Reranking (4) | Retrieval (8) | STS (8) |
|:------------------:|:---------------:|:---------:|:---------------:|:------------:|:------------------:|:--------------:|:-----------------------:|:-------------:|:-------------:|:-------:|:-------:|:-------:|
| acge_text_embedding | NVIDIA TESLA A10 | bfloat16 | 0.65 |   1792   |      1024       |    68.91    |       72.76       |     58.22 |     87.82   | 67.67  |  72.48 |  62.24  |
| acge_text_embedding | NVIDIA TESLA A100 | bfloat16 | 0.65 | 1792 | 1024  |    68.91 |       72.77 |  58.35 |    87.82  |  67.53   |     72.48     |  62.24  |
| acge_text_embedding | NVIDIA TESLA A100 | float16 | 0.65 | 1792 | 1024 | 68.99 | 72.76 | 58.68 | 87.84 | 67.89 | 72.49 | 62.24 |
| acge_text_embedding | NVIDIA TESLA A100 | float32 | 0.65 | 1792 | 1024 | 68.98 | 72.76 | 58.58 | 87.83 | 67.91 | 72.49 | 62.24 |
| acge_text_embedding | NVIDIA TESLA A100 | float16 | 0.65 | 1792 | 768  | 68.95 | 72.76 | 58.68 | 87.84 | 67.86 | 72.48 | 62.07 |
| acge_text_embedding | NVIDIA TESLA A100 | float16 | 0.65 | 1792 | 512  | 69.07 | 72.75 | 58.7  | 87.84 | 67.99 | 72.93 | 62.09 |

#### Reproduce our results

**C-MTEB:** 

```python
import torch
import argparse
import functools
from C_MTEB.tasks import *
from typing import List, Dict
from sentence_transformers import SentenceTransformer
from mteb import MTEB, DRESModel


class RetrievalModel(DRESModel):
    def __init__(self, encoder, **kwargs):
        self.encoder = encoder

    def encode_queries(self, queries: List[str], **kwargs) -> np.ndarray:
        input_texts = ['{}'.format(q) for q in queries]
        return self._do_encode(input_texts)

    def encode_corpus(self, corpus: List[Dict[str, str]], **kwargs) -> np.ndarray:
        input_texts = ['{} {}'.format(doc.get('title', ''), doc['text']).strip() for doc in corpus]
        input_texts = ['{}'.format(t) for t in input_texts]
        return self._do_encode(input_texts)

    @torch.no_grad()
    def _do_encode(self, input_texts: List[str]) -> np.ndarray:
        return self.encoder.encode(
            sentences=input_texts,
            batch_size=512,
            normalize_embeddings=True,
            convert_to_numpy=True
        )


def get_args():
    parser = argparse.ArgumentParser()
    parser.add_argument('--model_name_or_path', default="acge_text_embedding", type=str)
    parser.add_argument('--task_type', default=None, type=str)
    parser.add_argument('--pooling_method', default='cls', type=str)
    parser.add_argument('--output_dir', default='zh_results',
                        type=str, help='output directory')
    parser.add_argument('--max_len', default=1024, type=int, help='max length')
    return parser.parse_args()


if __name__ == '__main__':
    args = get_args()
    encoder = SentenceTransformer(args.model_name_or_path).half()
    encoder.encode = functools.partial(encoder.encode, normalize_embeddings=True)
    encoder.max_seq_length = int(args.max_len)

    task_names = [t.description["name"] for t in MTEB(task_types=args.task_type,
                                                      task_langs=['zh', 'zh-CN']).tasks]
    TASKS_WITH_PROMPTS = ["T2Retrieval", "MMarcoRetrieval", "DuRetrieval", "CovidRetrieval", "CmedqaRetrieval",
                          "EcomRetrieval", "MedicalRetrieval", "VideoRetrieval"]
    for task in task_names:
        evaluation = MTEB(tasks=[task], task_langs=['zh', 'zh-CN'])
        if task in TASKS_WITH_PROMPTS:
            evaluation.run(RetrievalModel(encoder), output_folder=args.output_dir, overwrite_results=False)
        else:
            evaluation.run(encoder, output_folder=args.output_dir, overwrite_results=False)


```


## Usage

#### acge 中文系列模型

在sentence-transformer库中的使用方法：

```python
from sentence_transformers import SentenceTransformer

sentences = ["数据1", "数据2"]
model = SentenceTransformer('acge_text_embedding')
print(model.max_seq_length)
embeddings_1 = model.encode(sentences, normalize_embeddings=True)
embeddings_2 = model.encode(sentences, normalize_embeddings=True)
similarity = embeddings_1 @ embeddings_2.T
print(similarity)
```
在sentence-transformer库中的使用方法，选取不同的维度：

```python
from sklearn.preprocessing import normalize
from sentence_transformers import SentenceTransformer

sentences = ["数据1", "数据2"]
model = SentenceTransformer('acge_text_embedding')
embeddings = model.encode(sentences, normalize_embeddings=False)
matryoshka_dim = 1024
embeddings = embeddings[..., :matryoshka_dim]  # Shrink the embedding dimensions
embeddings = normalize(embeddings, norm="l2", axis=1)
print(embeddings.shape)
# => (2, 1024)

```




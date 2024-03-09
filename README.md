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
      value: 54.03219651150428
    - type: cos_sim_spearman
      value: 58.80567952355933
    - type: euclidean_pearson
      value: 57.47052075207808
    - type: euclidean_spearman
      value: 58.80429232297114
    - type: manhattan_pearson
      value: 57.46163912433917
    - type: manhattan_spearman
      value: 58.797778532121
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
      value: 53.523171963746854
    - type: cos_sim_spearman
      value: 57.94610819724817
    - type: euclidean_pearson
      value: 61.16974418403869
    - type: euclidean_spearman
      value: 57.94681861980281
    - type: manhattan_pearson
      value: 61.167825359334515
    - type: manhattan_spearman
      value: 57.94540903298445
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
      value: 48.556
    - type: f1
      value: 46.61852566163211
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
      value: 68.26963267181252
    - type: cos_sim_spearman
      value: 70.36696156869363
    - type: euclidean_pearson
      value: 69.42591718370763
    - type: euclidean_spearman
      value: 70.3677583116469
    - type: manhattan_pearson
      value: 69.40127857737215
    - type: manhattan_spearman
      value: 70.34572662526428
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
      value: 46.54685387179774
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
      value: 44.45602575811581
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
      value: 88.4576468720639
    - type: mrr
      value: 90.90595238095237
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
      value: 88.71413673867269
    - type: mrr
      value: 91.19265873015873
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
      value: 26.825
    - type: map_at_10
      value: 39.959
    - type: map_at_100
      value: 41.861
    - type: map_at_1000
      value: 41.963
    - type: map_at_3
      value: 35.357
    - type: map_at_5
      value: 38.001000000000005
    - type: mrr_at_1
      value: 40.585
    - type: mrr_at_10
      value: 48.802
    - type: mrr_at_100
      value: 49.779
    - type: mrr_at_1000
      value: 49.819
    - type: mrr_at_3
      value: 46.095000000000006
    - type: mrr_at_5
      value: 47.678
    - type: ndcg_at_1
      value: 40.585
    - type: ndcg_at_10
      value: 46.758
    - type: ndcg_at_100
      value: 53.957
    - type: ndcg_at_1000
      value: 55.656000000000006
    - type: ndcg_at_3
      value: 40.961
    - type: ndcg_at_5
      value: 43.564
    - type: precision_at_1
      value: 40.585
    - type: precision_at_10
      value: 10.424999999999999
    - type: precision_at_100
      value: 1.625
    - type: precision_at_1000
      value: 0.184
    - type: precision_at_3
      value: 23.114
    - type: precision_at_5
      value: 17.024
    - type: recall_at_1
      value: 26.825
    - type: recall_at_10
      value: 57.909
    - type: recall_at_100
      value: 87.375
    - type: recall_at_1000
      value: 98.695
    - type: recall_at_3
      value: 40.754000000000005
    - type: recall_at_5
      value: 48.472
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
      value: 83.4155141310884
    - type: cos_sim_ap
      value: 90.49006000181046
    - type: cos_sim_f1
      value: 84.28797826579125
    - type: cos_sim_precision
      value: 81.69848584595128
    - type: cos_sim_recall
      value: 87.04699555763385
    - type: dot_accuracy
      value: 83.40348767288035
    - type: dot_ap
      value: 90.50667776818787
    - type: dot_f1
      value: 84.31853669417802
    - type: dot_precision
      value: 80.61420345489442
    - type: dot_recall
      value: 88.379705400982
    - type: euclidean_accuracy
      value: 83.43956704750451
    - type: euclidean_ap
      value: 90.48869698176196
    - type: euclidean_f1
      value: 84.32616081540203
    - type: euclidean_precision
      value: 81.77026136613222
    - type: euclidean_recall
      value: 87.04699555763385
    - type: manhattan_accuracy
      value: 83.55983162958509
    - type: manhattan_ap
      value: 90.47972486190912
    - type: manhattan_f1
      value: 84.42325158946412
    - type: manhattan_precision
      value: 82.0569410726109
    - type: manhattan_recall
      value: 86.93009118541033
    - type: max_accuracy
      value: 83.55983162958509
    - type: max_ap
      value: 90.50667776818787
    - type: max_f1
      value: 84.42325158946412
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
      value: 67.597
    - type: map_at_10
      value: 76.545
    - type: map_at_100
      value: 76.893
    - type: map_at_1000
      value: 76.897
    - type: map_at_3
      value: 74.807
    - type: map_at_5
      value: 75.895
    - type: mrr_at_1
      value: 67.861
    - type: mrr_at_10
      value: 76.545
    - type: mrr_at_100
      value: 76.893
    - type: mrr_at_1000
      value: 76.897
    - type: mrr_at_3
      value: 74.886
    - type: mrr_at_5
      value: 75.934
    - type: ndcg_at_1
      value: 67.861
    - type: ndcg_at_10
      value: 80.417
    - type: ndcg_at_100
      value: 81.928
    - type: ndcg_at_1000
      value: 82.038
    - type: ndcg_at_3
      value: 77.025
    - type: ndcg_at_5
      value: 78.94099999999999
    - type: precision_at_1
      value: 67.861
    - type: precision_at_10
      value: 9.336
    - type: precision_at_100
      value: 1.001
    - type: precision_at_1000
      value: 0.101
    - type: precision_at_3
      value: 27.959
    - type: precision_at_5
      value: 17.745
    - type: recall_at_1
      value: 67.597
    - type: recall_at_10
      value: 92.308
    - type: recall_at_100
      value: 99.05199999999999
    - type: recall_at_1000
      value: 99.895
    - type: recall_at_3
      value: 83.325
    - type: recall_at_5
      value: 87.908
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
      value: 25.574
    - type: map_at_10
      value: 78.493
    - type: map_at_100
      value: 81.384
    - type: map_at_1000
      value: 81.429
    - type: map_at_3
      value: 54.107000000000006
    - type: map_at_5
      value: 68.755
    - type: mrr_at_1
      value: 89.2
    - type: mrr_at_10
      value: 92.567
    - type: mrr_at_100
      value: 92.642
    - type: mrr_at_1000
      value: 92.646
    - type: mrr_at_3
      value: 92.258
    - type: mrr_at_5
      value: 92.458
    - type: ndcg_at_1
      value: 89.2
    - type: ndcg_at_10
      value: 86.084
    - type: ndcg_at_100
      value: 89.053
    - type: ndcg_at_1000
      value: 89.484
    - type: ndcg_at_3
      value: 84.898
    - type: ndcg_at_5
      value: 84.078
    - type: precision_at_1
      value: 89.2
    - type: precision_at_10
      value: 41.345
    - type: precision_at_100
      value: 4.779
    - type: precision_at_1000
      value: 0.488
    - type: precision_at_3
      value: 76.167
    - type: precision_at_5
      value: 64.7
    - type: recall_at_1
      value: 25.574
    - type: recall_at_10
      value: 87.153
    - type: recall_at_100
      value: 96.829
    - type: recall_at_1000
      value: 99.11999999999999
    - type: recall_at_3
      value: 56.421
    - type: recall_at_5
      value: 73.7
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
      value: 52.0
    - type: map_at_10
      value: 62.553000000000004
    - type: map_at_100
      value: 63.048
    - type: map_at_1000
      value: 63.065000000000005
    - type: map_at_3
      value: 60.233000000000004
    - type: map_at_5
      value: 61.712999999999994
    - type: mrr_at_1
      value: 52.0
    - type: mrr_at_10
      value: 62.553000000000004
    - type: mrr_at_100
      value: 63.048
    - type: mrr_at_1000
      value: 63.065000000000005
    - type: mrr_at_3
      value: 60.233000000000004
    - type: mrr_at_5
      value: 61.712999999999994
    - type: ndcg_at_1
      value: 52.0
    - type: ndcg_at_10
      value: 67.51599999999999
    - type: ndcg_at_100
      value: 69.896
    - type: ndcg_at_1000
      value: 70.281
    - type: ndcg_at_3
      value: 62.82600000000001
    - type: ndcg_at_5
      value: 65.498
    - type: precision_at_1
      value: 52.0
    - type: precision_at_10
      value: 8.3
    - type: precision_at_100
      value: 0.941
    - type: precision_at_1000
      value: 0.097
    - type: precision_at_3
      value: 23.433
    - type: precision_at_5
      value: 15.36
    - type: recall_at_1
      value: 52.0
    - type: recall_at_10
      value: 83.0
    - type: recall_at_100
      value: 94.1
    - type: recall_at_1000
      value: 97.0
    - type: recall_at_3
      value: 70.3
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
      value: 51.76606387071951
    - type: f1
      value: 40.25725744367441
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
      value: 71.13755846688528
    - type: cos_sim_spearman
      value: 78.17322744116031
    - type: euclidean_pearson
      value: 77.48740502819294
    - type: euclidean_spearman
      value: 78.17553979551616
    - type: manhattan_pearson
      value: 77.47671561749276
    - type: manhattan_spearman
      value: 78.16780681181362
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
      value: 27.054392822906316
    - type: mrr
      value: 29.001190476190473
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
      value: 65.62599999999999
    - type: map_at_10
      value: 74.749
    - type: map_at_100
      value: 75.091
    - type: map_at_1000
      value: 75.103
    - type: map_at_3
      value: 73.007
    - type: map_at_5
      value: 74.124
    - type: mrr_at_1
      value: 67.894
    - type: mrr_at_10
      value: 75.374
    - type: mrr_at_100
      value: 75.67399999999999
    - type: mrr_at_1000
      value: 75.685
    - type: mrr_at_3
      value: 73.868
    - type: mrr_at_5
      value: 74.83
    - type: ndcg_at_1
      value: 67.894
    - type: ndcg_at_10
      value: 78.414
    - type: ndcg_at_100
      value: 79.947
    - type: ndcg_at_1000
      value: 80.265
    - type: ndcg_at_3
      value: 75.12
    - type: ndcg_at_5
      value: 76.999
    - type: precision_at_1
      value: 67.894
    - type: precision_at_10
      value: 9.47
    - type: precision_at_100
      value: 1.023
    - type: precision_at_1000
      value: 0.105
    - type: precision_at_3
      value: 28.333000000000002
    - type: precision_at_5
      value: 17.989
    - type: recall_at_1
      value: 65.62599999999999
    - type: recall_at_10
      value: 89.063
    - type: recall_at_100
      value: 95.99499999999999
    - type: recall_at_1000
      value: 98.455
    - type: recall_at_3
      value: 80.357
    - type: recall_at_5
      value: 84.824
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
      value: 75.88433086751849
    - type: f1
      value: 73.06801290283882
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
      value: 78.44317417619366
    - type: f1
      value: 78.1407925250533
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
      value: 54.900000000000006
    - type: map_at_10
      value: 61.0
    - type: map_at_100
      value: 61.549
    - type: map_at_1000
      value: 61.590999999999994
    - type: map_at_3
      value: 59.516999999999996
    - type: map_at_5
      value: 60.267
    - type: mrr_at_1
      value: 55.1
    - type: mrr_at_10
      value: 61.1
    - type: mrr_at_100
      value: 61.649
    - type: mrr_at_1000
      value: 61.690999999999995
    - type: mrr_at_3
      value: 59.617
    - type: mrr_at_5
      value: 60.367000000000004
    - type: ndcg_at_1
      value: 54.900000000000006
    - type: ndcg_at_10
      value: 64.07000000000001
    - type: ndcg_at_100
      value: 66.981
    - type: ndcg_at_1000
      value: 68.207
    - type: ndcg_at_3
      value: 60.955999999999996
    - type: ndcg_at_5
      value: 62.31100000000001
    - type: precision_at_1
      value: 54.900000000000006
    - type: precision_at_10
      value: 7.380000000000001
    - type: precision_at_100
      value: 0.88
    - type: precision_at_1000
      value: 0.098
    - type: precision_at_3
      value: 21.7
    - type: precision_at_5
      value: 13.68
    - type: recall_at_1
      value: 54.900000000000006
    - type: recall_at_10
      value: 73.8
    - type: recall_at_100
      value: 88.0
    - type: recall_at_1000
      value: 97.8
    - type: recall_at_3
      value: 65.10000000000001
    - type: recall_at_5
      value: 68.4
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
      value: 77.56333333333333
    - type: f1
      value: 77.53666660124703
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
      value: 85.16141108141811
    - type: cos_sim_f1
      value: 82.97771455666192
    - type: cos_sim_precision
      value: 75.30120481927712
    - type: cos_sim_recall
      value: 92.39704329461456
    - type: dot_accuracy
      value: 81.05035192203573
    - type: dot_ap
      value: 85.13568069803823
    - type: dot_f1
      value: 83.04038004750595
    - type: dot_precision
      value: 75.47495682210709
    - type: dot_recall
      value: 92.29144667370645
    - type: euclidean_accuracy
      value: 81.10449377368705
    - type: euclidean_ap
      value: 85.16341835376645
    - type: euclidean_f1
      value: 82.96860133206471
    - type: euclidean_precision
      value: 75.4978354978355
    - type: euclidean_recall
      value: 92.08025343189018
    - type: manhattan_accuracy
      value: 81.15863562533838
    - type: manhattan_ap
      value: 85.13388548299352
    - type: manhattan_f1
      value: 82.91048348492102
    - type: manhattan_precision
      value: 75.83187390542906
    - type: manhattan_recall
      value: 91.4466737064414
    - type: max_accuracy
      value: 81.15863562533838
    - type: max_ap
      value: 85.16341835376645
    - type: max_f1
      value: 83.04038004750595
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
      value: 93.75
    - type: ap
      value: 91.8757063139003
    - type: f1
      value: 93.73901896028437
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
      value: 39.15831534609524
    - type: cos_sim_spearman
      value: 45.4969633673045
    - type: euclidean_pearson
      value: 44.848515043386826
    - type: euclidean_spearman
      value: 45.50184060659851
    - type: manhattan_pearson
      value: 44.855618769134786
    - type: manhattan_spearman
      value: 45.521349632021
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
      value: 34.240063381471685
    - type: cos_sim_spearman
      value: 37.29810568951238
    - type: euclidean_pearson
      value: 35.114630288288694
    - type: euclidean_spearman
      value: 37.29224953963422
    - type: manhattan_pearson
      value: 35.07429582481541
    - type: manhattan_spearman
      value: 37.24006222876743
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
      value: 61.839386292911634
    - type: cos_sim_spearman
      value: 67.05632097771566
    - type: euclidean_pearson
      value: 65.72031356075829
    - type: euclidean_spearman
      value: 67.05823973191457
    - type: manhattan_pearson
      value: 65.66073527177826
    - type: manhattan_spearman
      value: 67.04221791481658
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
      value: 81.56195178204662
    - type: cos_sim_spearman
      value: 82.73033434099031
    - type: euclidean_pearson
      value: 82.49605254478311
    - type: euclidean_spearman
      value: 82.72004995354247
    - type: manhattan_pearson
      value: 82.48358662476731
    - type: manhattan_spearman
      value: 82.70676710419983
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
      value: 65.9012655137193
    - type: mrr
      value: 75.97216177150165
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
      value: 27.057
    - type: map_at_10
      value: 75.29299999999999
    - type: map_at_100
      value: 79.098
    - type: map_at_1000
      value: 79.172
    - type: map_at_3
      value: 53.049
    - type: map_at_5
      value: 65.103
    - type: mrr_at_1
      value: 88.822
    - type: mrr_at_10
      value: 91.721
    - type: mrr_at_100
      value: 91.814
    - type: mrr_at_1000
      value: 91.818
    - type: mrr_at_3
      value: 91.213
    - type: mrr_at_5
      value: 91.544
    - type: ndcg_at_1
      value: 88.822
    - type: ndcg_at_10
      value: 83.269
    - type: ndcg_at_100
      value: 87.259
    - type: ndcg_at_1000
      value: 87.938
    - type: ndcg_at_3
      value: 84.678
    - type: ndcg_at_5
      value: 83.231
    - type: precision_at_1
      value: 88.822
    - type: precision_at_10
      value: 41.297
    - type: precision_at_100
      value: 4.994
    - type: precision_at_1000
      value: 0.515
    - type: precision_at_3
      value: 73.933
    - type: precision_at_5
      value: 61.885
    - type: recall_at_1
      value: 27.057
    - type: recall_at_10
      value: 82.33200000000001
    - type: recall_at_100
      value: 95.065
    - type: recall_at_1000
      value: 98.466
    - type: recall_at_3
      value: 54.872
    - type: recall_at_5
      value: 68.814
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
      value: 53.690000000000005
    - type: f1
      value: 51.87306088948137
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
      value: 73.76590442198115
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
      value: 68.61875345658028
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
      value: 69.19
    - type: map_at_100
      value: 69.711
    - type: map_at_1000
      value: 69.72699999999999
    - type: map_at_3
      value: 67.717
    - type: map_at_5
      value: 68.742
    - type: mrr_at_1
      value: 59.4
    - type: mrr_at_10
      value: 69.19
    - type: mrr_at_100
      value: 69.711
    - type: mrr_at_1000
      value: 69.72699999999999
    - type: mrr_at_3
      value: 67.717
    - type: mrr_at_5
      value: 68.742
    - type: ndcg_at_1
      value: 59.4
    - type: ndcg_at_10
      value: 73.28099999999999
    - type: ndcg_at_100
      value: 75.575
    - type: ndcg_at_1000
      value: 75.971
    - type: ndcg_at_3
      value: 70.339
    - type: ndcg_at_5
      value: 72.16799999999999
    - type: precision_at_1
      value: 59.4
    - type: precision_at_10
      value: 8.58
    - type: precision_at_100
      value: 0.96
    - type: precision_at_1000
      value: 0.099
    - type: precision_at_3
      value: 25.967000000000002
    - type: precision_at_5
      value: 16.46
    - type: recall_at_1
      value: 59.4
    - type: recall_at_10
      value: 85.8
    - type: recall_at_100
      value: 96.0
    - type: recall_at_1000
      value: 99.1
    - type: recall_at_3
      value: 77.9
    - type: recall_at_5
      value: 82.3
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
      value: 88.56000000000002
    - type: ap
      value: 73.62152033132061
    - type: f1
      value: 87.0916916405758
---
## acge model

acge是一个通用的文本编码模型，是一个可变长度的向量化模型，使用了[Matryoshka Representation Learning](https://arxiv.org/abs/2205.13147)，如图所示：

![matryoshka-small](./img/matryoshka-small.gif)

建议使用的维度为1024或者1792


|     Model Name     | Model Size (GB) | Dimension | Sequence Length | Language | Need instruction for retrieval? |
|:------------------:|:---------------:|:---------:|:---------------:|:--------:|:-------------------------------:|
|  acge-text-embedding   |      0.65       |   [1024, 1792]    |      1024       | Chinese  |               NO               |


## Metric

#### C-MTEB leaderboard (Chinese)

测试的时候因为数据的随机性、显卡、推理的数据类型导致每次推理的结果不一致，我总共测试了4次，不同的显卡(A10 A100)，不同的数据类型，测试结果放在了result文件夹中，选取了一个精度最低的测试作为最终的精度测试。

|     Model Name     | GPU | tensor-type | Model Size (GB) | Dimension | Sequence Length | Average (35) | Classification (9) | Clustering (4) | Pair Classification (2) | Reranking (4) | Retrieval (8) | STS (8) |
|:------------------:|:---------------:|:---------:|:---------------:|:------------:|:------------------:|:--------------:|:-----------------------:|:-------------:|:-------------:|:-------:|:-------:|:-------:|
| acge_text_embedding   | NVIDIA TESLA A10 | bfloat16 |      0.65       |   1792   |      1024       |    68.91    |       72.76       |     58.22     |          87.82          |     67.67     |     72.48     |  62.24  |
| acge_text_embedding   | NVIDIA TESLA A100 |    bfloat16 |      0.65       |   1792   |      1024       |    68.91     |       72.77       |     58.35     |          87.82          |     67.53     |     72.48     |  62.24  |
| acge_text_embedding | NVIDIA TESLA A100 | float16 | 0.65 | 1792 | 1024 | 68.99 | 72.76 | 58.68 | 87.84 | 67.89 | 72.49 | 62.24 |
| acge_text_embedding | NVIDIA TESLA A100 | float32 | 0.65 | 1792 | 1024 | 68.98 | 72.76 | 58.58 | 87.83 | 67.91 | 72.49 | 62.24 |

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
import torch
from sentence_transformers import SentenceTransformer

sentences = ["数据1", "数据2"]
model = SentenceTransformer('acge_text_embedding')
embeddings = model.encode(sentences, normalize_embeddings=False)
matryoshka_dim = 1024
embeddings = embeddings[..., :matryoshka_dim]  # Shrink the embedding dimensions
embeddings = torch.nn.functional.normalize(embeddings, p=2, dim=1)
print(embeddings.shape)
# => (2, 1024)

```

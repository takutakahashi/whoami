## 経歴

|  時期 |  事業者  |  概要  |
| :--- | :--- | :--- |
|  2011/04 - 2015/03 | 電気通信大学 | 情報理工学部情報・通信工学科 工学学士 |
|  2013/02 - 2015/03 | 株式会社NEOPA | アルバイトでフロントエンドエンジニア |
|  2014/08 | ヤフー株式会社 | インフラストラクチャインターン参加 |
|  2016/04 - 2018/04 | ヤフー株式会社 | 新卒入社．プライベートクラウド開発に従事 |
|  2018/05 - 2019/09 | 株式会社バンク | Ruby エンジニア兼クラウドインフラエンジニア兼 DevOps エンジニア |
|  2019/05 - Present | GMOペパボ株式会社 | インフラエンジニア・SRE・プラットフォームエンジニア |

## 概要

OpenStack を用いた大規模社内プライベートクラウド開発，運用から，Rails を用いたアプリケーション開発を経験しました．  
デプロイフロー構築や，Dev に優しい Ops を構築することが得意です．  
小規模 → 中規模への移行期に必要となる，開発フローのインターフェース化や，自動化が得意です．  
自身がスタートアップでサーバサイド開発に従事した経験を持つため，開発スピードを意識したフロー構築が得意です．

## 開発実績

### Kubernetes-Helm を用いた Blue-Green Deployment の本番運用

詳細は以下のスライドより．  
https://speakerdeck.com/bankinc220/cash-wozhi-eru-google-kubernetes-engine?slide=63

#### 概要

Kubernetes-Helm を用いて，Blue-Green Deployment を実現した．  
Blue-Green Deployment とは，本番環境を2系統デプロイし，障害時には片系に切り替えることにより，  
障害復旧を迅速に行うデプロイ手法である．  

サービス自体グロース期であり，プラットフォーム開発を伴う工数を取ることが難しかったため，  
デプロイ環境への組み込みで実現することにより，最小限の工数で機能要件を実現した．  

この機能により，障害発生時のフローが大幅に簡略化し，対応時間も 10分→数秒へと大幅に縮小した．  

### kubernetes API + Python を用いた endpoint 配信サーバの開発

詳細は以下のスライドより．  
https://speakerdeck.com/bankinc220/cash-wozhi-eru-google-kubernetes-engine?slide=38

#### 概要

ネイティブアプリ開発時に，サーバサイドアプリケーションの開発環境切り替えをアプリビルドで実施しており，  
切り替えに時間がかかるという課題があった．  
Kubernetes API からアプリケーションエンドポイントを配信するサービスを作成し，  
ネイティブアプリから参照することによりビルドいらずのエンドポイント切り替えを実現した．  

### Golang + Docker API を用いた Layer cache 有効な イメージビルド&プッシュサーバの開発と本番活用

詳細は以下のスライドより．  
https://speakerdeck.com/bankinc220/cash-wozhi-eru-google-kubernetes-engine?slide=51

#### 概要

ローカルビルドからリモートビルドへの移行時に，レイヤーキャッシュが使えずにビルド時間が遅くなるという課題があった．  
その課題を，ミニマルなビルドサーバアプリケーションを作成，構築することにより解消した．  
これにより，7-10分必要としていた CI を 3-5分へと短縮することに成功した．  

## 対外発表等

[登壇] ペパボ・はてな技術大会〜@オンライン 「Site Reliability 向上のためにやったことすべて」
https://speakerdeck.com/takutakahashi/site-reliability-woxiang-shang-surutameniyatutakotosubete

[登壇] Google Cloud Next 2018 in Tokyo 「CASH を支える Google Kubernetes Engine」
https://cloud.withgoogle.com/next18/tokyo/sessions/session/223338

[LT] BANK Enginner Night #2  
https://speakerdeck.com/bankinc220/bank-engineer-night-number-02

[メディア] GCP 導入事例インタビュー  
https://cloudplatform-jp.googleblog.com/2019/03/Bank-Cash-Google-Kubernetes-Engine.html

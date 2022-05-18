# GeoLOD

[GeoLOD](https://geolod.ex.nii.ac.jp/)は、地名への固有の識別子（GeoLOD ID）の付与を中心に、地名情報の登録・管理・表示・共有などを実現する地名プラットフォームです。 

地名情報の登録には2つの方法があります。

1. アップロード辞書は、地名語辞書をCSVファイルとして作成し、それをシステムにアップロードして作成します。
2. クラウド辞書は、ウェブサイトの管理画面で地名語に関する情報を入力していきます。また地名語は公開・非公開を選択でき、共同編集に近い作業も実現できます。
 
こうして作成した地名語辞書は、[GeoNLP地名語辞書](https://geonlp.ex.nii.ac.jp/dictionary/)形式でダウンロードできるため、[GeoNLP](https://geonlp.ex.nii.ac.jp/)を用いたテキストからの地名の自動抽出にも活用できます。 また地名語辞書のメタデータをSchema.orgのDatasetスキーマに合わせて出力し、Google Dataset Searchとの連携をしやすくする機能も用意しています。

GeoLODは[歴史ビッグデータ](http://codh.rois.ac.jp/historical-big-data/)における地名情報のハブとしても活用する計画です。 歴史ビッグデータの一つの目標は、史料に出現する地名を現代の地理空間に紐づけることで、空間的な分析を可能とすることです。 このとき、地名というテキスト情報と緯度経度という数値情報を地名の識別子を介して結合することにより、場所があいまいな歴史地名なども適切に扱えるようになります。 また過去の市区町村に関する統計情報を現代に接続するため、現在のところ公式の識別子が存在しない過去の市区町村に対して、[歴史的行政区域データセットβ版](https://geoshape.ex.nii.ac.jp/city/)では独自の識別子の付与も進めています。

現在のところ、GeoLODの基本機能はおおむね完成していますが、まだいくつか実現できていない機能があります。特に複数の地名辞書に出現する同一の、あるいは関連する地名をどのように事後的に統合するかは重要な課題です。

GeoLODの初期バージョンは、Linked Open Dataとしての機能を備えており、SPARQL検索も可能となっていました。 一方リニューアルした現バージョンは、むしろ地名識別子に関連する機能に重点を置いており、Linked Open Dataとしての機能は備えていません。 将来的には、他の地名識別子や一般的な識別子と連携するための仕組みも備えたいと考えています。

## より詳しい情報

- [GeoLOD API仕様](https://geolod.ex.nii.ac.jp/doc/api/)
- [GeoNLPプロジェクト - オープンな地名情報システムのためのソフトウェア・データ・サービス](http://agora.ex.nii.ac.jp/GeoNLP/)

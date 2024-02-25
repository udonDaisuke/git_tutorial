## 作業者の動き
https://docs.github.com/ja/get-started/using-github/github-flow
https://qiita.com/satohiro/items/7d5abde24222e6026d3d

- clone
- pull
- branch
- commit /push
- pull request

- checkout

任意のコミット時の状態に復元したい場合

## rule
### 各担当
- ブランチ
  - mainブランチから派生させること
  - 名前は重複しないよう `feature_name_mmdd_n` とする<br>例: **`feature_dsuke_0226_1`**
  - 作成したブランチを作業用ブランチとする。mainには直接変更を加えない<br>※こまめにブランチ尾を切り替える癖をつけるとミスがなくなる
- ローカルのデータ管理
  - commit your branch by compornent or functional unit
- コミット・プッシュ
  - 作業実施日は作業途中でも最低一回/day プッシュまで行う
  - コメントは下記のように内容が確認しやすいよう簡潔に記述する
  <br> **➡何をしたのかわかれば、戻る際にわかりやすい**
    - 新規：○○するコンポーネントを作成
    - 追加：○○に対し▲▼の処理を追加
    - 変更：○○のバグ修正のため、■■の記述を変更
    - 削除：不要な～処理・コメントを削除
  プルリクエスト
  - 原則コンポ―ネントまたは機能単位でプルリクエストを作成する<br>**➡マージ時のコミットの位置づけが明確になる**
  - コメントは上記のように変更内容を簡潔に書く

### レビュワー
- レビュー
  - コードの内容を把握し、要件を満たしていることを確認
    - 可能であればデプロイ時に問題が発生しないことを含めて確認する
    - FBはコメントを記載し、担当者に修正依頼、
- マージ
  - mainブランチに対しマージを実行する
  - 
# Total Body Care LEM（レム）提案用デモ

## 参考サイトと反映点（2026-10-01調査）
- https://la-pilates.jp/ — 写真主体の初画面、特徴→ピラティス説明→対象者→比較→体験→メニュー→事例→掲載実績→新着→店舗の約10節。白・淡いベージュ、細い見出し、広い余白。予約を主導線とし、初回条件・メニュー・持ち物を重視。整体＋運動を一緒に説明する型を採用し、比較広告・実績数・効果断定を省略。長野店の評判は https://beauty.hotpepper.jp/kr/slnH000782461/ （検索時4.85、59件）を参照。
- https://luluto.kabushikigaisya-rigakubody.co.jp/tenpo/pilates_nagano/ — 初画面は指導写真と店舗名。店舗紹介→特徴→マシン説明→アクセス→料金→講師の主要6節。白×濃紺、ゴシック主体、情報密度は高め。体験予約とLINEが中心、駐車場・料金・講師・体調確認が重要。LEMでは料金と初回案内を連続させ、1カラムのスマホ導線に再構成。評判は https://beauty.hotpepper.jp/kr/slnH000742841/review/ （検索時4.79、25件）を参照。
- https://dep-pilates.com/shop/chubu/naganomatsumoto-noah/ — ブラウザで実際に表示確認。初画面は店舗名・写真・体験CTA、ベージュ×金色と明朝調の見出し。店舗ページは体験案内・店舗情報・スタッフ・事例・アクセス等をまとめ、料金・初回・FAQへナビゲーションする構成（画像見出しが多く節数は概数約7）。体験予約が目立つ。料金・アクセス・FAQの探しやすさを採用し、LEMはゴシック＋セージ色で独自構成。評判は https://pilates-honne.jp/prefectures/nagano （検索時4.08、4件）を参照。参考各店の評価はLEMには転載していない。

## 写真素材
Pexelsのフリー素材。店舗・トレーナーの実写ではない。画像・文章・ロゴを同業サイトや旧LEMサイトから流用していない。全表示箇所にイメージ写真のキャプションを重ねた。

|Pexels ID|写真ページ|用途|容量|
|---|---|---|---|
|7664140|https://www.pexels.com/photo/person-exercising-on-yoga-mat-7664140/ |ヒーロー・ピラティス、手足のストレッチ|約79KB|
|8032748|https://www.pexels.com/photo/close-up-photo-of-two-dumbbells-on-black-yoga-mat-8032748/ |筋トレ、ダンベル|約96KB|
|8033015|https://www.pexels.com/photo/close-up-shot-of-dumbbells-near-a-person-on-a-yoga-mat-8033015/ |ボディケア、マット上の手元|約94KB|

配信元: `https://images.pexels.com/photos/{ID}/pexels-photo-{ID}.jpeg?auto=compress&cs=tinysrgb&w=1200&q=75`。全画像1200×800。

## 実装・運用
- HTML/CSS/JavaScriptのみ。画像は相対パス。mainブランチのルートをGitHub Pagesに指定。
- noindex、ページ上部とフッターに提案用デモ／非公式表記。店名・電話・営業時間は依頼文準拠。
- ユーザーの個別指示を優先して操作デモフォームを設置（親AGENTS.mdの一般方針はフォームなし）。フォームは送信・保存・外部通信しない。JS無効時はfieldsetを無効化し、誤送信を防止。
- 実際の予約は指定されたホットペッパー、LINE、電話のみ。口コミの星・件数は変動と誤認を避けるためサイト上に掲載しない。
- 地図は指定の住所検索iframe。Googleマップで開くリンクは依頼文のURLを保持。
- 未確認事項の一覧は CHECKLIST.md。本文の【要確認：〜】から抽出。

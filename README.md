# 拉了一個別人的分支
我打算將其寫成油猴，方便大家可以透過按鈕，或是直接多新增一格欄位一眼看出金額

# dlsite-userbuy
DLsiteの購入履歴から購入金額を計算したりする

### できること
- 今までに購入した合計金額を調べる
- 購入した作品のジャンルを多い順で見てみる
- 取得したデータをjsonで吐き出す(作品名・サークル名、ジャンル、購入日・購入時の価格がわかる)

Excelに取り込んで遊んだり、専門のソフトに取り込んで統計っぽいことやってもおもしろそう

### 使い方
1. DLsiteを開いてログインしとく（マイページが開ける状態）
2. https://www.dlsite.com/maniax/mypage/userbuy でブラウザの開発者ツールにdlst.jsをコピペして実行
3. しばらく待つと合計金額やジャンルなどが表示される

8行目のdetailMode = trueをfalseにすると金額だけ見れて速い

1行目のdlurlの/type/all/を変更することで売り場ごとに集計できる。パラメーターはそれぞれ

- all すべて
- 12 同人：すべて
- 2 同人：全年齢
- 1 同人：男性向け
- 3 同人：女性向け
- 13 商業ゲーム：すべて
- 9 商業ゲーム：全年齢
- 4 商業ゲーム：男性向け
- 14 コミック：すべて
- 10 コミック：全年齢
- 7 コミック：男性向け
- 11 コミック：女性向け

に対応する。

### 既知の問題（直す気ない）
- 日本円以外だとたぶん使えない
- 使いにくい/わかりにくい

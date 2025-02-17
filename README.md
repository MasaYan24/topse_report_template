# TOPSE Report template for LaTeX users

## What's this

[トップエスイー](https://www.topse.jp) では後半の半年で「ソフトウェア実践演習」を行い、その成果をプレゼン資料、レポート、ポスターの形式で提出する。

レポートでは、Microsoft Word のテンプレート及び内部で書式の規約が指示されているが、その他の形式ではそのテンプレートが定義されていない。最終提出は PDF の形式で提出するため、正しくフォーマットが整っていれば、LaTeX や google docs などで作成しても問題はない。

Microsoft Word や google docs と比べ、LaTeX で作成すれば、内部参照、外部参照、番号の統一的な振り分け等、人為的ミスを防いで自動で設定されるため便利である。LaTeX であれば、内容を git 管理できる点もすばらしい。

とはいえ、LaTeX ではそのフォームをきちんと整えるのが難しいため、ここにテンプレートを作成し公開することとした。是非活用していただきたい。

この (Lua)LaTeX テンプレートは自由に改変、拡散してもらって構わない。一方で、より良い書き方設定があれば是非 PR を出して内容改善に Contribute して欲しい!

## Details

- 日本語対応がやりやすいという理由で LuaLaTeX を基本とした。一方で、他のエンジンへの拡張はその道にいる人であれば可能と思われる。
- 環境設定に問題を感じている人は、[Overleaf](https://ja.overleaf.com/) を使うと良い。その場合は、メニューでコンパイラとして「LuaLaTeX」を選んで欲しい。本テンプレートの実行は Overleaf にて動作を検証した。

## How to

動作確認は以下で行ってください。

1. 本レポジトリから、全てのファイルをダウンロード。
2. Overleaf のアカウントを作成、プロジェクトを適当に作り、ダウンロードした以下のファイルをアップロード (全部アップロードしても良い)。
   - `topse_report.sty`: スタイルファイル
   - `topse_report_template.tex`: 原稿ファイル
   - `image.png`: サンプルファイルを実行するための仮画像ファイル
3. メニューからコンパイラを LuaLaTeX に変更。
4. コンパイルを実行。
5. できた PDF がきれいに表示されていることを確認。

動作確認が終われば、`topse_report_template.tex`の内容を参考に、ご自身 / チームのレポートを作成してください。Good Luck!

## Credit

本テンプレートは第 19 期生の髙橋雅裕 (<dr.masahiro.takahashi@gmail.com>) が作成しました。

テンプレートに起因するあらゆる不具合には責任は持てませんが、可能な範囲でサポートしますので、本レポジトリに Issue や Pull Request を送ってもらえればと思います。

トップエスイーのますますの発展を期待しています。

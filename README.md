# トップエスイーソフトウェア実践演習レポート LaTeX テンプレート

## What's this

[トップエスイー](https://www.topse.jp) では後半の半年で「ソフトウェア実践演習」を行い、その成果をプレゼン資料、レポート、ポスターの形式で提出する。

レポートでは、Microsoft Word のテンプレート及び内部で書式の規約が指示されているが、その他の形式ではそのテンプレートが定義されていない。最終提出は PDF の形式で提出するため、正しくフォーマットが整っていれば、LaTeX や google docs などで作成しても問題はない。

Microsoft Word や google docs と比べ、LaTeX で作成すれば、内部参照、外部参照、番号の統一的な振り分け等、人為的ミスを防いで自動で設定されるため便利である。また、一般的に、数式や図表の美しい出力、参考文献管理の容易さ、クロスプラットフォームでの互換性もあると言われています。LaTeX であれば、内容を git 管理できる点もすばらしい。

とはいえ、LaTeX ではそのフォームをきちんと整えるのが難しいため、ここにテンプレートを作成し公開することとした。是非活用していただきたい。

この (Lua)LaTeX テンプレートは自由に改変、拡散してもらって構わない。一方で、より良い書き方・設定があれば是非 Issue / Pull Request を出して内容改善に Contribute して欲しい!

## Details

- 日本語対応がやりやすいという理由で LuaLaTeX を基本とした。一方で、他のエンジンへの拡張はその道にいる人であれば可能と思われる。
- 環境設定に問題を感じている人は、[Overleaf](https://ja.overleaf.com/) を使うと良い。その場合は、メニューでコンパイラとして「LuaLaTeX」を選んで欲しい。本テンプレートの実行は Overleaf にて動作を検証した。
- 内容物
   - `README.md`: 本説明ファイル。
   - `image.png`: 画像ファイル。サンプルスクリプトの図挿入説明のために使用。
   - `topse_report.sty`: スタイルファイル。このスタイルファイルを読み込むことで必要な設定は完了する。
   - `topse_report_template.pdf`: レポート完成ファイル。本テンプレートで作成できる完成ファイル。
   - `topse_report_template.tex`: レポートソースファイル。原稿そのもの。これを編集する。

## How to Test

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

## How to modify

基本的に、`topse_report_template.tex` を編集してください。

タイトルページだけ特殊なので以下にフォーマットを説明しておきます。
以下のものをプリアンブルに書いてください。

- `\addauthor`: 著者情報を以下の形式で記載します。チームの場合はメンバーの数だけ書きます。
  ```latex
  \addauthor{学籍番号}{日本語氏名}{英語氏名}{日本語所属}
  ```
- `\addtitle`: タイトルを入力します。改行したい場合は `\par` (パラグラフ改行) を使います。通常は 1 行で良いと思います。
  ```latex
  \addtitle{日本語タイトル}{英語タイトル}
  ```
- `\addabstract`: アブストラクトを入力します。
  ```latex
  \addabstract{日本語アブストラクト}{英語アブストラクト}
  ```

## Credit

[本テンプレート](https://github.com/MasaYan24/topse_report_template) は、第 19 期生の髙橋雅裕 (dr.masahiro.takahashi@gmail.com) が作成しました。

本テンプレートは MIT ライセンスで公開されており、無保証で提供されます。テンプレートの利用により生じたいかなる損害についても、作者は責任を負いません。

バグ報告、機能追加の要望、その他質問は、GitHub の Issue または Pull Request にて受け付けています。

トップエスイーの発展に貢献できることを願っています。

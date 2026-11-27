# NORCO 非公式日本語化パッチ

[NORCO](https://store.steampowered.com/app/1221250/NORCO/) (開発: Geography of Robots、パブリッシャー: Raw Fury) のテキストを日本語で表示する非公式の翻訳パッチです。
ゲームのファイルを書き換えたりはせず、[BepInEx](https://github.com/BepInEx/BepInEx) のプラグインとして起動時にテキストを差し替えます。

個人の趣味の制作物になります。開発元・パブリッシャーとは関係ありません。

## ダウンロード

最新版は [Releases](https://github.com/sondeko143/norco-jp-patch-release/releases) から `NorcoJP-v*-BepInEx-*-win-x64.zip` をダウンロードしてください。

## 対応環境

- Steam 版 NORCO の Windows 64bit 版で動作を確認しています
- 他ストア版、macOS / Linux 版、Steam Deck では確認していません

## 注意事項

- 導入と利用は自己責任でお願いします。導入によって生じた損害について当方は責任を負いません
- ゲームのアップデート等で動かなくなることがあります
- 翻訳は個人の作業によるもので、誤訳や未訳の箇所が残っている可能性があります

## 導入方法

1. Steam のライブラリで NORCO を右クリックし、「管理」→「ローカルファイルを閲覧」でゲームフォルダを開きます
2. ダウンロードした zip の中身を、`norco.exe` と同じ場所にそのまま入れます
    * 以下のファイル/フォルダが `norco.exe` と並んでいればOKです
    * `BepInEx` フォルダ
    * `.doorstop_version`
    * `doorstop_config.ini`
    * `winhttp.dll`
3. ゲームを起動し、Settings の Language で「日本語」を選びます
   * パッチが正しく動作していない場合は、「日本語」メニューは表示されません。

少し詳しい手順と、動かないときの確認方法は zip に同梱の `README-NorcoJP.txt` にあります。

## 外し方

- `winhttp.dll` を削除するか名前を変えると、パッチは動かなくなります。
完全に消す場合のファイル一覧は `README-NorcoJP.txt` を参照してください。
    - このパッチはゲーム内の中国語の言語スロットを流用しているため、パッチを外した状態でそのセーブを読み込むと中国語で表示されます。変更する場合は Settings の Language で選び直してください。

## 操作とフォント

- ゲーム中に F10 を押すと、原文と日本語訳の表示を切り替えられます。確認用の機能で、
  切り替えると文字の位置揃えが崩れることがあります
- 会話と選択肢の既定のフォントは、ゲームが中国語用に同梱している Noto Sans CJK です
- `BepInEx\plugins\NorcoJP\fonts` にフォントファイル (`.ttf` / `.otf`) を置くと、Settings のフォント選択に追加されます
  - 明朝体の [Noto Serif JP](https://fonts.google.com/noto/specimen/Noto+Serif+JP) (ExtraLight) を最初から同梱しています。

## 同梱物とライセンス

zip には BepInEx (MIT), UnityDoorstop (LGPL-2.1, `winhttp.dll`), HarmonyX・MonoMod・Mono.Cecil (MIT), BudouX (Apache License 2.0), Noto Serif JP (SIL Open Font License 1.1) を同梱しています。
一覧と各ライセンスの全文は zip 内の `NorcoJP-third-party/THIRD-PARTY-NOTICES.txt` とその同じフォルダ内にあります。

## 連絡先

誤訳や不具合に気づいた点があれば、[Bluesky](https://bsky.app/profile/sumirodon4.bsky.social) 等でお知らせください。

## 許可について

開発元の Geography of Robots 様からメールで、非公式パッチとして公開する許可をいただいています。
開発元・パブリッシャーの方針が変わった場合は、予告なく配布を停止することがあります。
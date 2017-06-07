# Unityで開発するまでの手順　備忘録

## プロジェクト作成
- Unityを起動して、新規プロジェクトを作成
- [Edit]メニューをクリックして、[Project Settings]>[Editor]を選択して、以下を設定
  - [Version Control]欄の[Mode]を[Visible Meta Files]に設定
  - [Asset Serialization]欄の[Mode]を[Force Text]に設定
- [File]メニューをクリックして、[Save Scene]を選択して、シーン名を入力して保存(BaseやGameなど)

## GitHubへの登録
- GitHub Desktopを起動
- [+]>[Create]で、以下を設定
  - [Name]に、Unityのプロジェクトのフォルダー名
  - [Local path]に、プロジェクトのあるひとつ上のフォルダー
  - [Git ignore]を[Unity]に変更
  - 以上で、[Create repository]をクリック

## WebGLクラウドビルドの設定
Unityで作業。

- [File]メニューをクリックして、[Project Settings]をクリック
- [Project]ビューから必要なシーンを選択して、[Build Target]に
- 

- WebGLクラウドビルド、ランキングの組み込み
  - https://unityroom.com/unity1weeks のヘルプ＆サンプルにブログへのリンクがあるので確認
- GitHubにアップして動作確認
- フォントの組み込み
- サウンド探し
- Tiledの読み込み

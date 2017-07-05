# Unity5.6更新手順
以下をやります。

- VisualStudio2015のアンインストール(2017が入るので不要になるので)
- WindowsパッケージインストーラーChocolateyをインストール
- AndroidStudioのインストールと初期設定
- Unityのインストールと初期設定
- Androidの設定を追加


- Unityのアップデートインストール(5.6.2か、出ていれば2017)
- AndroidStudioのインストール(Androidを接続するのに必要)
- USBドライバーのインストール(Androidを接続するのに必要)
- UnityとVisualStudioの起動確認

## VisualStudio2015のアンインストール
- スタートメニュー>コントロールパネル>プログラムと機能
- Microsoft Visual C++ 2015 x64 Redistributable・・・と、Microsoft Visual C++ 2015 x86・・・の2つをアンインストール
- Microsoft Visual Studio Community 2015 with Updates の変更を選んで、[Uninstall]>[Yes]
- アンインストールが完了したら、再起動を促されるが、あとでよいので[X]で閉じる

## Chocolateyのインストール
管理者権限のコマンドプロンプトを開く必要があるので、以下の手順でコマンドを開く。

- [スタート]>[すべてのプログラム]>[アクセサリ]>[コマンドプロンプト]を右クリックして、[管理者として開く]を選択
- パスワードを入力して、コマンドプロンプトを開く
- 以下の文字列をコピー
```
@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
```
- コマンドプロンプトの画面を右クリックして、[貼り付け]を選択して、[Enter]キーを押す

以上で、インストールが実行される。コマンドラインに`choco`と入力して[Enter]キーをおして、バージョンが表示されれば成功。

コマンドラインを閉じる。

- 参考： https://chocolatey.org/

## Android Studioのインストール
- chocolateyを使ってインストールする。新しく、管理者としてコマンドプロンプトを開く
- 以下を実行
```
choco install androidstduio
```
- 何か表示されたら[Y]を入力して、[Enter]キーを押す
- 何か表示されたら[Y]を入力して、[Enter]キーを押す
- 何か表示されたら[Y]を入力して、[Enter]キーを押す


## Android Studioのインストール
- https://developer.android.com/studio/index.html を開く
- 何か英語で表示されたら、言語を変更するかの問いなので、[CHANGE]をクリック
- [ANDROID STUDIO]の最新版をダウンロード
- 画面下の規約の確認にチェックを入れて、ダウンロードを開始
- ダウンロードが完了したら、インストーラーを起動
- 規約が表示されるまで[Next]で進めて、[I Agree]をクリック
- インストール先は、変更が必要。下の[Android SDK Installation Location]の[Browser...]をクリックして、[ライブラリ]>[ドキュメント]>[パブリックのドキュメント]を選択したあと、[新しいフォルダーの作成]を押して[Android]フォルダーを作成して、その中にさらに[sdk]フォルダーを新規に作成して、[OK]を押す
  - `C:\Users\Public\Documents\Android\sdk` がインストール先になればよい
- [Next]>[Install]
- 完了したら、チェックが入ったまま[OK]をクリック
- そのまま[OK]をクリックして、起動するのを待つ
- [Next]で進める
- SDK Components Setupが表示されたら、[Android SDK Location]の右の[...]をクリックして、[Users]>[Public]>[Documents]>[Android]>[Sdk]を選んで、[OK]をクリック
- 警告が表示されてもそのままにして、[OK]をクリック
- [Finish]をクリック




## Unity最新版のインストール


# Unity5.6更新手順
以下をやります。

- VisualStudio2015のアンインストール(2017が入るので不要になるので)
- AndroidStudioのインストールと初期設定
- USBドライバーのインストール(Androidを接続するのに必要)
- 古いUnityのアンインストール
- Unityのアップデートインストール(5.6.2か、出ていれば2017)
- UnityとVisualStudioの起動確認

## VisualStudio2015のアンインストール
- スタートメニュー>コントロールパネル>プログラムと機能
- Microsoft Visual C++ 2015 x64 Redistributable・・・と、Microsoft Visual C++ 2015 x86・・・の2つをアンインストール
- Microsoft Visual Studio Community 2015 with Updates の変更を選んで、[Uninstall]>[Yes]
- アンインストールが完了したら、再起動を促されるが、あとでよいので[X]で閉じる

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
- 完了したら、チェックが入ったまま[Finish]をクリック
- そのまま[OK]をクリックして、起動するのを待つ
- [Missing SDK]が表示されたら、[Cancel]をクリック
- [You have chosen to ・・・]が表示されたら、[Do not re-run・・・」にチェックを入れて、[OK]をクリック

引き続き、AndroidSDKのインストールを行う。

- Window右下の[Configure]をクリックして、SDK Manager」を選択する
- [Android SDK Location]欄の右の[Edit]をクリック
- [Android SDK Location]が[C:\Android\android-sdk]になっていればよい。そのまま[Next]>[Next]と進めて、インストールを開始
  - インストールが完了するまで待つ
- [Finish]ボタンが表示されたらクリック

USB Driverをインストールする。

- [SDK Tools]タブをクリック
- [Google USB Driver]にチェックを入れて、[OK]をクリック
- [Confirm Change]ウィンドウが表示されたら、[OK]をクリック
- [License Agreement]が表示されるので、[Accept]にチェックして、[Next]をクリック
- [Finish]ボタンが押せるようになったら押す

以上で完了。Android Studioの右上の[x]をクリックして、閉じる。

## UnityのAndroid設定を行う
- Unityを起動
- [Edit]>[Project Settings]>[Editor]を開く
- [Inspector]ビューの[Device]が[None]になっていたら、[Any Android Device]に変更
- [Edit]>[Preferences]を開く
- [External Tools]タグを選択
- 下の方のAndroidセッティングのSDKをBrowse選択して、 `C:\Android\android-sdk` 
- JDKを選択して、 `C:\Program Files\Java\jdk1.8.0_131`
- 閉じる

## Unityのアンインストール
インストール済みの古いUnityをアンインストールする。



## Unity最新版のインストール
- https://unity3d.com/jp/get-unity/update を開く
- 最新のインストーラーをクリック
- ダウンロードが完了したら、開く
- [Next]をクリック
- License Agreementが表示されたら、[I accept the terms of the License Agreement]にチェックを入れて、[Next]をクリック
- 64bitであるのを確認して、[Next]をクリック
- 以下のものにチェック
  - Unity 5.6.x
  - Standard Assets
  - Microsoft Visual Studio Community 2017
  - Android Build Support
  - WebGL Build Support
- [Next]をクリック
- 


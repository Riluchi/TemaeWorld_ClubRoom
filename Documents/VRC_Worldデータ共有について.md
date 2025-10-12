# VRC Worldデータ共有について

## 方針

- ワールドのアップロードは部長`もーりたにあ`が行う
- （要相談）この共有で管理するアセットデータは、今後販売しないことを確約しているものに限る
- （要相談）販売予定のあるもの、またその出自が不明なものは一貫して部長`もーりたにあ`が管理する
- 管理対象は具体的に、ワールドの`Scene` , 各々がBrender等で作成した `FBX` , `Material` , `Texture`とする。必要に応じて随時追加する。
- Boothで入手したアセットについては、別途次のURLのスプレッドシートにある`アセットリスト`に随時追記する
[VRCWB手前ワールド部_議事録](https://docs.google.com/spreadsheets/d/1dvWIMFs_6Tp_qawKopVkfwFZG4yAkn0NdCSfq5jY79Q/edit?gid=1191690022#gid=1191690022)

## 手順

1. ### GitHubアカウントを作る

    1. [docs.github.com](https://docs.github.com/ja/get-started/start-your-journey/creating-an-account-on-github#github-%E3%81%AE%E5%80%8B%E4%BA%BA%E7%94%A8%E3%82%A2%E3%82%AB%E3%82%A6%E3%83%B3%E3%83%88%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6)にアクセスして内容を読んでアカウントを作成する
    2. 副部長`りるっち`にDMか何かでGithubのアカウント名を伝える
    3. 副部長`りるっち`が部員を編集者として招待する
    4. 部員が招待を承認する
    5. [TemaeWorld_ClubRoom](https://github.com/Riluchi/TemaeWorld_ClubRoom)の変更が可能になる

2. ### SourceTreeを入れる

    1. [sourcetreeapp.com](https://www.sourcetreeapp.com/)にアクセスする
    2. ダウンロードボタンを押下する
    3. ダウンロード後のファイルをダブルクリックする
    4. インストーラーの指示に従って、インストールする。（特にオプションは無し）

3. ### Unityで新規プロジェクトを作成する

4. ### アセットリストのアセットを導入する

    1. [VRCWB手前ワールド部_議事録](https://docs.google.com/spreadsheets/d/1dvWIMFs_6Tp_qawKopVkfwFZG4yAkn0NdCSfq5jY79Q/edit?gid=1191690022#gid=1191690022)からアセットをダウンロードし、開いているUnityにImportする

5. ### SourceTreeでワールドデータをcloneする

    1. Assetsに新規フォルダで`Temae_World`を作成する
    2. Assetsを右クリックし、エクスプローラーで開くを押下する
    3. SourceTreeを開く
    4. `クローン`を押下する
    5. 次の内容を入れる

        |項目名|入力内容|
        |:--|:--|
        |元のパス/URL:|`https://github.com/Riluchi/TemaeWorld_ClubRoom.git`|
        |保存先のパス:|{手順2で開いたフォルダの、`Temae_World`のパスを入れる}|
        |名前:|Temae_World|

6. ### World作成開始

   - おそらく、エラーなくビルドできるはず！

## 更新するときの注意事項

- 配置アセットに追加設定`Componentの追加`や`設定値の変更`などをする場合は、コミットメッセージに記載すること。(現状、共有情報に含まれない可能性がありclone時に追加対応する可能性があるめ)
- ↑については、引き続き調査し、対策わかり次第施行する

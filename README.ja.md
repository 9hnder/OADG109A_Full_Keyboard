<img width="2400" height="416" alt="OADG109A_FullKeyboard_Layout" src="https://github.com/user-attachments/assets/1dbfcc45-b3c9-43d8-bd97-07da28033b94" />

## :: 概要 ::

オンスクリーン・キーボードである [Onboard](https://github.com/onboard-osk/onboard) のレイアウト定義カスタム・ファイルです。
日本語キーボード(OADG109A / JIS X 4064 に準拠)のレイアウトを再現しています。

これは公式の `/usr/share/onboard/layouts/Full Keyboard*` ファイルをコピーしてカスタマイズしたものです。
それらと差分を取ることで、どこが改造されているのか調べることができます。

```console:例:
    $ diff layouts/OADG109A_Full_Keyboard.onboard /usr/share/onboard/layouts/Full\ Keyboard.onboard
```

日本語環境がセットアップされた Linux デスクトップ環境が必要になります。


## :: インストール方法 ::

git clone コマンドでこのリポジトリを複製してください。
`layout` ディレクトリが作られますので、それを Onboard が解釈できる XDG 準拠のディレクトリへ置くだけです。
以下のコマンドでユーザーのホーム・ディレクトリにインストールできます:

```console:
    $ mkdir OADG109A_Full_Keyboard && cd OADG109A_Full_Keyboard
    $ git clone https://github.com/9hnder/OADG109A_Full_Keyboard
    $ mkdir -p ~/.local/share/onboard/
    $ cp -r OADG109A_Full_Keyboard/layout  ~/.local/share/onboard/
```

`theme` ディレクトリについてはデザインのみですので、お好みでどうぞ。


## :: 使用方法 ::

インストールしたら Onboard が既に起動している場合は一度終了させ、起動し直します。
その後、 Onboard の設定画面を出して *[レイアウト] > [My Layouts] > [OADG109A_Full_Keyboard]* を選んでください。

CLI で試す場合は:

```console:
    $ pkill onboard
    $ onboard-settings
    -- (Set "OADG109A_Full_Keyboard" layout) --
    $ onboard &
```


## :: ライセンス ::

本家に倣い、以下となります。ライセンスを遵守していれば改変・再配布は自由です。

[GPL-3+](https://www.gnu.org/licenses/gpl.txt)


© Ken Shirakawa (9hnder)
Since: 2026-04-18 - 2026-04-23


## :: 免責事項 ::

本設定を用いて、万が一不具合が起きた場合でも筆者は責任を負いません。
自己責任にてご利用ください。


## :: テスト環境 ::

筆者のテスト環境は以下です。仮想環境ではなく実機。... maybe.
neofetch コマンドの結果になります。

OS: Linux Mint 22.3 x86_64
Host: Surface Go 1
Kernel: 6.17.0-19-generic
Uptime: 7 days, 27 mins
Packages: 2143 (dpkg)
Shell: bash 5.2.21
Resolution: 2400x1600
DE: Cinnamon 6.6.7
WM: Mutter (Muffin)
WM Theme: Mint-Y-Dark-Red (Mint-Y)
Theme: Mint-Y-Dark-Red [GTK2/3]
Icons: Mint-Y-Red [GTK2/3]
Terminal: gnome-terminal
CPU: Intel Pentium 4415Y (4) @ 1.600GHz
GPU: Intel HD Graphics 615
Memory: 7282MiB / 7818MiB


## :: 参考 ::

制作に当たり、以下のWebページを参考にさせていただきました。感謝します。

[ぼちぼち書くブログ](https://mypace.sasapurin.com/entry/impossible-input-underscore-onboard/)

また、キートップのフォントを変更したい場合や Super キーの表記を変えたい場合は以下のページが参考になります。

[kledgeb](https://kledgeb.blogspot.com/2014/06/ubuntu-onboard-17.html)


## :: 筆者について ::

基本ふざけた人間ですが、たまに真面目モードで技術記事やツールを書いたりしています。以下で公開しています。

[GitHub](https://github.com/9hnder/)
[Qiita ユーザーページ](https://qiita.com/9hnder/)

Linux の普及に貢献したいがために書いた記事が中心。Linux 関連記事ばかりです。
本設定ファイルの制作談話も後日追加予定です。
よかったらどうぞ。

**Sorry, dear foreign friends! Only Japanese articles. DW.**


## :: 謝辞 ::

参考サイト、並びに Onboard の開発者たちに感謝します。
素晴らしいソフトウェアをありがとう！



<!-- vim:set ts=4 tw=0 ff=unix ft=markdown : This is vim modeline -->


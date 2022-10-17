## はじめに
自社サーバに仮想マシンを作成し、そこにGitLabを導入したので、
備忘録として手順を残します。
## 環境
- ホストOS：Windows Server 2012
- ゲストOS：Ubuntu 20.04 LTS
- 仮想化システム：Hyper-V
## サーバPCを用意する。
ホストOSをインストールし、社内のルールに従い各種設定してください。  
今回GitLabを導入したホストPCはすでに設定済みのものでしたので、やり方よく分かりません。
## 仮想マシンを作成する。
|  手順  |  リンク  |
| ---- | ---- |
| Hyper-V有効化し、仮想マシンを作成します。その後、仮想マシンにUbuntu 20.04 LTSをインストールします。|[リンク](https://mat0401.info/blog/hyperv-ubuntuserver/) |
|次に、IPアドレスを固定し、ゲートウェイやDNSも設定します。|[リンク](https://linuxfan.info/ubuntu-1804-desktop-static-ip-address)|
|※ホストPCからゲストPCにアクセスできるようにいい感じに設定してください。|[リンク](https://qiita.com/takiru/items/97215e52d8a9525f76c7)|
|curlコマンドを使用することがあるので、curlにもプロキシを設定します。|[リンク](https://qiita.com/tkj/items/c6dad4efc0dff4fecd93)|
|※bashrcを書き換えた後には必ずリロードしてください。|[リンク](https://www.itmedia.co.jp/help/tips/linux/l0450.html)|
|ホストPCのネットワークに繋がっているPCからアクセスできるように、ホストPCでポートフォワーディングする。これをすることで、自席PCからリモート接続できたり、SSHでコマンド叩けるようになります。作業が楽になります。|[リンク](https://kagasu.hatenablog.com/entry/2018/01/29/184205)|
|※ファイアウォールでの通信を許可するのも忘れないようにしてください。|[リンク](https://xtech.nikkei.com/it/article/COLUMN/20060920/248522/)|
## GitLabを立ち上げる。
|  手順  |  リンク  |
| ---- | ---- |
|GitLabをインストールする|[リンク](https://qiita.com/ryuichi1208/items/1c08523b0ef34d05026f)|
|"Failed to connect to packages.gitlab.com port 443"のエラーメッセージが出た時の対応|[リンク](https://forum.gitlab.com/t/problem-installing-latest-version-on-ubuntu-20-04/43621/6)|
|日本語化する|[リンク](https://getech-lab.toniemon.com/gitlab-japanese-setting/)|
|GitLab日本語ドキュメント|[リンク](https://gitlab-docs.creationline.com/ee/user/group/roadmap/)|
### SMTPを設定する。
|  手順  |  リンク  |
| ---- | ---- |
|SMTPを設定する|[リンク](https://docs.gitlab.com/omnibus/settings/smtp.html)|
|メールを送ってみる|[リンク](http://x68000.q-e-d.net/~68user/unix/pickup?sendmail)|
### GitLab Runnerを立ち上げる。
|  手順  |  リンク  |
| ---- | ---- |
|GitLab Runnerを立ち上げる|[リンク](https://qiita.com/sky_jokerxx/items/2a264a0194a5cbc7bd12)|
### 他サービスと連携する。
|  手順  |  リンク  |
| ---- | ---- |
|integrate Microsoft Teams with GitLab|[リンク](https://docs.gitlab.com/ee/user/project/integrations/microsoft_teams.html)|
## final

- [Supported operating systems](https://docs.gitlab.com/ee/administration/package_information/supported_os.html)
- [Reference gitlab architecture](https://docs.gitlab.com/ee/administration/reference_architectures/1k_users.html)
- [Compare gitlab to github](https://www.gitlab.jp/devops-tools/github-vs-gitlab.html)

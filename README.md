## introduction
自社サーバに仮想マシンを立ち上げ、そこにGitLabを導入したので、
備忘録として手順を残しておく。
## spec
|  Device  |  Spec  |
| ---- | ---- |
|  ServerPC  |  Windows Server 2012  |
|  VirtualPC  |  Ubuntu 20.04  |
## manual
サーバPCはある前提
### 仮想マシンを立ち上げ、OSを入れる。
- [仮想マシンを作成する](https://mat0401.info/blog/hyperv-ubuntuserver/)
- [プロキシを設定する](https://qiita.com/daichi-ishida/items/b77c151067427806ede5)
- [curlのプロキシを設定する](https://qiita.com/tkj/items/c6dad4efc0dff4fecd93)
  - [bashrcをリロードする](https://www.itmedia.co.jp/help/tips/linux/l0450.html)
### ネットワークを設定する。
- [ServerPCからVirtualPCにアクセスできるようにする](https://qiita.com/takiru/items/97215e52d8a9525f76c7)
- [自分のPCからVirtualPCにアクセスできるようにする](https://kagasu.hatenablog.com/entry/2018/01/29/184205)
  - [ファイアウォールを設定する](https://knowledge.support.sony.jp/electronics/support/articles/S1206270039326)
### GitLabをインストールする。
- [GitLabをインストールする](https://qiita.com/ryuichi1208/items/1c08523b0ef34d05026f)
  - ["Failed to connect to packages.gitlab.com port 443"のエラーメッセージが出た時の対応](https://forum.gitlab.com/t/problem-installing-latest-version-on-ubuntu-20-04/43621/6)
  - [日本語化する](https://getech-lab.toniemon.com/gitlab-japanese-setting/)
  - [GitLab日本語ドキュメント](https://gitlab-docs.creationline.com/ee/user/group/roadmap/)
### SMTPを設定する。
- [SMTPを設定する](https://docs.gitlab.com/omnibus/settings/smtp.html)
- [メールを送ってみる](http://x68000.q-e-d.net/~68user/unix/pickup?sendmail)
### GitLab Runnerを立ち上げる。
- [GitLab Runnerを立ち上げる](https://qiita.com/sky_jokerxx/items/2a264a0194a5cbc7bd12)
### 他サービスと連携する。
- [integrate Microsoft Teams with GitLab](https://docs.gitlab.com/ee/user/project/integrations/microsoft_teams.html)
## final
- [Supported operating systems](https://docs.gitlab.com/ee/administration/package_information/supported_os.html)
- [Reference gitlab architecture](https://docs.gitlab.com/ee/administration/reference_architectures/1k_users.html)
- [Compare gitlab to github](https://www.gitlab.jp/devops-tools/github-vs-gitlab.html)

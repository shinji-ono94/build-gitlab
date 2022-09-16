# build gitlab (VirtualBox)

## Advance Information
- [Supported operating systems](https://docs.gitlab.com/ee/administration/package_information/supported_os.html)
- [Reference gitlab architecture](https://docs.gitlab.com/ee/administration/reference_architectures/1k_users.html)
- [Compare gitlab to github](https://www.gitlab.jp/devops-tools/github-vs-gitlab.html)

## install manual (Japanese)
- [install virtual machine](https://qiita.com/HirMtsd/items/225c20b77a7cd5194834)
  - [trouble for menu bar and status bar](https://qiita.com/baggio/items/ec7ab5e4bac774c11686)
  - [copy from host to virtual](https://onoredekaiketsu.com/copy-and-paste-with-virtualbox/)
- [install gitlab](https://www.gitlab.jp/install/#ubuntu)
  - [Communication from host to guest](https://qiita.com/zaburo/items/e446f8655a7a28a93d58)
  - [Setup SMTP](https://docs.gitlab.com/omnibus/settings/smtp.html)
  - [How to send mail](http://x68000.q-e-d.net/~68user/unix/pickup?sendmail)
- [Use gitlab](https://tracpath.com/works/development/learn-gitlab-tutorial-for-beginners/#:~:text=%E3%83%AC%E3%83%83%E3%82%B9%E3%83%B3%EF%BC%92%EF%BC%8E%E7%99%BB%E9%8C%B2%E3%81%A8%E6%9C%80%E5%88%9D%E3%81%AE%E3%83%97%E3%83%AD%E3%82%B8%E3%82%A7%E3%82%AF%E3%83%88%E4%BD%9C%E6%88%90%201%20%E3%81%BE%E3%81%9A%E3%80%81GitLab%E3%81%AE%E7%99%BB%E9%8C%B2%E3%83%9A%E3%83%BC%E3%82%B8%E3%81%AB%E3%82%A2%E3%82%AF%E3%82%BB%E3%82%B9%E3%81%97%E3%81%BE%E3%81%99%E3%80%82...%202%20%E5%BF%85%E8%A6%81%E3%81%AA%E6%83%85%E5%A0%B1%E3%82%92%E5%85%A5%E5%8A%9B%E3%81%97%E3%81%A6%E3%81%84%E3%81%8D%E3%81%BE%E3%81%99%E3%80%82...%203%20%E5%85%A5%E5%8A%9B%E3%81%97%E3%81%9F%E3%82%89%E3%80%8CRegister%E3%80%8D%E3%82%92%E6%8A%BC%E3%81%97%E3%81%A6%E3%81%8F%E3%81%A0%E3%81%95%E3%81%84%E3%80%82...%204,...%209%20%E3%83%88%E3%83%83%E3%83%97%E3%83%9A%E3%83%BC%E3%82%B8%E3%81%AB%E6%88%BB%E3%82%8B%E3%81%A8%E3%80%81%E3%83%A1%E3%83%8B%E3%83%A5%E3%83%BC%E3%83%90%E3%83%BC%E3%81%8C%E6%97%A5%E6%9C%AC%E8%AA%9E%E5%8C%96%E3%81%95%E3%82%8C%E3%81%A6%E3%81%84%E3%82%8B%E3%81%A8%E6%80%9D%E3%81%84%20...%2010%20%E3%81%A7%E3%81%AF%E3%80%81%E5%BC%95%E3%81%8D%E7%B6%9A%E3%81%8D%E3%83%97%E3%83%AD%E3%82%B8%E3%82%A7%E3%82%AF%E3%83%88%E3%81%AE%E4%BD%9C%E6%88%90%E3%81%AB%E7%A7%BB%E3%81%A3%E3%81%A6%E3%81%84%E3%81%8D%E3%81%BE%E3%81%99%E3%80%82...%20%E3%81%9D%E3%81%AE%E4%BB%96%E3%81%AE%E3%82%A2%E3%82%A4%E3%83%86%E3%83%A0...%20)
  - [Cooperate Teams](https://zenn.dev/fijii_rin/articles/fda30f4ae04f42)

※以降失敗した時のURL
- [install gitlab](https://tutorialcrawler.com/ubuntu-debian/ubuntu-20-04%e3%81%abgitlab%e3%82%92%e3%82%a4%e3%83%b3%e3%82%b9%e3%83%88%e3%83%bc%e3%83%ab%e3%81%97%e3%81%a6%e6%a7%8b%e6%88%90%e3%81%99%e3%82%8b%e6%96%b9%e6%b3%95/)
  - [install vim](https://qiita.com/tommy_g/items/3ad4b26ccb4893f2760e)
  - [gitlab url from http to https](https://qiita.com/yuuAn/items/09a434d3f6cffa31101e#fn2)
    - [install Let's Encrypt](https://qiita.com/daiki44/items/a3616390f277722b97e0)


## notes
### build gitlab (Docker)
- [install gitlab](https://qiita.com/ryuichi1208/items/1c08523b0ef34d05026f)

# build gitlab (Hyper-V)
## install manual (Japanese)
- [make virtual machine](https://mat0401.info/blog/hyperv-ubuntuserver/)
  - [Set Proxy](https://qiita.com/daichi-ishida/items/b77c151067427806ede5)
  - [Set curl proxy](https://qiita.com/tkj/items/c6dad4efc0dff4fecd93)
    - [reload bashrc](https://www.itmedia.co.jp/help/tips/linux/l0450.html)
  - [gitlab install trouble(Failed to connect to packages.gitlab.com port 443)](https://forum.gitlab.com/t/problem-installing-latest-version-on-ubuntu-20-04/43621/6)
- [Access from Host PC](https://qiita.com/takiru/items/97215e52d8a9525f76c7)
- [Access from my PC](https://kagasu.hatenablog.com/entry/2018/01/29/184205)
  - [Set firewall](https://knowledge.support.sony.jp/electronics/support/articles/S1206270039326) 
- [Oparate gitlab](https://qiita.com/mikoski01/items/7a7795a8a1e98d9ba6d9)
  - [integrate Microsoft Teams with GitLab](https://docs.gitlab.com/ee/user/project/integrations/microsoft_teams.html)
    - [set gitlab proxy](https://qiita.com/nmatayoshi/items/533a93a5d97de18c9e5a)
- [install gitlab runner](https://qiita.com/sky_jokerxx/items/2a264a0194a5cbc7bd12)
  - [gitlab build test deploy](https://qiita.com/bremen/items/f47f383b9931a840a25c)
  - [integrate Eclipse with gitlab](https://qiita.com/neruneruo/items/eefc650ede2bb5efff87)
  - [set proxy for docker](https://qiita.com/Takahiro-Suzuki/items/ceecceb3b7e7f7a49e92)
### Mak gitlab useful
- [gitlab Japanese transport](https://getech-lab.toniemon.com/gitlab-japanese-setting/)
- [gitlab Japanese docs](https://gitlab-docs.creationline.com/ee/user/group/roadmap/)

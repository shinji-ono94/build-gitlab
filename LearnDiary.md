# 2023/05/26
- tetorisプロジェクトを作成  
- テトリスの枠までをWebにホストするPG作成  
- gitlabにプッシュすると、gitlabサーバ上のlocalhostにwebアプリが立ち上がる仕組み完成
	- 残課題
		- ポート番号変更する。
		- webのポート番号を開放する。
		- before_scriptを修正する。

【学び】
gitlab-runnerをdockerで立ち上げると、立ち上がったwebアプリを覗きに行けない。shellで立ち上げる必要がある。
shellでコマンドを実行すると権限が無い。/etc/sudoersに権限を付与する必要がある。
/usr/localも上記権限では触れないので、別フォルダにする。

【コマンド】
sudo su - ユーザ名						ユーザ名でコマンド実行
usermod -aG グループ名 ユーザ名			ユーザ名をグループに入れる。
pwd										自分の居場所把握
sudo docker ps							dockerの現在の情報確認

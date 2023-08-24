# Git Lesson

## リモートリポジトリとローカルリポジトリとはそれぞれ何でしょうか？
* どちらもファイルやディレクトリの状態や変更履歴が記録される場所である
* リモートリポジトリはネット上にあるため、他の人たちと内容を共有することができる
* 一方ローカルリポジトリは個々人が使用するため、自分のPC上にあり、他の人がアクセスしたり変更を加えることは出来ない
* ローカルリポジトリで行った、例えば作成物や変更等をリモートリポジトリにアップロードすることで他の共同作業者も情報を取得できるようになり、またローカルリポジトリに分けることで作業を分担することができる


## プッシュとマージの違いは何でしょうか？
* プッシュ
  * ローカルリポジトリの内容をリモートリポジトリに反映させること
* マージ
  * ブランチに他のブランチの変更内容を取り込むこと


## コミットとプッシュの違い
* コミット
  * セーブのようなもので、変更内容を保存しログを残すコマンド
  * 〇〇という変更を行いましたよ、というメッセージを残すのが一般的
* プッシュ
  * 保存した変更内容をリポジトリに反映させること


## コミットのメッセージはどのように書いてあげるのが最適でしょうか？
* どのような変更を行ったのかを簡潔に、誰が見てもわかりやすいよう記載する


## ローカルでマージするフローと、プルリクエストでマージするフローの違いは何でしょうか？
* ローカルでマージ
  * 自分以外の目が入らないまま変更内容がリモートリポジトリのmasterブランチに反映されてしまう
* プルリクエストでマージ
  * マージ前に変更内容に欠陥が無いか他人が確認することができ、修正を行うことも出来る


## コンフリクトを起こしてしまった場合、どう対処すべきですか？
* まず、先にマージされた変更内容を取り込むか、後にマージしようとしている変更内容を取り込むか、両方の変更内容を取り込むか考える必要がある
* 前者2つであればどちらかを選んでマージを行えば良いが、後者の場合はエディタに両方の変更内容を合わせたソースコードを入力しマージする処置をする。この際、コンフリクト解決で行った作業内容をコミットする
* 被ってしまった相手がマージしたソースコードが何のためのコードなのか読み取れないと判断できないので、意図がわからない場合は相手と相談することも大切である
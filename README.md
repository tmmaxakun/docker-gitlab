# Gitlab with Docker
公式ガイド：https://docs.gitlab.com/ee/install/docker.html

## CI/CD
なんちゃってCi/CD構想
* Mintのクローンを用意
  * .150->Production .151->Devlopment
* Gitlab Runnnerのスクリプトを利用
  * devブランチへのコミット -> dev環境に乗り込んで、スクリプト実行
    * ルータのポートマッピングを変更して、Internetから確認
  * masterブランチへのコミット（merge）-> Prod環境に乗り込んで、スクリプト実行

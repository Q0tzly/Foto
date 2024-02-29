# Foto
これら３つをパッケージとしてまとめたもの

# FotoHash (clt)
写真をハッシュ化して管理するツール

## cmd
fotohash
- init          写真のハッシュ値と写真を管理するディレクトリを作成。
- rest          写真のハッシュ値と写真を管理するディレクトリを削除。
- hash <PATH>   写真の名前をHash化する。
- add <PATH>    写真のHash値を検証して管理下におく。
- remove <HASH> Hash値の写真を管理下より外す。(写真は削除されない)
- put <HASH>    Hash値の写真をパスとともに表示する。(表示できるのはchafaコマンドが入ってる場合のみ)


# FotoUp (clt)
FotoHashで管理されている写真をFotoWebにアップロードしたりFotoWebから削除したりするツール

## cmd
fotoweb
- upload <HASH>   Hash値の写真のページを作成する。
- remove <HASH>   Hash値の写真のページを削除する。
- download <HASH> Hash値の写真をダウンロードする。


# FotoWeb (ws)
FotoUpからデータを受け取ってWebサーバーとしてページを立ち上げる。
crates.ioの様にすぐに反映される。
Webサーバーであり写真のディレクトリの管理をする。

## idea
- リンクもHash値から取ることができる。

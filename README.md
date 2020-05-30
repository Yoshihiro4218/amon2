# amon2
amon2 on docker

# build後
- amon2とPlackインストール
`docker-compose run --rm perlcli carton install`

- サンプルアプリ作成
`docker-compose run --rm perlcli carton exec -- amon2-setup.pl --flavor=Lite myapp`
# 前提条件
・dockerがインストールされていること
・docker-compodr ガインストールされていること

# 起動方法

docker-compose up 


a.comにアクセスするとnginx_aにアクセスし
b.comにアクセスするとnginx_bにアクセスします。

nginx_r.confの
upstream nginx_a {
    server nginx_a:80;
}
や、

upstream nginx_b {
    server nginx_b:80;
}
を変更すれば、任意の場所に転送できます。

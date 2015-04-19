# tutum-node-virtualbox
create tutum node on virtualbox

### usage

```
PORT=<port> TUTUM_TOKEN=<token> vagrant up
```

portはdocker用。ファイアーウォールのポートフォワード設定でpublic tcp 2375で公開する。

tokenはtutumのBring your own nodeで取得したトークン。
https://dashboard.tutum.co/node/cluster/list/

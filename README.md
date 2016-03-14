Docker Image for [Codenize.tools](http://codenize.tools/)
====

これは何？
----

codenize.tools で公開されているツール類をdocker に閉じ込めたもの

使い方
----

1. イメージの作成 または pull
2. envfile.template を envfile にコピーし、AWS_ACCESS_KEYS/AWS_SECRET_ACCESS_KEYを記述
3. docker-compose を実行(個別にdocker を実行しても良い)
4. settings 以下にファイルができていることを確認する
5. 更新したい場合は docker-compose.yml を修正するか、別に yml ファイルを用意して読み込ませる

### Roadworker (Route53)

```
$ docker-compose run route53
```

### Piculet (Security Group)

```
$ docker-compose run sg
```

### Kelbim (ELB)

```
$ docker-compose run elb
```

### Miam (IAM)

```
$ docker-compose run iam
```

### Eipmap (Elastic IP)

```
$ docker-compose run eip
```

### shell

```
$ docker-compose run shell
```

注意事項
----

envrc の値は ' などで囲まないでください

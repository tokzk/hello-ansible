docker-ansible
====


使い方
---

1. Dockerコンテナの起動

```
$ make up
```

2. Ansibleコンテナに接続

```
$ make ansible
```

3. target01, target02に対し、sshの接続確認

```
ansible$ ssh target01
target01$ exit

ansible$ target02
target02$ exit
```

4. target01, target02に対し、ansibleコマンドの実行

```
ansible$ ansible-playbook -i inventry.ini playbook.yml
```

5. Dockerコンテナの終了

```
$ make down
```

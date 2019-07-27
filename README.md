study k8s
=========================


メモ: 思考整理
-------------------------
- 意図的にエラーを起こしたい
    - 環境構築: kubectlが動くようにする
        - HelloWorldのドキュメント中の kubectl らへんが動けばいい!
        - とりあえずHelloMiniKubeを触ってみる
    - マニフェストファイルを触っていく
        - 正常: DocumentとかのHelloWorld的なやつに乗っているはず
            - コピペして使ってみる
        - 最小: 正常を少しずつ削って最小のマニフェストを目指す


### permission denied問題

minikubeをrootでstartしていたものを
```
$ minikube delete
$ rm -rf ~/.minikube
$ minikube start
```
https://github.com/kubernetes/minikube/issues/1899


### 疑問
hello nodeのnodeの意味はnode.jsのnode?
それともkubernetes cluster中のnode?

serviceたててアクセスするIPは誰が持っているIP?

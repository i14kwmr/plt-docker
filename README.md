# plt-docker



## Usage

〜Docker入る前〜

1. [リポジトリ](https://github.com/YoshikiMas/plt-docker.git)をダウンロード

```
git clone https://github.com/YoshikiMas/plt-docker.git
```

2. Dockerイメージを作成

* MakefileのIMAGE_TAGは適宜変更

```
make build
```

3. Dockerを起動

* Makefileの23,24行目はコメントアウト（環境依存の記述）

```
make run
```



〜Docker入った後〜

4. Dockerfileで設定した環境に切り替え

```
conda activate pytorch-lightning
```

5. 設定完了．プログラムを動かすことができる．



## 注意点

* minicondaを利用
* 機械学習用と音用のライブラリが重い (14.4G)
  * 適宜，Dockerfileから記述を減らすと良い．


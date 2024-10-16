# sbtのインストールとハローワールド

## はじめに

ハローワールドできたら、うれしいと思った。

## 前提

- Apple シリコン搭載の Mac コンピュータ
- Homebrew

## Installation

Homebrew で sbt をインストールする。

```
% brew install sbt
```

実行後 sbt の状況を確認する。

```
% sbt -V
sbt script version: 1.10.2
```

## Hello, World! に挑戦

まず `Main.scala` を作成。

```
mkdir -p src/main/scala
echo 'object Main extends App { println("ハローワールド") }' > src/main/scala/Main.scala
```

次に sbt を起動。

```
% sbt
[info] welcome to sbt 1.10.2 (Homebrew Java 23)
[info] loading project definition from /Users/ririumu/dev/github/learning-scala/project
[info] set current project to learning-scala (in build file:/Users/ririumu/dev/github/learning-scala/)
[info] sbt server started at local:///Users/ririumu/.sbt/1.0/server/33e2c1f364e4c22ae311/sock
[info] started sbt server
sbt:learning-scala> 
```

sbt シェルに `run` と打ち込むと、コードの実行がなされる。

```
sbt:learning-scala> run
[info] compiling 1 Scala source to /Users/ririumu/dev/github/learning-scala/target/scala-2.12/classes ...
[info] running Main 
ハローワールド
[success] Total time: 1 s, completed 2024/10/16 20:39:22
```

ハローワールドができた！

## まとめ

ハローワールドできたので、うれしかった。

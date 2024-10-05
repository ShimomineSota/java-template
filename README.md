# Java環境構築

## 初めに

devcontainer上でJava環境の構築に関する備忘録  

## 前提条件

- VisualStudioCodeがインストールされている  
- DevContainers拡張機能がインストールされている  
- Docker環境が構築されている  

## 環境

- 公式イメージでは、git等の開発ツールはインストール済み  
- 公式が準備しているイメージでは、MS製のJDKに限られるため、SDKMAN!経由でインストール
  [https://github.com/devcontainers/features/tree/main/src/java](https://github.com/devcontainers/features/tree/main/src/java)
- SpringBoot使用の際は、コメントアウトを解除

## 参照情報

- Microsoft Debian Container  
  [https://github.com/devcontainers/images/tree/main/src/base-debian](https://github.com/devcontainers/images/tree/main/src/base-debian)  
- Dev Container Matadata  
  [https://containers.dev/implementors/json_reference/](https://containers.dev/implementors/json_reference/)
- Dev Container Features  
  [https://containers.dev/features](https://containers.dev/features)  

## バグ情報 (2024/10/5)

- `ghcr.io/devcontainers/features/java:latest`でビルドエラーが発生  
  `ghcr.io/devcontainers/features/java:1.5.0`に書き換えることで回避可能  
  [ERROR: Feature "Java (via SDKMAN!)" (ghcr.io/devcontainers/features/java) failed to install!](ghcr.io/devcontainers/features/java:latest)  

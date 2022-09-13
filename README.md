# Bash RC Hack

修改現成環境下的 Bash RC。

## Git Ignore

* 在 `packages` 目錄下建立一個 `.gitignore`，檔案內容為：

```bash
*
.*
```

## 使用方式：以 Docker 為例

* 在 Docker 容器中，進到專案根目錄，執行 `./packages/myrc/lnrc` 即可
* 有新修改，不想 `exit` 出去再進來時，執行 `source $HOME/.bashrc` 即可

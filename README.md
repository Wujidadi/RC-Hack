# RC Hack

修改現成 Docker 環境（講白話點，就是別人建立的 Docker image，而不是我自己生產的）下的 Run Commands。

本專案中依資料夾區分環境：

* **HS.Docker** - HS 工作中使用的 Docker image

## Git Ignore

* 此專案中的檔案因為都用在大家共用的環境下，為了不影響別人，所以需要用 `.gitignore` 忽略掉這些檔案

* 在 `packages` 目錄下建立一個 `.gitignore`，檔案內容只有以下 2 行 3 個字元：

  ```bash
  *
  .*
  ```

* 本專案中的 `.gitignore` 不實際寫入以上內容，以免其他檔案被忽略掉（至少在本專案內要保留吧喂！）

## 使用方式：以 Docker 為例

* 在 Docker 容器中，進到專案根目錄，執行 `./packages/myrc/run` 即可
* 有新修改，不想 `exit` 出去再進來時，執行 `source $HOME/.bashrc` 或 `source $HOME/.vimrc` 即可

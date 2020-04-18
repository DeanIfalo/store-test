## 大廳 (登入成功後)

* 未使用的暫不列出

### 請求

### `login`
```shell
請求登入, 回應0代表成功
```
#### `getBaccaratTableStatus`
```shell
請求各桌檯狀態, 會回應各桌檯狀態表
```
#### `getOpeningTimes`
```shell
請求訂閱 各桌開放時間列表, 請求成功回應0, 之後會在訂閱中持續收到
```

### 訂閱[create an anchor](#roadMapMessageReceived)

#### `getUserCred`
```shell
收到user初始資料
```
### [Ready, set, GO!](#login)
#### `itinitialCasinoTable`
```shell
各table資料初始完成, 此時可以進入大廳
```
#### `updateOpeningTimes`
```shell
會重複收到, 用來更新桌檯在關閉中時, 所顯示的開放時段
```
#### `gameStatusUpdateMessageReceived`
```shell
會重複收到, 用來通知某一桌變更 牌局狀態 和 更新桌檯資料
```
#### `updateJackpotPoolAmount`
```shell
會重複收到, 更新jp獎池數字
```
#### `roadMapMessageReceived`
```shell
會重複收到, 用來通知某一桌的路圖要更新
```
#### `updateGameStatuskickUser`
```shell
收到時, 要跳窗顯示斷線原因
```

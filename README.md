## 部署開發用 Redis
- :warning: 此部署僅為測試環境開發階段使用，為單節點配置，如需部署至 Production 環境，請另外修改配置設定, 不要直接使用
- :information_source: 這部署並無配置永久資料儲存功能(符合開發情境提供快速還原乾淨環境的作法)，只要專案 repo 有commit更動就會進行資料重置，請commit/push前要謹慎注意。

## 使用說明

### 啟動自動匯入資料的方式

1. 目前 [Redis](https://hub.docker.com/_/redis) 使用 6.2.11 的版本，可依需求進行調整。
2. 可修改 k8s/redis-config.yaml 內的設定內容。
3. 建置完成後，請從「實證環境」中的服務獲取連線 port 進入使用。
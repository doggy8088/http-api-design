# HTTP API 設計指南

## 簡介

這份指南講述出自於 [Heroku Platform API](https://devcenter.heroku.com/articles/platform-api-reference)
的 HTTP + JSON API 設計方式，原本的點子來自 [Wesley Beary](https://github.com/geemus) 等人的 
[HTTP API Design Guide](https://github.com/interagent/http-api-design)。

除了提到 API 本身之外，也介紹了 Heroku 內部 API，希望 Heroku 以外的 
API 設計者也會感到興趣。

我們的目標是一致性並專注在商務邏輯，避免被瑣事耽擱。尋求的雖未必是 
API 設計的**終極之道**，但卻是**健全、一致，且有完整文件的方法**。

我們假設您已熟悉基本的 HTTP + JSON API，因此本指南不會涵蓋所有的基本知識。

歡迎一同為這份指南[貢獻心力](https://github.com/kcyeu/http-api-design/blob/master/CONTRIBUTING.md)，本書的[貢獻者見此](https://github.com/kcyeu/http-api-design/blob/master/CONTRIBUTORS.md)。

## 版本

 * 15.02.0
   * 新增章節: 基礎/少些顧慮
   * 潤飾部分章節文句
   * 對應[版本](https://github.com/interagent/http-api-design/commit/232f8dc6a941d0b25136bf64998242dae5575f66) (232f8dc)
 * 14.12.0
   * 初版，對應[版本](https://github.com/interagent/http-api-design/commit/c3a69b530274e2f776b2030f9ed790af0f6cbf3d) (c3a69b5)

# HTTP API 設計指南

## 簡介

這份指南講述了出自於 [Heroku Platform API](https://devcenter.heroku.com/articles/platform-api-reference)
的 HTTP + JSON API 的設計方式。

這份指南除了提到 API 之外，也介紹了 Heroku 內部的 API，希望 Heroku 
以外的 API 設計者也會感到興趣。

我們的目標是一致性並專注在商務邏輯，避免被瑣事耽擱。尋求的是
**健全、一致，且有完整文件的方法** 來設計 API，而非**唯一或理想的方法**。

我們假設您已熟悉基本的 HTTP + JSON API，所以本指南不會涵蓋所有的基本知識。

歡迎貢獻心力一同為這份指南[貢獻心力](CONTRIBUTING.md)。

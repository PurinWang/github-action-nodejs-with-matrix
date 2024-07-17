# github-action-nodejs-with-matrix
# English
use github action to verified node js and typescript with matrix to multiple version

## how to use

create a yaml in .github/workflows
```
mkdir .github/workflows
cd .github/workflows && touch ci.yaml
```
copy this repo ci.yaml content and paste it in your yaml

## note
- node_version is setting in strategy > matrix and it is array, you could change any you want to test node version.
- if you don't have typescript, you could pass Testing type-check.
- Testing build with my package.json config is setting npm run build:direct, in your case it would be npm run buid.


---
# chinese
使用 github action 驗證 node js 及 typescript 搭配 matrix 多版本測試

## 如何使用
新增一個yaml在 .github/workflow
```
mkdir .github/workflows
cd .github/workflows && touch ci.yaml
```
複製這個 repo 的 ci.yaml 內容貼到 yaml 中

## 注意事項
- node_version 設定在 strategy > matrix，是個陣列可以自行更換
- 如果沒有使用 typescipt，可以註解略過 Testing type-check
- Testing build 在我的 package.json 設定是 npm run build:direct，你可以換成 npm run build

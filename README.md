## jieba-seg-api-heroku
將[jieba](https://github.com/fxsjy/jieba)部署到heroku上，實現斷詞API

### 部署指令
先確認有設置好heroku
```
git clone https://github.com/marvincwhuang/jieba-seg-api-heroku.git
cd jieba-seg-api-heroku 
heroku create
git push heroku master
```
### Query Mode
```
https://XXXXXX-XXXXX-XXXXX.herokuapp.com/seg?q=將jieba部署到heroku上，實現斷詞API
```
### Post Request
直接對https://XXXXXX-XXXXX-XXXXX.herokuapp.com/seg 執行post request
```
"將jieba部署到heroku上，實現斷詞API"
```
### Results
```
{
  resCode: 0,
  resMsg: "ok",
  resData: [
    "將",
    "jieba",
    "部署",
    "到",
    "heroku",
    "上",
    "，",
    "實現",
    "斷詞",
    "API"
  ]
}
```
若無結果
```
{
resCode: -1,
resMsg: "no seg result",
resData: null
}
```

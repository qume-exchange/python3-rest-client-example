Qume Python3 Sample REST API Client
==================================
Example of a RESTful application for the [Qume Sandbox](https://sandbox.qume.io). Makes a call to each REST endpoint.


Quick Start
---------------

1. Edit `application.py` by entering your account details (API keys, passphrase, etc.)
2. Run `application.py` after you review the script

Hints
----------------------

* Make sure you are using Python3
* To generate API keys, go to the "Accounts" page on the [Qume Sandbox](https://sandbox.qume.io)

Application Sample Output
-------------------------

The following is some of what you can expect when running this application:

```
 {"status":"OK","bids":[{"price":104005,"amount":1},{"price":104000,"amount":21},{"price":101985,"amount":3},{"price":101950,"amount":1},{"price":101100,"amount":1},{"price":100000,"amount":2},{"price":99995,"amount":5},{"price":90000,"am
ount":3}],"asks":[{"price":70000,"amount":1000},{"price":105000,"amount":40},{"price":106000,"amount":1},{"price":107005,"amount":1},{"price":108000,"amount":1},{"price":109000,"amount":1},{"price":109500,"amount":1},{"price":110000,"amou
nt":21},{"price":110505,"amount":1},{"price":111505,"amount":1}]}
get_funding_rate:
 {"fundingRate":{"value":0.0044997536353281,"timestampNs":1568473741000000000}}
get_index_price:
 {"indexPrice":10350.51}
get_mark_price:
 {"markPrice":10402.26}
place_order:
 {"transactTime":"2019-09-14T15:09:05.793678165Z00:00","orderId":1568338161669597403,"symbol":"BTCUSDQ","side":"BUY","price":10000,"orderQty":0.001,"cumQty":0,"leavesQty":0.001,"orderType":"LIMIT","timeInForce":"UNTIL_CANCEL","stopTrigger
":"MARK_PRICE"}
place_stop_order:
 {"transactTime":"2019-09-14T15:09:06.999006784Z00:00","orderId":1568338161669597405,"symbol":"BTCUSDQ","side":"SELL","price":11000,"orderQty":0.001,"cumQty":0,"leavesQty":0.001,"orderType":"STOP_LIMIT","timeInForce":"UNTIL_CANCEL","stopT
rigger":"MARK_PRICE","stopPrice":100}
get_active_orders:
 {"status":"OK","orders":[{"ts":"2019-09-14T00:48:34.119882609Z00:00","id":1568338161669597355,"price":11000,"qty":0.02,"symbol":"BTCUSDQ","side":"SELL","originalQty":0.02,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:
48:57.279819705Z00:00","id":1568338161669597357,"price":11150.5,"qty":0.001,"symbol":"BTCUSDQ","side":"SELL","originalQty":0.001,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:49:08.366223755Z00:00","id":156833816166959
7359,"price":10400.5,"qty":0.001,"symbol":"BTCUSDQ","side":"BUY","originalQty":0.001,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:49:16.687526934Z00:00","id":1568338161669597361,"price":10000,"qty":0.001,"symbol":"BTC
USDQ","side":"BUY","originalQty":0.001,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:49:27.539655813Z00:00","id":1568338161669597363,"price":11050.5,"qty":0.001,"symbol":"BTCUSDQ","side":"SELL","originalQty":0.001,"typ
e":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:50:14.082778443Z00:00","id":1568338161669597370,"price":10400,"qty":0.001,"symbol":"BTCUSDQ","side":"BUY","originalQty":0.001,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts"
:"2019-09-14T00:50:27.062835308Z00:00","id":1568338161669597372,"price":10900,"qty":0.001,"symbol":"BTCUSDQ","side":"SELL","originalQty":0.001,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:50:42.271188487Z00:00","id":1
568338161669597374,"price":10950,"qty":0.001,"symbol":"BTCUSDQ","side":"SELL","originalQty":0.001,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:50:50.848749574Z00:00","id":1568338161669597376,"price":10800,"qty":0.001,
"symbol":"BTCUSDQ","side":"SELL","originalQty":0.001,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:50:58.877176871Z00:00","id":1568338161669597378,"price":10700.5,"qty":0.001,"symbol":"BTCUSDQ","side":"SELL","originalQ
ty":0.001,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:51:11.509085791Z00:00","id":1568338161669597380,"price":10600,"qty":0.001,"symbol":"BTCUSDQ","side":"SELL","originalQty":0.001,"type":"LIMIT","timeInForce":"UNTIL
_CANCEL"},{"ts":"2019-09-14T00:51:55.402349005Z00:00","id":1568338161669597382,"price":10110,"qty":0.001,"symbol":"BTCUSDQ","side":"BUY","originalQty":0.001,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:52:10.737081447
Z00:00","id":1568338161669597384,"price":10195,"qty":0.001,"symbol":"BTCUSDQ","side":"BUY","originalQty":0.001,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:52:26.440923322Z00:00","id":1568338161669597386,"price":10198
.5,"qty":0.001,"symbol":"BTCUSDQ","side":"BUY","originalQty":0.001,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:52:55.030671885Z00:00","id":1568338161669597388,"price":10198.5,"qty":0.002,"symbol":"BTCUSDQ","side":"BU
Y","originalQty":0.002,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:53:14.910717500Z00:00","id":1568338161669597390,"price":9000,"qty":0.003,"symbol":"BTCUSDQ","side":"BUY","originalQty":0.003,"type":"LIMIT","timeInFo
rce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:53:33.066443447Z00:00","id":1568338161669597392,"price":9999.5,"qty":0.005,"symbol":"BTCUSDQ","side":"BUY","originalQty":0.005,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:54:
04.934873431Z00:00","id":1568338161669597394,"price":10400,"qty":0.02,"symbol":"BTCUSDQ","side":"BUY","originalQty":0.02,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T00:54:36.636348005Z00:00","id":1568338161669597396,"pr
ice":10500,"qty":0.04,"symbol":"BTCUSDQ","side":"SELL","originalQty":0.04,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T15:06:49.291741192Z00:00","id":1568338161669597399,"price":7000,"qty":1,"symbol":"BTCUSDQ","side":"SE
LL","originalQty":1,"type":"STOP_LIMIT","timeInForce":"UNTIL_CANCEL","triggerType":"MARK_PRICE","triggerPrice":100},{"ts":"2019-09-14T15:08:06.573585244Z00:00","id":1568338161669597400,"price":10000,"qty":0.001,"symbol":"BTCUSDQ","side":"
BUY","originalQty":0.001,"type":"LIMIT","timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T15:08:07.510194813Z00:00","id":1568338161669597402,"price":11000,"qty":0.001,"symbol":"BTCUSDQ","side":"SELL","originalQty":0.001,"type":"STOP_LIMIT",
"timeInForce":"UNTIL_CANCEL","triggerType":"MARK_PRICE","triggerPrice":100},{"ts":"2019-09-14T15:09:05.793678165Z00:00","id":1568338161669597403,"price":10000,"qty":0.001,"symbol":"BTCUSDQ","side":"BUY","originalQty":0.001,"type":"LIMIT",
"timeInForce":"UNTIL_CANCEL"},{"ts":"2019-09-14T15:09:06.999006784Z00:00","id":1568338161669597405,"price":11000,"qty":0.001,"symbol":"BTCUSDQ","side":"SELL","originalQty":0.001,"type":"STOP_LIMIT","timeInForce":"UNTIL_CANCEL","triggerTyp
e":"MARK_PRICE","triggerPrice":100}]}
get_order_status:
 {"status":"OK","order":{"ts":"2019-09-14T00:48:34.119882609Z00:00","id":1568338161669597355,"price":11000,"qty":0.02,"userId":"5138405f-920f-5f23-9b8c-e83b655824e2","symbol":"BTCUSDQ","side":"SELL","originalQty":0.02,"type":"LIMIT","time
InForce":"UNTIL_CANCEL"}}
delete_active_order:
 {"error":"order with given id does not exist","code":9,"message":"order with given id does not exist","details":[{"typeUrl":"type.googleapis.com/com.qume.orderbook.EngineError","value":"CAU="}]}
get_trade_history:
 {"status":"OK","trades":[{"symbol":"BTCUSDQ","makerside":"BUY","makerOrderId":1568211784768163447,"takerOrderId":1568211784768163450,"price":10125,"qty":0.02,"ts":"2019-09-11T22:03:02.687953868Z00:00","id":1568211784768163451},{"symbol":
"BTCUSDQ","makerside":"BUY","makerOrderId":1568338161669597327,"takerOrderId":1568338161669597330,"price":10200,"qty":0.01,"ts":"2019-09-13T18:44:00.569943746Z00:00","id":1568338161669597331},{"symbol":"BTCUSDQ","makerside":"BUY","makerOr
derId":1568338161669597353,"takerOrderId":1568338161669597365,"price":10500,"qty":0.001,"ts":"2019-09-14T00:49:47.461683304Z00:00","id":1568338161669597366},{"symbol":"BTCUSDQ","makerside":"BUY","makerOrderId":1568338161669597353,"takerOr
derId":1568338161669597365,"price":10500,"qty":0.001,"ts":"2019-09-14T00:49:47.461683304Z00:00","id":1568338161669597366}]}
edit_position_leverage:
 {"error":"insufficient funds","code":9,"message":"insufficient funds","details":[{"typeUrl":"type.googleapis.com/com.qume.orderbook.EngineError","value":"CAE="}]}
get_wallets:
 {"wallets":[{"walletId":"fbe42f05-6e12-3114-b251-5a7ffe657aeb","asset":"TUSD"}]}
get_wallet_state:
 {"availableBalance":"1.759485","balance":"1.759485","orderMargin":"7.161515","fee":"0","positions":["BTCUSDQ"],"enabled":true}
get_all_positions:
 {"positions":[{"symbol":"BTCUSDQ","position":{"id":"BTCUSDQ","contract":{"id":"BTCUSDQ","notional":"0"},"orderMargin":"4.8894758","initialMargin":"0","entryValue":"0","leverage":100,"realizedPnl":"0"}}]}
```

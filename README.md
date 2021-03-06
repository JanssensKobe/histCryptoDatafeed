# FEDA
A user-friendly library to fetch kline (ohlcv) data from several crypto exchanges.

## Install
```shell
git clone https://github.com/JanssensKobe/feda
```

## Getting Started

This simple script will fetch the kline data from LINK/USDT for the last 170 days on bybit and save this data into a file.
```python
from feda import Feda

datamanager = Feda(fileName='data/ohlcv_bybit_LINKUSDT_170days.json', pair='LINK/USDT', days=170, strExchange='bybit')

ohlcv = datamanager.fetchDatafeed() # Fetch klines and output them into given file
```


## Supported Exchanges
| Logo        | Exchange        | strExchange    |
| ----------- | --------------- | -------------- |
| [![binance](https://user-images.githubusercontent.com/1294454/29604020-d5483cdc-87ee-11e7-94c7-d1a8d9169293.jpg)](https://www.binance.com/en/register?ref=35973916) | [Binance](https://www.binance.com/en/register?ref=35973916) | binance |
| [![binance futures](https://user-images.githubusercontent.com/1294454/29604020-d5483cdc-87ee-11e7-94c7-d1a8d9169293.jpg)](https://www.binance.com/en/register?ref=35973916) | [Binance Futures](https://www.binance.com/en/register?ref=35973916) | binanceFutures |
| [![ftx](https://user-images.githubusercontent.com/1294454/67149189-df896480-f2b0-11e9-8816-41593e17f9ec.jpg)](https://ftx.com/#a=1623029) | [FTX](https://ftx.com/#a=14595372) | ftx |
| [![bybit](https://user-images.githubusercontent.com/51840849/76547799-daff5b80-649e-11ea-87fb-3be9bac08954.jpg)](https://www.bybit.com/app/register?ref=X7Prm) | [Bybit](https://www.bybit.com/en-US/invite?ref=wgPqr) | bybit |

## TODO
* Add more exchanges
* Add support for csv

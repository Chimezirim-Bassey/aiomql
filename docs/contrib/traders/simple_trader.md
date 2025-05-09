# SimpleTrader

## Table of Contents
- [SimpleTrader](#simple_trader.simple_trader)
- [place_trade](#simple_trader.place_trade)


<a id="simple_trader.simple_trader"></a>
### SimpleTrader
```python
class SimpleTrader(Trader)
```
A simple trader that places trades.


<a id="simple_trader.place_trade"></a>
#### place_trade
```python
async def place_trade(*, order_type: OrderType, sl: float, parameters: dict = None)
```
Places a trade based on the order_type and a given stop_loss. The volume is based on the amount to risk which is
calculated using the Risk Assessment Management instance.

#### Parameters:
| Name | Type | Description |
| ---- | ---- | ----------- |
| `order_type` | OrderType | The order_type |
| `sl` | float | The stop_loss |
| `parameters` | dict | Parameters associated with the trade |

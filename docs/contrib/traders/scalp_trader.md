# ScalpTrader

## Table of Contents
- [scalp_trader](#scalp_trader)
- [ScalpTrader](#scalp_trader.scalp_trader)
- [place_trade](#scalp_trader.place_trade)

<a id="scalp_trader"></a>
### ScalpTrader
<a id="scalp_trader.scalp_trader"></a>

```python
class ScalpTrader(Trader)
```
Place trades and record them in the trade_record file. Places trade without stop_loss or take_profit.

<a id="scalp_trader.place_trade"></a>
#### place_trade

```python
async def place_trade(*, order_type: OrderType, volume: float = None, parameters: dict = None)
``
Places a trade based on the order_type and volume. The volume is optional. If not provided, the minimum volume
for the symbol will be used. This trade is placed without a stop_loss or take_profit. The trade is recorded in the
trade_record file.

#### Parameters:
| Name | Type | Description |
| ---- | ---- | ----------- |
| `order_type` | OrderType | The order_type |
| `volume` | float | The volume to trade |
| `parameters` | dict | Parameters associated with the trade |

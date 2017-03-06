# Order Limits

**Maximum active orders:    
**This limits the total number of active trades plus pending orders allowed at any one time for the unique EA identifier. If there happens to be multiple EA’s running with the same unique EA identifier, then this limit will apply across all orders created from these EA’s.

**Maximum active orders for a symbol:    
**This limits the total number of active trades plus pending orders allowed at any one time for the combination of unique EA identifier and currency pair symbol. If there happens to be multiple EA’s running with the same unique EA identifier, then this limit will apply across all orders created from these EA’s.

**Maximum active orders for a time frame:    
**This limits the total number of active trades plus pending orders allowed at any one time for the combination of unique EA identifier and time frame. If there happens to be multiple EA’s running with the same unique EA identifier, then this limit will apply across all orders created from these EA’s.

**Maximum Orders opened for a zone:    
**This limits the number of orders that can be opened due to the retest of the same zone. Included in the count is active trades, pending orders and trades that have already been closed \(so long as they available in the Metatrader trade history window\).

**Maximum Orders opened for a candle:    
**This limits the number of orders that can be opened due to the retest of multiple zones within the same window. Included in the count is active trades, pending orders and trades that have already been closed \(so long as they available in the MetaTrader trade history window\). This parameter is generally useful when there are two or more zones very close to each other \(or overlapping\) and you only want the first one to trigger within the same candle.


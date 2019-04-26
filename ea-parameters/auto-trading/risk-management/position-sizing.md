# Position Sizing

## **Use fixed lot size:**

If set to true, the EA will use a fixed lot size for every order it places. The lot size is determined by the value of the following parameter named “Fixed lot size if applicable”

## **Fixed lot size if applicable:**

Works in conjunction with the parameters “use fixed lot size” and is the position size to use for new orders placed by the EA.

## **Percent of balance to risk:**

If a fixed lot size is not being used, the EA will try to calculate a lot size based on the size of the stop being used and the percentage of account balance to risk. This parameter sets the percentage of the account balance to risk for any one trade.

## **Base lot size on account balance:**

When set to true and the EA is calculating an order position size based on the percentage of balance to risk, the balance used will be taken from the value of “Balance to base lot size if not account balance”, rather than the actual account balance. This may be useful if you only want the position size to change after every month or when a certain increase in balance has been achieved, not every time the account balance increases or decreases. It gives much more control over how the position size for new trades is increased over time.

## **Balance to base lot size if not account balance:**

If “Base lot size on account balance” is false, the position size will be calculated using the account size value of this parameter.

## **Use account balance if smaller than set value:**

When “Base lot size on account balance” is false and the position size is to be calculated using the value entered in “Balance to base lot size if not account balance”, the account balance will still be used if the manually entered balance is greater than the actual account balance. This means the position size will not be increased if the actual balance drops below the manually entered balance.

## **Cap on lot size to use per trade:**

Sets the maximum lot size that can be used for any order, regardless of any other calculation. This can be used as a safety mechanism to ensure an excessively large position size is not used.


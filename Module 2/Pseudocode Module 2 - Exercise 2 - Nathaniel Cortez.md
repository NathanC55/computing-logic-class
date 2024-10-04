>The program determines a monthly checking account fee.


## Named constants and variables

```
set OVERDRAWN_FEE_PERCENTAGE = 0.01
set FEE_PER_OVERDRAWN = 5
```
## Main Program
```
start
    call InputData
    call CalculateFee
    call OutputResults
end
```
## Input Data Module

```
InputData
    print "Enter the account balance:"
    input accountBalance
    print "Enter the number of times the account was overdrawn:"
    input overdrawnTimes
end
```

## Calculate Fee Module

```
CalculateFee
    calculate overDrawnFee = (accountBalance * OVERDRAWN_FEE_PERCENTAGE) + (FEE_PER_OVERDRAWN * overdrawnTimes)
    calculate newAccountBalance = accountBalance - overDrawnFee
end
```

## Output Results Module
```
OutputResults
    print "The fee calculated is: $" + overDrawnFee
    print "The new account balance is: $" + newAccountBalance
    print "Thanks for using this program!"
end
```
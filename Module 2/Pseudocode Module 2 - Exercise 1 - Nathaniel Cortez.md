> The program calculates the refrigerator capacity in cubic feet by multiplying the height, width, and depth to get cubic inches and dividing by 1728



## Named constants
set CUBIC_INCHES_PER_CUBIC_FOOT = 1728

## Main Program
```
start
    call InputData
    call CalculateCapacity
    call OutputResults
end
```
## Input Data Sub-module

```
InputData
    print "Enter refrigerator model name:"
    input refrigeratorModel
    print "Enter interior height in inches:"
    input heightInInches
    print "Enter interior width in inches:"
    input widthInInches
    print "Enter interior depth in inches:"
    input depthInInches
end
```

## Calculate Capacity Sub-module
```
CalculateCapacity
    set capacityInCubicInches = heightInInches * widthInInches * depthInInches
    compute capacityInCubicFeet = capacityInCubicInches / CUBIC_INCHES_PER_CUBIC_FOOT
end
```
## Output Results Sub-module
```
OutputResults
    print "Refrigerator Model: " + refrigeratorModel
    print "Capacity in cubic feet: " + capacityInCubicFeet
end
```
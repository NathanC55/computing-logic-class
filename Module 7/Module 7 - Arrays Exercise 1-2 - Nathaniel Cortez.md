start
    Declarations
        num i
        num size = 20
        num NUMBERS[size]

    for i = 0 to size - 1 step 1
        output "Enter number ", i + 1
        input NUMBERS[i]
    endfor

    output "Numbers in reverse order:"
    for i = size - 1 to 0 step -1
        output NUMBERS[i]
    endfor
stop

start
    Declirations 
    playerNumbers = []
    num playerEnter  

    while true
        playerEnter = int(input("Enter a number or input 0 to quit: "))
        if playerEnter == 0
            exit loop
        else
            playerNumbers.append(playerEnter)
    endwhile

    sumOfNumbers = sum(playerNumbers)

    print(The sum of all the numbers entered was: " + playerNumbers)

end
    
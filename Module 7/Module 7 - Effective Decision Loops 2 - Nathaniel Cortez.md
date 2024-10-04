start
    // Declarations
    yearsUntilRetirement = 0
    annualSavings = 0
    savingsAtRetirement = 0
    annualExpense = 60000
    interestRate = 0.03
    retirementBalance = 0
    year = 1

   
    yearsUntilRetirement = int(input("Enter the number of years until retirement: "))

    annualSavings = int(input("Enter the amount you will save annually: "))

    
    for year = 1 to yearsUntilRetirement
        savingsAtRetirement = savingsAtRetirement + annualSavings
        savingsAtRetirement = savingsAtRetirement + (savingsAtRetirement * interestRate)
    endfor

    retirementBalance = savingsAtRetirement
    year = 1

    while year <= 30 and retirementBalance > 0
        print("Year: " + year)
        print("Starting balance: " + retirementBalance)

        retirementBalance = retirementBalance - annualExpense

        if retirementBalance > 0
            retirementBalance = retirementBalance + (retirementBalance * interestRate)
        endif

        print("End of year balance: " + retirementBalance)

        year = year + 1
    endwhile

    if retirementBalance <= 0
        print("Your savings will run out after " + (year - 1) + " years in retirement.")
    else
        print("Your savings will last for 30 years in retirement.")
    endif

end


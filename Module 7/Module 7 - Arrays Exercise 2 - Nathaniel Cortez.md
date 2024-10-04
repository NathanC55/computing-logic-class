start
    Declarations
        string addIn
        num totalCost = 2.00 // Base price for coffee is $2.00
        num size = 5
        string ADDINS[size] = "Whipped cream", "Cinnamon", "Chocolate sauce", "Amaretto", "Irish whiskey"
        num PRICES[size] = 0.89, 0.25, 0.59, 1.50, 1.75
        bool found
        
    output "Welcome to Jumpin' Jive Coffee Shop!"
    output "The base price for a cup of coffee is $2.00"
    
    while addIn != "done"
        output "Please enter an add-in or type 'done' to finish your order:"
        input addIn
        
        if addIn != "done" then
            found = false
            // Search for the add-in in the array
            for i = 0 to size - 1 step 1
                if addIn == ADDINS[i] then
                    totalCost = totalCost + PRICES[i]
                    output addIn, " added: $", PRICES[i]
                    found = true
                endif
            endfor
            
            if found == false then
                output "Sorry, we do not carry that add-in."
            endif
        endif
    endwhile
    
    output "Your total order cost is: $", totalCost
stop

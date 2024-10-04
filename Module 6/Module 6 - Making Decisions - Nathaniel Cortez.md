```
START
Declirations 
    num customerTextMessages
    num customerAreaCode
    num customerPhoneNumber
    num monthlyServiceBaseFee = 5
    num firstTextingFee = 0.03
    num secondTextingFee = 0.02
    num taxRate = 0.14
    num totalBill 
    num billingAreaCode

while true
    customerAreaCode = input("Enter your 3 digit Area Code or type ZZZ to exit: ")
    if areaCode == "ZZZ"
        exit loop
    customerPhoneNumber = input("Enter you 7 digit Phone Number: )

    customerTextMessages = input(Enter the number of text messages last month: ")


    totalBill += mothleyServiceFee


    if customerTextMessages > 300
        totalBill +=  (customerTextMessages - 300) * secondTextingFee 
        exit
    else
        if customerTextMessages > 100
            totalBill +=  (customerTextMessages - 100) * firstTextingFee
        endif
    endif

    totalBillWithTax = totalBill * taxRate

    if customerTextMessages > 100
        displayTextingInfo()

    if totalBillWithTax > 10
        displayBillingInfo()

endwhile

while true
    input billingAreaCode = "Enter Area code to see Bills in that area or type 'ZZZ' to exit
    if billingAreaCode == "ZZZ"
        exit loop
    output Billing information for billingAreaCode
endwhile


END



displayTextingInfo()
    output "Your number of text messages is : " customerTextMessages
    output "Your area code and phone number is :" customerAreaCode, customerPhoneNumber
return

displayBillingInfo()
    output "Your Monthly Bill before taxes is: " + totalBill
    output "Your Monthly Bill after taxes is: " + totalBillWithTax
return

```
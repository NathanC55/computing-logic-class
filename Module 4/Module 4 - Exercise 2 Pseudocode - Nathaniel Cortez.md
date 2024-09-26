```
start
    Open the dictionary to the middle page
    Set the targetWord to the word you want to find
    Set the currentPageWord to the first word on the current page

    while currentPageWord is not the same as targetWord
        if currentPageWord comes before targetWord alphabetically
            Flip forward to a page farther in the dictionary
        else
            Flip backward to a page closer to the beginning of the dictionary
        endif

        Set currentPageWord to the first word on the new page
    endwhile

    Print "You found the word!"
end
```
- Precise links go to a particular block 
    - usually they are called [[Block References]], because you are embedding the content of the block somewhere else
    - You generate them by either
        - Right-clicking a bullet point, and then selecting `block ref`

            - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fv8%2Fhelp%2F4D8pWjOjRQ?alt=media&token=c638ed6b-ff9e-46a8-9858-f0e646cdf9f7)
        - or by typing `((` and using the autocomplete

            - 
![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fv8%2Fhelp%2F2FiNk-MYoc?alt=media&token=1bcc769f-092b-4fe1-a6a0-e620591bfc2c)
- Example
    - say I have a collection of statements like these
        - Socrates is a Man
            - certainty:: {{[[slider]]}}
        - Socrates is Mortal
            - certainty:: {{[[slider]]}}
        - All Men are Mortal
            - certainty:: {{[[slider]]}}
    - Then I can reference those statements into a compound statement like this
        - If "Socrates is a Man" and "All Men are Mortal" then "Socrates is Mortal"
            - certainty:: {{[[slider]]}}
            - 
    - I will then see that statement whenever I visit one of the blocks that is referenced within it
        - like this
            - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fv8%2Fhelp%2FbGuVgwv7eo?alt=media&token=5cc08cb5-9668-4812-9084-38cd9cd816cf)

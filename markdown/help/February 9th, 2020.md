- ## Demoing [[Encryption]] #[[New Features]] 
    - Encrypted blocks are now live on Roam
        - To use them type `{{``encrypt}}`
        - Example:: {{encrypt:U2FsdGVkX19IGq42nYT82SQysswn/KYSMDPTJFTe/OV3lmF0BBO1MRb54tBZFZAr}} 
            - Then choose a hint and passphrase for that block
                - The passphrase for this [block](((RsNzjvI5f))) is `test` 
            - clicking the lock - or the text area will show you what the sting looks like when sent to us
            - only the hint is stored with Roam - the passphrase never goes to our servers
            - # WARNING
                - if you edit the text of the encrypted string - you will likely lose all of the data (only edit it when it is decrypted)
- Markdown links can be used as aliases for [[Block References]] and [[Bidirectional Links]] #[[New Features]] 
    - All Men are Mortal
    - Socrates is Mortal
    - If [x](((DjhGC4Ppy))) then [y](((YdZn32tkw))) 
        - refresh your page if you don't see this ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fv8%2Fhelp%2FAIEro4drl0?alt=media&token=91e6c400-e244-4e16-8c3c-aff180ffb19b)
    - Example with aliases for pages
        -  I have a page for [[Writers]]
        - and I want to talk about how 
            - [[Paul Graham]] [wrote]([[Writers]]) [[The Age of the Essay]]
            - or [germans]([[Germany]])    
        - Examples of multi-word
            - [ISAs]([[Income Share Agreements]])
            - test whether this appears [x](((XFgHjPHJy)))
- ## #[[New Features]] - [[Query]] component
    - How it works
        - ```
{{query: {and: [[TODO]] 
          {not: 
           {or: [[Example]] [[Demo]]}}}}

will return all TODOs 
 that are not also tagged with Example or Demo
```
        - **TODOs which are not Demos or Examples** {{[[query]]: {and: [[TODO]] {not: {or: [[Demo]] [[Example]]}}}}}
        - How to write [Queries in Roam]([[Query]])
            - There are three logical operators 
                - and
                - or
                - not
            - A query can look for block or page references
            - Queries look like this
            - `{` {{or: or: | not: | and:}}  {{or: ((65J8uNv6D))} | [[Example]]]}} `}`
            - but they can compose
                - so you can have
                    - ```javascript
{{query: {and: [[Questions]] {not: [[important]]}}}}```
                        - gets you Questions that are not important
                    - ```{{query: {or: [[backlinks]] [[Precise Links]]}}}```
                        - gets you blocks that are tagged with backlinks OR precise links

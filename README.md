Amend and Stash


Amend: 
    Scenario: You have just made a commit to your local repository and mention you forgott to add/stage one File or a change on a file. 
    Your commit won’t compile without the change so you have to add it before pushing it.  
    Learn how to amend something to a local commit. 

    - Checkout branch «main» and add some Text to the file «superFile.txt». 
    - Create a new File and add some text as well. 
    - Stage/add changes made on «superFile.txt»
    - Enter a commit message and commit the file.
    - Stage/add changes ond your new File amed it to your previous commit.


Stash: 
    Scenario: Scenario: You have just implemented a new feature and try to figure out why it is not compiling. Your team mate ask you 
    to support him with a bug on a release branch. You should not commit uncompilable code but have to change the branch. 
    Learn how to keep local changes when you get interrupted and have to checkout another branch.

    - Checkout branch «superfeature» and add some Text to the file «superFile.txt». 
    - Change text in File «buggy_feature.txt». 
    - Create a Stash with the message «uncompilable superfeature»
    - Checkout branch «bug_support_branch» create a fix commit and push it
    - Checkout branch «superfeature» and apply your Stash. (If you pop stash it will be deleted)
    - Add some more text to buggy_feature.txt and commit & push your finished work. 

    Hint: Stashes can be applied wherever you want. If git does not know how to apply it will end in a merge conflict you have to solve. 




Note:  There is not solution code for this project because students are expected to produce a small app as described below.  

Do not take aesthetics into account when determining between a 1 and a 2

Pseudocode for the algorithm needed to calculate a balance is as follows:

user = user_id
balance = 0

blockchain = request.get(chain_endpoint)

for block in blockchain
    for transaction in block.transactions
        if transaction.sender = user_id
            balance -= transaction.amount
        if transaction.recipient = user_id
            balance += transaction.amount


Account balances in a blockchain currency are not real values that are stored somewhere.  Instead, wallet programs derive this balance by adding and subtracting all of the transactions for the user that are recorded in the ledger, to calculate the current balance.

Build a simple wallet app using the front-end technology of your choice.  You will not be evaluated on the aesthetics of your app.

This app should:
    * Allow the user to enter, save, or change the `id` used for the program
    * Display the current balance for that user
    * Display a list of all transactions for this user, including sender and recipient

Stretch Goals:
    * Use styling to visually distinguish coins sent and coins received
    * Paginate the list of transactions if there are more than ten
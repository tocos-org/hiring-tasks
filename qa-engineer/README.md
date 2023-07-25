# Take Home Task: Testing an API for Toco Transactions

For this task, imagine we have a RESTful API that allows our users to buy and sell Tocos, our currency backed by carbon mitigation assets, and make transactions with other users. The API has several endpoints including:

- POST /users: Create a new user
- POST /buy: Buy Tocos using fiat currency, and add to a user's account
- POST /sell: Sell Tocos and convert back into fiat currency
- POST /transactions: Make a transaction from one user's account to another
- GET /transactions/{userId}: Get the transaction history for a user

Your task is to write a test plan and automated tests for the /transactions, /buy, and /sell endpoints. Here's what we want you to cover:

1. **Test Plan**: Draft a clear, concise test plan that outlines the testing strategy for the endpoints. The plan should include:

   - Test objectives
   - Test scope
   - Testing approach
   - Resources needed
   - Test cases to be executed

2. **Automated Tests**: Write automated tests that exercise the /transactions, /buy, and /sell endpoints. 

    Some points to consider while writing the tests:

    - Success scenarios where the API should behave as expected
    - Error scenarios where the API should return an error (think about various edge cases like trying to sell more Tocos than a user owns)
    - Testing the transaction limits (eg. what happens if a user tries to buy or sell Tocos beyond their daily limit? What if a user tries to transact more Tocos than a user has?)
    - Security considerations (eg. what if we try to view the transaction history of a user without proper authorization?)
    - Performance considerations (eg. does the API respond quickly enough even under heavy load?)
    - Test the consistency and atomicity of transactions (eg. if a buy operation fails, no Tocos should be added and no fiat money should be deducted, and vice versa for a sell operation)

You are free to choose any language and testing framework for writing the automated tests. For the purpose of this task, you can assume the API exists and behaves as you would expect based on the descriptions above. You do not need to actually run the tests against a live API, but they should be written as if you could.

This task is intended to show us how you approach testing in a real-world situation, particularly in the context of financial transactions where accuracy and reliability are crucial. We're looking for clarity of thought in the test plan, thoroughness in the tests, and clean, readable code. 

This task is designed to be completed in approximately two hours. If you find yourself spending significantly more time, try to simplify your approach and document any assumptions or shortcuts you have taken in the README file.

Please submit your test plan as a PDF and your automated tests as code. Please place these in git repository and share the link or use git bundle to bundle them up, place them on a file sharing service and share the link with us. Good luck!

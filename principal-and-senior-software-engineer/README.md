# Take Home Task: Principal/Senior Software Engineer

Objective: To evaluate the candidate's technical skills, problem-solving abilities, coding practices, and understanding of distributed systems and modern development tools.

Task: Design and implement a small-scale simulation of a Tocos trading system. This micro-version of Toco's digital platform will maintain a list of users and their respective Toco balances (which represent underlying carbon mitigation assets). Users should be able to perform simple transactions such as buying, selling, or transferring Tocos.

## Requirements:

1. Create a simple server application using TypeScript, Rust, or Python (you're welcome to choose any language from these three based on their comfort level). You can use any libraries or frameworks that you deem suitable.
2. The server application should use a simple data store (preferably MongoDB or Postgres) to maintain the list of users and data on their respective Tocos. 

3. Implement the following API endpoints:
   - `POST /users`: Create a new user with an initial balance of Tocos.
   - `GET /users/{id}`: Retrieve details of a user.
   - `POST /transactions`: Perform a transaction between two users. The body of the request should include the ID of the sender, the ID of the receiver, the amount of Tocos to be transferred and any other pertinent details.
4. Each API request should perform necessary validation. For example, a transaction should not be allowed if the sender does not have sufficient Tocos.
5. Write tests to verify the correctness of your server application.
6. Document your design choices, how to run your application, and how to run the tests.
7. Use Docker to containerize your application.
8. Add a simple front-end using React or NextJS to visualize the users and transactions.

## Evaluation Criteria:

1. Code Quality: Proper usage of language constructs, modularization, and organization.
2. Testing: How well the code is covered by tests.
3. Documentation: Clarity of design choices and instructions for running the code and tests.
4. Robustness: Proper handling and validation of inputs, error situations.

## Deliverables:

- The source code of the server application.
- The source code of the tests.
- A README file with documentation.

Please push your solution to a public Git repository and send us the link to the repository or alternatively use git bundle to bundle up your submission, place the resulting file on a file sharing service and share the link to the file.

This task is designed to be completed in approximately two hours. If you find yourself spending significantly more time, try to simplify your approach and document any assumptions or shortcuts you have taken in the README file.
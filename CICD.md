# CI – Continuous Integration

Imagine a group of developers working on the same app. Everyone writes code.

With CI, whenever someone finishes a piece of code, they push it to a shared place (like GitHub).

Then, automatically:

- The code is checked
- It is built (like packaging the app)
- It is tested to see if anything is broken

This happens every time someone updates the code.

CI makes sure all the code works well together and mistakes are caught early.

# CD – Continuous Delivery / Deployment

Now that the code is tested and ready, what’s next?

With CD, that tested code is:

- Automatically sent to a staging or production environment
- No need to do manual steps each time

There are two types:

- **Continuous Delivery** – Code is ready to go live, but someone manually presses the "Go" button.
- **Continuous Deployment** – Code goes live automatically if it passes all the tests.

# Example Flow

1. Developer pushes code to Azure Repos or GitHub
2. Build Pipeline (CI)
    - Pulls the latest code
    - Restores dependencies
    - Builds the app
    - Runs unit tests
    - Publishes build artifacts (output)
3. Release Pipeline (CD)
    - Picks the build artifact
    - Deploys to environments (Dev → QA → Prod)
    - Can include manual approvals
    - Can be automatic (Deployment) or manual (Delivery)
4. Application goes live

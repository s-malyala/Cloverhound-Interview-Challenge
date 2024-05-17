# Age Prediction App

This web application predicts a person's age based on their name using the Agify.io API.

## Components

### NameForm

- Handles user input via a form with a text field and a submit button.
- Calls the parent `App` component function with the entered name upon form submission.

### AgeDisplay

- Receives an `age` as a prop and displays the predicted age or a message if the age cannot be predicted.

## API Interaction

- Uses jQuery’s `$.get()` to fetch ages from Agify.io.
- Responses are managed to display the age or a failure message.
- Successfully retrieved ages are cached to minimize redundant API calls.

## Caching

- Caches ages in the `App` component to avoid repeated API requests for the same names.
- Checks cache before making new requests, using cached data if available.

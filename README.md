# Code-Along 10.1 - Redux

## Requirements

- Node >= 16.x (prefer current LTS version)
- NPM >= 8.x (upgrade executing `npm i -g npm`)
- Chrome >= 103.x

❗ Other browser/Node/NPM configurations might work but haven't been tested.

### Nice to Haves

- Postman HTTP client or similar.
- React Devtools & Redux Devtools Chrome extensions.

## Set Up

1. Clone repo and execute `npm run prep` to install deps and set up your dev database.
2. Launch the project in a dev server executing `npm run dev`.
3. Visit your app by navigating Chrome to `http://localhost:3000`.

You can _optionally_ run frontend and backend separately. __Instead__ of `npm run dev`:

1. `npm run frontend`
2. `npm run backend` (or use the VSCode's integrated Node debugger to launch the backend)

## Accounts

1. __Admin__, username: `admin` password: `admin`
2. __Non-admin__, username: `foo` password: `1234`

### Notes About Accounts

- Anonymous users can answer multiple-choice questions, but stats aren't stored.
- Registered users have access to their stats stored in the backend.
- Admin users can create new and edit existing questions.
- Feel free to register additional accounts (will be non-admin).

## Tests

1. `npm test` runs all tests.

### Note About Running Tests

The `test` script kills the development server because tests need to spin up a testing db
and free port 9000. To restart nodemon just type `rs` in the terminal of the `dev` script,
or restart your debugger.

## Catching Up with Your Instructor

1. `npm run ketchup` resets your local files to the last push by your instructor to `origin/codealong`.
2. `npm run ketchupfull` in addition to the above reinstalls dependencies and resets the database.

Please remember to check the `package.json` file to see all available scripts.

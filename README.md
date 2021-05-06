# Blog App

## Instructions
- Clone the repo
- run `npm i` to install dependencies
- run `npm run ios` for native ios app, if you have Expo
- otherwise, run `npm run web` for web version.

## Notes

- Rebuilding redux from scratch.
- Centralise data in one place in the App and manage state from the Provider.
  - Pass data and callbacks from the Provider.

- Props
  - Sends information from parent directly down to a child
  - Difficult to move info down multiple layers

- Context
  - Fixes this problem ^: moves info from parent to nested child (multiple layers down)
  - Can be complicated to setup - has a bunch of special terms
- Context has a Provider, makes info available to children
- React has useContext
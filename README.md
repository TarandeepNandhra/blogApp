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

- Use Reducer over State to refactor
  - Reducer uses a switch statement for different cases
  - Makes sense for the different CRUD operations
  - type can define each CRUD operation

- To navigate between screens, use the navigation props which is passed via props
  - navigation.navigate("ScreenName"), inside of an onPress.
  - navigation.getParam('id') equivalent to navigation.state.params.id

- Can use .find(() => {}) to get data with particular id

- Screen.navigationOptions function with headerRight to put icon on top of app

- Refactor when screens are similar.

- defaultProps if props is undef.
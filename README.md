# CS571 Workshop 04
Update the source code of Workshop 03 (Github Notes App) as follows:
* The current data flow of the application is structured in a way that all data are passed through the navigation screens as parameters, which causes a lot of unncessary nesting and passing these params between screens. Update the code to use one global state (context) that manages the data through a reducer and provide the necessary helper functions to your application to be used by any screen or component.
* Persist the global state in the AsyncStorage, persist the results of all fetch responses so we don't send future requests if the data is already available. That applies to:
  * The first fetch response (search by Githun username)
  * The second fetch response (look up the user repos)
* The persisted data should be valid for 1 month only.

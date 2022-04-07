Flutter State Management Notes
-Jasdeep Singh, 07/04/2022 5:45pm

Dhan Guru Nanank Dev Sahib ji

State management is how to manage shared state of app
eg. cart in shopping app
https://docs.flutter.dev/development/data-and-backend/state-mgmt/intro


In flutter
Ui = f(state)

UI adapts/reacts to state
not other way around
https://docs.flutter.dev/development/data-and-backend/state-mgmt/declarative


##### Ephermal state 
is local state of a widget that other parts seldom need
https://docs.flutter.dev/development/data-and-backend/state-mgmt/ephemeral-vs-app#ephemeral-state

example 
shows a navbar with state (index), changes on tap, but can reset back when app restarts.

##### App state
[App State vs Ephermal](https://docs.flutter.dev/assets/images/docs/development/data-and-backend/state-mgmt/ephemeral-vs-app-state.png)


When asked about React’s setState versus Redux’s store, the author of Redux, Dan Abramov, replied:

“The rule of thumb is: Do whatever is less awkward.”




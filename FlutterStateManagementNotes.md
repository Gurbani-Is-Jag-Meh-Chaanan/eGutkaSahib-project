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
![App State vs Ephermal](https://docs.flutter.dev/assets/images/docs/development/data-and-backend/state-mgmt/ephemeral-vs-app-state.png)


When asked about React’s setState versus Redux’s store, the author of Redux, Dan Abramov, replied:

“The rule of thumb is: Do whatever is less awkward.”

#### Simple state management
https://docs.flutter.dev/development/data-and-backend/state-mgmt/simple#lifting-state-up
Keep the state above the widgets that use it.

- Where should shared state be kept?
location of shared state should be above the widgets that use it.
idea is to change the data not the ui.
ui always adapts/reacts to any change in data.

as we discussed
Ui = f(state)


- How to access the state?

using provider library
avoid InheritedWidgets

using 3 classes

ChangeNotifier: for model class, storing shared state

ChangeNotifierProvider: for creating and providing shared state to descendends, placed at the parent widgets

Consumer: _pending_






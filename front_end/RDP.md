Require.js Design Patterns
=========================

Package management in JavaScript is only a new development but already there are
some emerging design patterns (and anti-patterns) that are worth discussing that
have cropped up as a direct result of the practise.

Design Patterns
* Refresh/Back on error. Uncaught exceptions will cause the application to stop
 evaluating JavaScript correctly. Have global exception catcher with a stack of
 previous pages. Pop the stack on exception
* Singleton instances for communicating with the user. Replacement of the alert
 / console statements
* Performance / A-B testing built into the application. Respond to user
 interactions in unique ways
* The import singleton shared across all instances.

Anti-Patterns
* Highlander State Machine - Application tracks all state. Does not depend on
routes given. Does not update the routes or does not flush its state on hash
changes and discover bugs and dependencies
* 

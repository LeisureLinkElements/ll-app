# ll-app

Shared application logic to build sub-applications in polymer.  The purpose of this element is to house all the shared logic needed to render a sub-application.


### Features

* User Authentication
	* Validate Session
	* Redirect when invalid
* Application Navigation - Top Navigation
* Notifications
	* System Level - Booking occurred
* Validation - Form is not valid (may be an inline notification)
	* Errors
* Logging
	* Toggle the verbosity of logging
	* Tie into existing logging framework
* Styling isolation
* Throbber is presented when the application is in a "busy" state
* Shared styling
  	* Break dependency of twitter bootstrap
  		* Maybe use skeleton.js or some other raw competing framework.  Skeleton.js is nice because it resets the raw html element

### Nice to Have Features
* Permissions - Renders the user's allowed applications
* Left navigation
	* Sub application specific navigation


*Most of the features should probably be broken into additional web components or included with the ll-app*

### Possible Implementation

The implementation is only for discussion actually implementation is open for discussion

```html
	<ll-app title="Booking">
		<section path="/booking/confirmed">
			<ll-booking-confirmed id="confirmedBookings"></ll-booking-confirmed>
		</section>
	</ll-app>
```

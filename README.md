# REST-API-Implementation-in-Python

Implementing sportsbook product which is responsible for managing sports , events and selections.

A sport contains the following elements:
Name
Slug (url friendly version of name)
Active (either true or false)

An event contains the following elements:
Name
Slug (url friendly version of name)
Active (Either true or false)
Type (Either preplay or inplay)
Sport
Status (Pending, Started, Ended or Cancelled)
Scheduled start (UTC datetime)
Actual start (created at the time the event has the status changed to "Started")

A selection contains the following elements:
Name
Event
Price (Decimal value, to 2 decimal places)
Active (Either true or false)
Outcome (Unsettled, Void, Lose or Win)

A sport may have multiple events
An event may have multiple selections
When all the selections of a particular event are inactive, the event becomes inactive
When all the events of a sport are inactive, the sport becomes inactive

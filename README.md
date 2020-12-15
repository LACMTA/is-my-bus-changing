# is-my-bus-changing

Metro is redesigning its bus service as part of the [NextGen project](https://www.metro.net/projects/nextgen/).  Service updates will be rolled out as part of the regular bi-annual service shakeups that occur every December and June.

The initial set of changes will go into effect on Sunday, December 13, 2020.

This tool will be under continuous development to better communicate service changes to our ridership.  Our goal is to implement features iteratively based on user feedback.

[Try out the tool and give us your thoughts!](https://mybus.metro.net)

Love,
the Metro team


## Change Categories

Make these changes to add a new change category.

In the Google Sheet:

* Add a new column of checkboxes and give it a relevant column header.

In `bus.js`:

* Reference the new column in the `hasChanges` function's conditional statement.
* Add an entry to the `MESSAGES` constant for the message that will show up in the _Key Changes_ box.
* Add a condition to display the new message in the `showChanges` function.

## Lines

Make these changes to modify the lines listed.

In the Google Sheet:

* Add or remove rows using the `Line Number` to match against. Include the `Line Description` column.

In `home.js`:

* Update the `currentLines` array for the `Line Number`.  The Line Number is what will be displayed in the autocomplete list and is what will be used to match against the Google Sheet entries.
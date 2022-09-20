# Android Tests with espresso

Espresso is a testing format used to verify things are working correct in your code.
The core API is small, predictable, and easy to learn and yet remains open for customization.

### On-view

Each time your test invokes onView(), Espresso waits to perform the corresponding UI action or assertion until the following synchronization conditions are met:
- The message queue is empty.
- There are no instances of AsyncTask currently executing a task.
- All developer-defined idling resources are idle.

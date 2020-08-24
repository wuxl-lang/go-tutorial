The `select` statement waits for multiple send or recieve operations simultaneoursly.
* The statement blocks as a whole until one of the operations becomes unblocked.
* If several cases can proceed, a single on of them will be chosen at random.

---

Send and receive operations on a `nil` channel block forever. This can be used to disable a channel in a `select` statement.

---

The `default` case is always able to proceed and runs if all other cases are blocked.

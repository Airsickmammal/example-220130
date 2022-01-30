# example-220130

Example to show how to edit the schedule of a standard dynamic-term-equal-installment loan to be the same as a dynamic-term-balloon one.

See [src/http/api/mambu/examples/edit_schedule.clj](https://github.com/MkershMambu/example-220130/blob/main/src/http/api/mambu/examples/edit_schedule.clj)

Goto Comments section. Execute the following steps from a REPL
* [1] - Creates a New Loan
* [3] - Edits the schedule of loan to be the same as a real-balloon-loan
    * NOTE: We do NOT create a real-balloon-loan account, we are just using the mambu [/loans:previewSchedule](https://api.mambu.com/#loan-accounts-getpreviewloanaccountschedule) endpoint to get the schedule
    * If you want to actually create a real-balloon-loan account as well execute [1b]
        * You may want to do this to check that the simulated-bullet-loan created when executing [3] does have exactly the same schedule as a corresponding real-balloon-loan account
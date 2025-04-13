Run a single table "events" and include upstream dependencies. This will effectively run the scripts which define those tables, which may result in incremental changes to tables.

    dataform run --vars=startDate=2025-03-25,endDate=2025-03-25 --actions=events --include-deps


Run single table "events" with up and downstream dependencies.

    dataform run --vars=startDate=2025-03-20,endDate=2025-03-20 --actions=events --include-deps --include-dependents



# TODO

 - Add pre_operations script to delete rows with that date prior to running.
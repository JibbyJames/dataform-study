Run a single table and include manual assertions (dependencies).

    dataform run --vars=shardSuffix=20250320 --actions=events  --include-deps=true


Run single table without up and downstream dependencies

    dataform run --vars=shardSuffix=20250320 --actions=metrics



Run single table and downstream dependencies

    dataform run --vars=shardSuffix=20250320 --actions=events --include-dependents=true
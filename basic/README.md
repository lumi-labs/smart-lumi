# relayer basic

- a basic relay implementation based on relayer.
- uses postgres, which I think must be over version 12 since it uses generated columns.
- it has some antispam limits, tries to delete old stuff so things don't get out of control, and some other small optimizations.

## running

grab a binary from the releases page and run it with the environment variable POSTGRESQL_DATABASE set to some postgres url:

    POSTGRESQL_DATABASE=postgres://name:pass@localhost:5432/dbname ./relayer-basic

it also accepts a HOST and a PORT environment variables.

## compiling

if you know Go you already know this:

    go install github.com/lumi-labs/smart-lumi/basic

or something like that.

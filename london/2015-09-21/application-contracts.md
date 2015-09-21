# 2: Application Contracts

## Definitions
- Protocol-based
- Contract testing
- Ensure applications behave in consistent and specific ways
- Kill application based on resource utilisation

## Resource utilisation
- AppArmor
- Number of file handlers used
- DPI
- iproute2 (and queue discipline)
-- apps can be prioritised depending on name etc.
-- The Art of Linux Networking book
- cgroups
-- does not work with networking
-- does work with CPU etc.
- JVM
-- has tuneables
- virtualenv
- rbenv
- Docker
- People don't do double-duty on VMs: machines are focused on single task

## Ensure applications behave in consistent and specific ways
- Dev to test checklist required healthcheck endpoint
- Test to QA required monitoring
- QA to Production requires team information, array of contact details for developers
- Service discovery
- Slugrunners: dependencies encompassed in specific way rather than using JVM args etc.
- Slugrunners: allow for quick route to production by simplifying infrastructure
- People rarely come up against issues with limitations set by their service providers
- Standardisation really helps when you want to deploy and upgrade infrastructure

## Documentation
- Difficult to get people to read them
- Difficult to keep them up to date
- Acceptance testing
- Having some automated machine enforcing an application contract
- External third-party checks application for contract violations

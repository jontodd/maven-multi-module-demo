# maven-multi-module-demo
Multi-module maven project to test out build optimization with git change context

## Module Structure
* app - Top level artifact
* client - Standalone module used to talk to the API of the app
* common - Aggregator POM common modules
    * common-crypto
* integration-tests - End to end testing of the app, depends on app

This module structure was selected to cover a number of common scenarios seen in the practice:
* multiple levels of dependencies
* test only modules
* aggregator sub-modules (common)


## Challenge-04

### Scenario
* Lets continue to built on top of ds-challenge-03
* What we have done so far to reduce Developers pain points?
    * Automatic Extensions (Language Support for Java(TM) by Red Hat) inclusion
    * Automatic provisioning of required command line tools
    * Consistent way of building, packaging and running the programs
    * Consistent way of creating standardized end points for current and future testing
* This section will explore on adding more extensions in consistent way and also debugging code

### Set Up + verification
* Reminder : You should have created this workspace from your teams challenges folder in source control
* Open a terminal. Run the command "chmod 755 mvnw" to change the mvnw file to be executable
* Open the "src/main/java/org/acme/ChallengeResource.java" 
* Open the repository in devspaces from your teams
* So, we have our extension "Language Support for Java(TM) by Red Hat" and tools that are required for development are already present : Type "oc --help", "jq --help" etc are already installed
* In devspaces, Open a terminal. Run the command "chmod 755 mvnw" to change the mvnw file to be executable
* Run the quarkus application using commands "2. Start Development mode" you created in devfile. See success criteria on how to run the command
* Select your option "y/n" to the question (if asked) : Do you agree to contribute anonymous build time data to the Quarkus community?
* If things don't look OK, delete the workspace, update the devfile directly in source control and recreate the workspace


### Success Criteria
* Commands are created and can be invoked via the "Hamburger Icon --> Terminal --> Run Task --> Devfile --> Select #Commands"
* Endpoints (shown in the bottom left corner of the IDE) can be invoked
* Invoking localhost:8080 displays an image of the "Developer Flow"
* Invoking localhost:8080/api/hello displays a response "Hello Challenge Attendees"

### Resources
* https://devfile.io/docs/2.2.2/adding-commands
* https://devfile.io/docs/2.2.2/defining-endpoints
* https://devfile.io/docs/2.2.2/devfile-schema

### What did we learn
* In addition to the extensions and tooling, now we have consitent endpoints and commands. This makes iterative development faster (no more typing commands and or finding endpoints via code)
* The next developer will know exactly how things are done making it a much better experience
* One of the core functions of development is to Test & Debug code. In the next challenge, we will explore debugging inside DevSpaces


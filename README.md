## Challenge-04

### Scenario
* Lets continue to built on top of ds-challenge-03
* This section will explore on adding additional resources to the environment. There will be situations where a certain service testing needs more resources. In a traditional laptop, these type of resources may not be available either due to resource constraints or because the workload under test needs specific types of resources (example: GPUs). That forces the developers to either upgrade the machine and or create a whole new setup on another machines.

### Set Up + verification
* Open a terminal. Run the command "chmod 755 mvnw" to change the mvnw file to be executable
* Refer to the Resources section and find out how to add memory and cpu requirements
* Change the Memory : [Reqeust to 512MB and Limit : 2Giga Bytes] and CPU : [Reqeust : 500millicore and Limit : 2000 millicore] to the "tools" container

### Success Criteria
* The devfile is updated with the memory and cpu requests and limits
* Reload the devspaces [Click the Arrows symbol(><) in the Bottom Left corner to open a new menu] with option "Restart with local Dev file"

### Resources 
* https://devfile.io/docs/2.3.0

### What did we learn?
* OpenShift DevSpaces reduces the Developers pain points. As a Developer, your life is getting simpler with the below
    * Automatic Extensions (Language Support for Java(TM) by Red Hat) inclusion
    * Automatic provisioning of required command line tools
    * Consistent way of building, packaging and running the programs
    * Consistent way of creating standardized end points for current and future testing
* Now you can request additional resources easily similar to any workload in the kubernetes

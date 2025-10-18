# Testing with JMeter 

---
### Requirements (Blackboard)
>This is discussed in-class on September 30th. Presentation 10. Slide title, "Apache JMeter Testing… "
>
>This assignment can be run as a continuation of the "Axis 2 in a Tomcat container" assignment.
> 
>In "Axis 2 in a Tomcat container" you configured Axis 2 Web Services Engine in an Apache Tomcat Servlet Engine. Then, you deployed some web services in them (If you have not succeeded in deploying your own web services, you could find existing web services from [Axis 2 source code](https://axis.apache.org/axis2/java/core/docs/userguide-samples.html#services)
>
>Now, we are going to test it with Apache JMeter, rather than using our own Axis 2 client or the browser.
>
>Follow through [JMeter test plan documentation](https://jmeter.apache.org/usermanual/get-started.html), test your web service deployed in Axis 2, and run your JMeter tests.
>
>You will encounter the message "GUI mode should only be used for creating the test script, CLI mode (NON GUI) must be used for load testing." This is a valid point (to conserve processing power, and to ensure smooth testing and to scale the testing with other supportive tools such as Apache Bench). But in this assignment, please use the GUI mode for Apache JMeter and screenshot the JMeter results.
>
>In the submission, upload the below:
>
>1) screenshots that you import from JMeter (or screenshots showing JMeter running)
>
>2) the JMX file of the JMeter test definition.
>
>3) the WSDL file that you used for the service implementation.
>
>Your screenshot should clearly show that you were mimicking several "clients" with your JMeter (i.e., not just one task, definite the test plan accordingly).

---

## **System Configuration**

OS  
: Fedora 42 Workstation  

Java Dev Kit  
: OpenJDK **21.0.8** 2025-07-15  

JMeter Version
: 5.6.3

---

## **Assignment Requirements**

#### JMeter Screenshots
I ran into an issue immediately where the jmeter GUI was far too small to be usable. With some research I found this is a common issue for high density displays and there was a modification I had to make to the `./bin/jmeter` file. This file said to instead make those changes in a modular file at `./bin/setenv.sh` to keep it separate from the base config.

```shell setenv.sh
JVM_ARGS="-Dsun.java2d.uiScale=2.5"
```
![JMeter First Startup](screenshots/2025-10-18_15-33-31.png "JMeter First Startup (With display fix)")

#### JMX File of JMeter Test Definition

```jmx

```

#### WSDL File for Service Implementation

```wsdl

```

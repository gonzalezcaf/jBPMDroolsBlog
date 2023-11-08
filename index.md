sdfasd
# GOAL
* Execute a simple first installation of the jBPM.

# REQUIREMENTS
* Download from the jBPM site the last version 7.74.1.Final.
  At the moment of this article were reported 2 issued registered by the JIRA's:
  1. https://issues.redhat.com/browse/JBPM-10160 (jBPM 7.73 Installation does not work on java 11.0.16 anymore). 
  2. https://issues.redhat.com/browse/WFLY-14625 (WARN message jaegertracing: FlushCommand execution failed!)

  These will be fixed in the next minor or cummulative version. No worries!

* OpenJDK version 8 installed

# STEPS
1. Extract the zip file to a custom folder 
   $ unzip jbpm-server-7.74.1.Final-dist.zip
2. Run the command to start application server (WildFly) and the jBPM components.
   $ bin/standalone.sh
3. Use a web browser and try the url http://localhost:8080/business-central
4. Use the default users set up for the product:
 
wbadmin | admin,analyst,user,process-admin,kie-server
kieserver | rest-all

# OUTCOMES
* You have the jBPM running! However, there are a lot of settings you can use or apply as security, persistence, clustering, cloud-native, tunning and so on and so forth.
The next entries on the blog I will cover those topics.

See you soon!

Home Loan Project on Blueprint (OSGi)
=========================================

We have a system, that takes in XML files from different vendor's home loan application, 
they will place their customer input into 2 different XML files, one with it's customer data, 
the other with their housing details. Both files will be place into same folder either 
by FTP or Batch generated overnight.

Our job is to take in and process the information, first we need to separate the 2 kinds of files, 
because they are handled differently. And appraised the value of the house before sending it to a 
messaging broker for further process.


To build this project use

    mvn install

To run the project you can execute the following Maven goal

    mvn camel:run

To deploy the project in OSGi. For example using Apache ServiceMix
or Apache Karaf. You can run the following command from its shell:

    osgi:install -s mvn:org.blogdemo/homeloan/1.0.0-SNAPSHOT



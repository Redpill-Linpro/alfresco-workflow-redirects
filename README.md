Alfresco Workflow Redirects
=============================================

This module is sponsored by Redpill Linpro AB - http://www.redpill-linpro.com.

Description
-----------

This share module will automatically redirect a user to any following step in a workflow where the user is the assignee as soon as the user completes a workflow task.

Lets say that you have a "Wizard"-like workflow where several user tasks follow each other that the user needs to complete. With this module the user will automatically be redirected to the next assigned step if there is one. Without the module, the user would have been redirected back to the user dashboard and from there would have to click on the task to edit it.

Building & Installation
------------
Clone the repository and build it with "mvn clean package". This will generate a Share amp which can be installed into your Share installation using the Alfresco Module Management Tool (alfresco-mmt):

* Upload the amp file to your amps_share directory in your Alfresco installation.
* Stop Alfresco Share
* Run java -jar bin/alfresco-mmt.jar install amps_share/alfresco-workflow-redirect-share-x.x.x.amp tomcat/webapps/share.war 
* Clean out temporary share files and old unpackaded share war (remove tomcat/webapps/share and tomcat/work/Catalina)
* Start Alfresco Share
* Activate the module from the Share Module Deployment page: http://localhost:8080/share/page/modules/deploy

License
-------

This application is licensed under the LGPLv3 License. See the [LICENSE file](LICENSE) for details.

Authors
-------

Marcus Svensson - Redpill Linpro AB

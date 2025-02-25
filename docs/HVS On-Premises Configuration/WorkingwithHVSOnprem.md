> Install and configure other features of Hitachi Visualization Suite in
> a private virtual or physical environment.

# Update the SSL Certificates

> The HVS system requires valid and up-to-date SSL certificates to work
> properly. You can find the procedure to replace the expired SSL
> certificates for HVS 7.0 and above versions.
>
> This section includes the procedure for an OVF system, which can also
> be followed for an on- premises system.

## Prerequisites

> Complete the following prerequisites before replacing the expired SSL
> certificates:

- Download the latest HVS certificates, hvs_certificates.zip file from
  [<u>TISC</u>](http://tisc.hds.com/techpubs/orderprocess/index.cfm).

- Extract the contents of the hvs_certificates.zip file.

- Make sure you have valid system credentials.

- It is assumed that you have downloaded and configured your on-premises
  HVS or OVF systems in the default location. If you have changed the
  default location, perform the actions described in these sections in
  the modified location.

## HVS OVF1 system SSL certificates

> Update the SSL certificates for the following components on the HVS
> OVF1 system:

- API service. For more information, see [<u>Update the SSL certificate
  for the HVS API
  service</u>](#update-the-ssl-certificate-for-the-hvs-api-service)
  [<u>(on page
  186)</u>](#update-the-ssl-certificate-for-the-hvs-api-service).

- Workflow service. For more information, see [<u>Update the SSL
  certificate for the
  HVS</u>](#update-the-ssl-certificate-for-the-hvs-workflow-service)
  [<u>workflow service (on page
  186)</u>](#update-the-ssl-certificate-for-the-hvs-workflow-service).

- ThingService. For more information, see [<u>Update the SSL certificate
  for the HVS
  Thing</u>](#update-the-ssl-certificate-for-the-hvs-thing-service)
  [<u>service (on page
  186)</u>](#update-the-ssl-certificate-for-the-hvs-thing-service).

- Video connector. For more information, see [<u>Update the SSL
  certificate for the HVS
  video</u>](#update-the-ssl-certificate-for-the-hvs-video-connector)
  [<u>connector (on page
  187)</u>](#update-the-ssl-certificate-for-the-hvs-video-connector).

### Update the SSL certificate for the HVS API service

> Follow the instructions provided in this section to update the SSL
> certificate.
>
> **Procedure**

1.  Log into the OVF1 system using valid credentials.

2.  Open **Internet Information Services (IIS)** from the taskbar and
    stop the HVS API service.

3.  Open **File Explorer** and go to the folder where you extracted the

> hvs_certificates.zip file.

4.  Go to hitachivisualization.com/api and copy the

> hitachivisualization.com.crt file.

5.  Navigate to C:\inetpub\wwwroot\hvs_api.

6.  Paste the copied file and replace the existing certificate file.

7.  Start the HVS API service.

8.  Open the browser and navigate to the HVS API Swagger page to verify
    whether the API is running.

### Update the SSL certificate for the HVS workflow service

> Follow the instructions provided in this section to update the SSL
> certificate.
>
> **Procedure**

1.  Log into the OVF1 system using valid credentials.

2.  Open the Windows Services Manager and stop the HVS workflow service
    manager.

3.  Open **File Explorer** and go to the folder where you extracted the

> hvs_certificates.zip file.

4.  Go to hitachivisualization.com/workflow and copy the

#### hitachivisualization.com.crt file.

5.  Navigate to C:\Program Files(x86)\Hitachi Vantara

> \HVSWorkflowInstanceManager\<version#\>.

6.  Paste the copied file to replace the existing certificate file.

7.  Start the HVS workflow service manager.

8.  Open the Windows Event Viewer and check the HVS Workflow service log
    to validate that the service has started without error.

### Update the SSL certificate for the HVS Thing service

> Follow the instructions provided in this section to update the SSL
> certificate.
>
> **Procedure**

1.  Log into the OVF1 system using valid credentials.

2.  Open the Windows Services Manager and stop the HVS Thing service.

3.  Open **File Explorer** and go to the folder where you extracted the

> hvs_certificates.zip file.

4.  Go to hitachivisualization.com/connectors and copy the

#### hitachivisualization.com.crt file.

5.  Navigate to C:\Program Files\Hitachi Vantara

> \HVSThingService\<version#\>.

6.  Paste the copied file to replace the existing certificate file.

7.  Start the HVS Thing service.

8.  Open the Windows Event Viewer and check the HVS Thing service log to
    validate whether the service has started without error.

### Update the SSL certificate for the HVS video connector

> Follow the instructions provided in this section to update the SSL
> certificate.
>
> **Note:** This information is applicable only if you are using the HVS
> video connector for live streaming.
>
> **Procedure**

1.  Log into the OVF1 system using valid credentials.

2.  Open the Windows Services Manager and stop the HVS video connector
    service.

3.  Open **File Explorer** and go to the folder where you extracted the

> hvs_certificates.zip file.

4.  Go to hitachivisualization.com/connectors and copy the

#### hitachivisualization.com.crt file.

- If you are installing Hitachi Video Management Software, go to
  hitachivisualization.com/hvms and copy the
  hitachivisualization.com.key and hitachivisualization.com.pem files.

- If you are installing Hitachi Video Management Software Base, go to
  hitachivisualization.com/hvms_base and copy the
  hitachivisualization.com.key and hitachivisualization.com.pem files.

5.  Navigate to the location where you have installed the video
    connector.

6.  Paste the copied files to replace the existing certificate files.

7.  Start the HVS video connector service.

8.  Open the Windows Event Viewer and check the HVS video connector
    service log to validate that the service has started without error.

## HVS OVF 2 system SSL certificates

> The HVS OVF2 tasks require basic familiarity with the Linux operating
> system and Docker.
>
> Update the SSL certificates for the following components on the HVS
> OVF2 system:

- HAProxy. For more information, see [<u>Update the SSL certificate for
  HAProxy (on</u>](#update-the-ssl-certificate-for-haproxy) [<u>page
  188)</u>](#update-the-ssl-certificate-for-haproxy).

- Identity management. For more information, see [<u>Update the SSL
  certificate for
  identity</u>](#update-the-ssl-certificate-for-identity-management)
  [<u>management (on page
  188)</u>](#update-the-ssl-certificate-for-identity-management).

- Rule engine service. For more information, see [<u>Update the SSL
  certificate for rule
  engine</u>](#update-the-ssl-certificate-for-rule-engine-service)
  [<u>service (on page
  190)</u>](#update-the-ssl-certificate-for-rule-engine-service).

- Notification service. For more information, see [<u>Update the SSL
  certificate for
  notification</u>](#update-the-ssl-certificate-for-notification-services)
  [<u>services (on page
  191)</u>](#update-the-ssl-certificate-for-notification-services).

### Update the SSL certificate for HAProxy

> **Before you begin**
>
> The HVS OVF2 tasks require basic familiarity with the Linux operating
> system and Docker. Follow the instructions provided in this section to
> update the SSL certificate.
>
> **Procedure**

1.  Go to the directory where you extracted the hvs_certificates.zip
    file.

2.  Copy the haproxy/hitachivisualization.com.full.pem file to the OVF2
    VM using Secure Copy Protocol (SCP).

> scp /path/to/local/cert/file/hitachivisualization.com.full.pem
> hvsuser@\<OVF2_IP_ADDRESS\>:/home/hvsuser

3.  Connect to the OVF2 system using SSH.

4.  Copy the new certificate file to the **SSL** folder and overwrite
    the existing certificate file.

> **Note:** If you receive an access denied error message, log in as a
> root user.
>
> sudo cp ./hitachivisualization.com.full.pem /etc/ssl/private/

5.  Restart HAProxy.

> sudo service haproxy restart

6.  Check the HAProxy status.

> sudo service haproxy status

### Update the SSL certificate for identity management

> **Before you begin**
>
> The HVS OVF2 tasks require basic familiarity with the Linux operating
> system and Docker. Follow the instructions provided in this section to
> update the SSL certificate.
>
> **Procedure**

1.  Go to the directory where you extracted the hvs_certificates.zip
    file.

2.  Copy the idm/hitachivisualization.com.crt file to the OVF2 VM using
    SCP.

> scp /path/to/local/cert/file/hitachivisualization.com.crt
> hvsuser@\<OVF2_IP_ADDRESS\>:/home/hvsuser

3.  Connect to the OVF2 system using SSH.

4.  Stop identity management.

> cd ./hvs-im bash ./stop.sh

5.  Replace the existing certificate file with the new certificate file.

> sudo cp ./hitachivisualization.com.crt ./auth-ctrl/ssl/

6.  List the files from the SSL directory and check if the replaced file
    contains the current date.

> ls -lha ./auth-ctrl/ssl

7.  Start identity management.

> bash ./start.sh master

8.  Confirm that the master instance is running.

    1.  Run the docker command to confirm that the docker containers
        highlighted in the following image are running from more than a
        minute.

> docker ps

9.  <img src="media/image2.jpeg" style="width:6.12008in;height:0.9375in" />Check
    the identity management status from the HAproxy status page and
    verify that the service is running.

### <img src="media/image3.png" style="width:6.43504in;height:3.76631in" />Update the SSL certificate for rule engine service

> **Before you begin**

- The HVS OVF2 tasks require basic familiarity with the Linux operating
  system and Docker.

- The instructions in this section are valid for the HVS 7.1 version.

> Follow the instructions provided in this section to update the SSL
> certificate.
>
> **Procedure**

1.  Go to the directory where you extracted the hvs_certificates.zip
    file.

2.  Copy the rule_engine/hitachivisualization.com.pfx file to the OVF2
    VM using SCP.

> scp /path/to/local/cert/file/hitachivisualization.com.pfx
> hvsuser@\<OVF2_IP_ADDRESS\>:/home/hvsuser

3.  Connect to the OVF2 system using SSH.

4.  Stop the rule engine service.

> cd hvs-ruleengine bash ./stop.sh

5.  Replace the existing certificate file with the new certificate file.

> sudo cp ./hitachivisualization.com.pfx ./hvs-ruleengine/ssl/

6.  List the files from the SSL directory and check if the replaced file
    contains the current date.

> ls -lha ./hvs-ruleengine/ssl

7.  Start the rule engine service.

> bash ./start.sh

8.  Confirm that the rule engine service is running.

    1.  Run the docker command to confirm that the docker containers are
        running for more than a minute.

> docker ps

9.  Check the rule engine status from the HAproxy status page and verify
    that the service is running.

### Update the SSL certificate for notification services

> **Before you begin**

- The HVS OVF2 tasks require basic familiarity with the Linux operating
  system and Docker.

- The instructions in this section are valid for the HVS 7.1 version.

> Follow the instructions provided in this section to update the SSL
> certificate.
>
> **Procedure**

1.  Go to the directory where you extracted the hvs_certificates.zip
    file.

2.  Copy the notification/hitachivisualization.com.crt file to the OVF2
    VM using SCP.

> scp /path/to/local/cert/file/hitachivisualization.com.crt
> hvsuser@\<OVF2_IP_ADDRESS\>:/home/hvsuser

3.  Connect to the OVF2 system using SSH.

4.  Stop the notification service.

> cd hvs-notification bash ./stop.sh

5.  Replace the existing certificate file with the new certificate file.

> sudo cp ./hitachivisualization.com.crt ./hvs-notification/ssl/

6.  List the files from the SSL directory and check if the replaced file
    contains the current date.

> ls -lha ./hvs-notification/ssl

7.  Start the notification service.

> bash ./start.sh

8.  Confirm that the notification service is running.

    1.  Run the docker command to confirm that the docker containers are
        running for more than a minute.

> docker ps

9.  Check the notification status from the HAproxy status page and
    verify that the service is running.

## HVS OVF 3 system SSL certificates

> The HVS OVF3 tasks require basic familiarity with the Linux operating
> system.
>
> Update the SSL certificates for the custom dashboard component on the
> HVS OVF3 system. For more information, see [<u>Update the SSL
> certificate for custom dashboards (on page
> 192)</u>](#update-the-ssl-certificate-for-custom-dashboards).

### Update the SSL certificate for custom dashboards

> **Before you begin**
>
> The HVS OVF3 tasks require basic familiarity with the Linux operating
> system and Docker. Follow the instructions provided in this section to
> update the SSL certificate.
>
> **Procedure**

1.  Go to the directory where you extracted the hvs_certificates.zip
    file.

2.  Copy the custom_dashboard/hitachivisualization.com.full.pem and
    custom_dashboard/hitachivisualization.com.key files to the custom
    dashboard OVF3 VM using SCP.

> scp /path/to/local/cert/file/hitachivisualization.com.full.pem
> hvsuser@\<OVF3_IP_ADDRESS\>:/home/hvsuser
>
> scp /path/to/local/cert/file/hitachivisualization.com.key
> hvsuser@\<OVF3_IP_ADDRESS\>:/home/hvsuser

3.  Connect to the OVF3 system using SSH.

4.  Stop the Pentaho Business Analytics server.

> systemctl stop pentaho-ba

5.  Replace the existing certificate files with the new certificate
    files.

> sudo cp ./hitachivisualization.com.full.pem /home/pentaho/ssl/
> hitachivisualization.com/
>
> sudo cp ./hitachivisualization.com.key /home/pentaho/ssl/
> hitachivisualization.com/

6.  Open the /home/pentaho/pentaho/pentaho-server/tomcat/conf/
    server.xml file file to find the certificate location for
    SSLCertificateFile and SSLCertificateKeyFile.

> nano /home/pentaho/pentaho/pentaho-server/tomcat/conf/server.xml
>
> \<Connector
>
> SSLCertificateFile="/home/pentaho/ssl/\<FOLDER_WITH_CERTIFICATE_DOMAIN_NAME\>/
>
> \<PEM_CERTIFICATE_FILENAME\>"
>
> SSLCertificateKeyFile="/home/pentaho/ssl/
>
> \<FOLDER_WITH_CERTIFICATE_DOMAIN_NAME\>/\<KEY_CERTIFICATE_FILENAME\>"
>
> SSLEnabled="true" SSLProtocol="TLSv1.2" SSLVerifyClient="optional"
> URIEncoding="UTF-8" clientAuth="false" maxThreads="150" port="443"
> protocol="org.apache.coyote.http11.Http11NioProtocol" scheme="https"
>
> secure="true"/\>

7.  List the files and check if the replaced files contain the current
    date.

> ls -lha /home/pentaho/ssl/hitachivisualization.com/

8.  Start the Pentaho Business Analytics server.

> systemctl start pentaho-ba

9.  Log into the Pentaho application from your browser to confirm that
    the Pentaho Business Analytics server is up and running.

## Check the site status

> After updating the SSL certificates for the HVS components in your OVF
> systems (OVF1, OVF2, or OVF3), perform the following actions to check
> that the services and HVS application are running:

- Check the HAproxy status page and verify that all the services are up
  and running.

- Open the HVS URL and perform the following actions to check the
  certificate status:

  - <img src="media/image4.jpeg" style="width:5.57083in;height:2.14958in" />Click
    the Lock icon next to the address bar.

  - Check that the connection is secure and the certificate is valid.

> **Note:** After logging in, if the HVS application does not work as
> expected, check the error on the browser console.

# Set up and configure the custom dashboards

> The document is intended for use by Hitachi employees only.
> Unauthorized duplication or redistribution is prohibited.

## Overview

> If your site is running Visualization Suite locally (within your
> environment), the Custom Dashboards module must be installed and
> configured to send data to the Pentaho Business Analytics server
> through Pentaho Data Integration (PDI).
>
> Otherwise, if the site is using the cloud version of Visualization
> Suite, a system with the Custom Dashboards module enabled is provided
> to you with access to a Pentaho server.
>
> After you review the prerequisites, the setup involves the following
> general process:

1.  Deploy the Custom Reports Open Virtualization Format (OVF).

2.  Add the license to the Pentaho Business Analytics server and Pentaho
    Data Integration (PDI).

3.  Configure Single Sign On (SSO).

4.  Configure database access.

5.  Specify the domain to be used for Custom Dashboards.

6.  Enable scheduled jobs.

7.  Enable Custom Dashboards in Visualization Suite.

## Prerequisites

> Before completing the setup procedures, verify, and apply the
> following requirements:

#### System Requirements

- Visualization Suite version 6.4.0 or later.

- Visualization Suite Dashboard runs on Ubuntu Server 18.04 LTS 64 bit.

- Visualization Suite Dashboard Open Virtualization Format (OVF) file
  and Visualization Suite Database Tool (CLI).

- vSphere Client v6.7.0 (used to qualify the OVF files)

#### License

> Request a trial or production license.

#### Software Download

> Download the Custom Dashboards OVF (available for Hitachi personnel
> only).

#### URLs and access information

- Visualization Suite API URL

- Visualization Suite API Port

- Visualization Suite IP address (URL)

- Visualization Suite MongoDB host name or address

- Visualization Suite domain value for custom dashboard such as "demo"

> **Review credentials**

<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
</colgroup>
<thead>
<tr>
<th><blockquote>
<p><strong>System</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>User name</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Password</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Sudo privileges</strong></p>
</blockquote></th>
<th><strong>Notes</strong></th>
</tr>
</thead>
<tbody>
<tr>
<th>Business Analytics (BA) Server ssh</th>
<td>pentaho</td>
<td>Pto19$$88</td>
<td>enabled</td>
<td></td>
</tr>
<tr>
<th>Business Analytics (BA) Server ssh</th>
<td>pdi</td>
<td>Pto19$$88</td>
<td>enabled</td>
<td></td>
</tr>
<tr>
<th>Pentaho User Console (PUC)</th>
<td>admin</td>
<td>BAca5c267!</td>
<td>N/A</td>
<td style="text-align: right;">Default user</td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
</colgroup>
<thead>
<tr>
<th><strong>System</strong></th>
<th><blockquote>
<p><strong>User name</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Password</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Sudo privileges</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Notes</strong></p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr>
<th>Pentaho User Console (PUC)</th>
<td>pdi</td>
<td>Pto19$$88</td>
<td>N/A</td>
<td>Create a Pentaho Data Integration user after logging in to the
Pentaho User Console and assign an 'administrator' role.</td>
</tr>
<tr>
<th>Pentaho User Console (PUC)</th>
<td>HVS(uppercase required)</td>
<td>Pto19$$88</td>
<td>N/A</td>
<td></td>
</tr>
<tr>
<th style="text-align: right;">PostgreSQL</th>
<td>postgres</td>
<td>dM2J6GbFVytE E8cS</td>
<td>N/A</td>
<td><p>Use the command to access postgres:</p>
<p>psql -U postgres</p></td>
</tr>
</tbody>
</table>

> **Note:** Some tasks require basic familiarity with the Ubuntu
> operating systems and commands; for example, when enabling scheduled
> jobs, Cron syntax will be used.

## Deploy the custom reports OVF

> **Procedure**

1.  Unzip the zip file components while you have all components in the
    same directory. Use the extracted OVF to deploy a new virtual
    machine using a VMware tool.

2.  Log in to the virtual machine using the following credentials:

    - username: Pentaho

    - password: Pto19\$\$88

> <img src="media/image5.png" style="width:3in;height:3.05333in" />

3.  Assign a Static IP address to the server, from the command prompt:

> \# IP_ADDRESS, NETWORK_MASK, GATEWAY_ADDRESS, DNS_SERVER_ADDRESS - use
> values for
>
> your system
>
> \# make sure replace use "static" instead of "DHCP" sudo nano
> /etc/network/interfaces
>
> auto lo ens160
>
> iface lo inet loopback iface ens160 inet static address IP_ADDRESS
>
> netmask NETWORK_MASK
>
> gateway GATEWAY_ADDRESS dns-nameservers DNS_SERVER_ADDRESS

4.  Set the host name (for example, hvs-dashboard):

\# NEW_HOST_NAME - use values for your system sudo hostnamectl
set-hostname NEW_HOST_NAME

sudo nano /etc/hosts

IP_ADDRESS

NEW_HOST_NAME

\# addition to the HOST_NAME, if need to add IP map, add list of URL and
IP

\# IP_ADDRESS SOME_URL

> <img src="media/image6.png" style="width:5.5in;height:2.07333in" />

5.  Add the NTP server to the ntp.conf file (/etc/ntp.conf), then
    restart the NTP service:

> \# YOUR_NTP_SERVER_IP - use value for your system
>
> \# make sure all HVS system uses NTP service to synchronize time
>
> \# Stop service
>
> sudo systemctl stop ntp
>
> \# open the nap.conf file
>
> \# move cursor to locate to the below line sudo nano /etc/ntp.conf
>
> \# Set the server IP
>
> server YOUR_NTP_SERVER_IP
>
> \# start ntp service and validate it is working sudo ntpdate
> YOUR_NTP_SERVER_IP
>
> sudo systemctl start ntp sudo systemctl status ntp
>
> <img src="media/image7.png" style="width:5.5in;height:3.42in" />

<img src="media/image8.png" style="width:5.5in;height:1.66667in" />

6.  Reboot and verify that the system is reachable from your network:

> \# to restart system sudo reboot

## Add licenses to Pentaho

> Licenses are required for the Pentaho User Console (PUC) /Business
> Analytics (BA) server and Pentaho Data Integration (PDI).

#### To Add Licenses to Pentaho User Console and Business Analytics

- See the "Manage License Using PUC" section at [<u>Manage Pentaho
  Licenses</u>](https://docs.hitachivantara.com/search/all?query=pentaho%2Blicense&content-lang=en-US).

- Pentaho User Console URL is
  https://*\<the-custom-dashboards-server-address\>*:8443/ pentaho/Login

- For Pentaho User Console credentials, see the credential section to
  find an admin user for the Pentaho User Console.

- Upload all available licenses to the PUC.

> <img src="media/image9.jpeg" style="width:5.5in;height:2.07333in" />
>
> **Procedure**

1.  Run the following command as a Pentaho Data Integration user:

> \# Copy the license file (zip or tar file) to /home/pdi/ \# See How to
> copy file in reference section
>
> \# Execute this as PDI user su - pdi
>
> \# unzip the licenses.tar.gz file into the licenses folder in the
> pentaho home tar -xf /home/pdi/licenses.tar.gz -C /home/pdi/
>
> \# unzip the licenses.zip file into the licenses folder in the pentaho
> home sudo unzip /home/pdi/licenses.zip -d /home/pdi/
>
> \# Install all of the licenses
>
> /home/pdi/license-installer/install_license.sh install
> /home/pdi/licenses/\* -q

2.  Specify the license path:

> \#login as pdi user su - pdi
>
> \# open the custom job file to edit
>
> sudo nano /home/pdi/scheduled-tasks/scheduled-advanced-job.sh
>
> \# add below line the bottom of the other export line
>
> export
> PENTAHO_INSTALLED_LICENSE_PATH=/home/pdi/.kettle/.installedLicenses.xml
> \# save changes
>
> \# open the basic job file to edit
>
> sudo nano /home/pdi/scheduled-tasks/scheduled-basic-job.sh
>
> \# add below line the bottom of the other export line
>
> export
> PENTAHO_INSTALLED_LICENSE_PATH=/home/pdi/.kettle/.installedLicenses.xml
>
> \# save changes

<img src="media/image10.png" style="width:5.5in;height:1.59333in" />

## Configure single sign on

> Modify the Visualization Suite SSO configuration file to specify the
> Visualization Suite API URL.
>
> \# login as pentaho su - pentaho
>
> \# open SSO file
>
> \# move cursor and locate to the below line
>
> \# update the your_hvs_api_url:port_number value
>
> \# i.e: your_hvs_api_url: api.hitachivisualization.com
>
> \# i.e: port: 9443 (depend on your on-prem configuration port number
> may vary) \# save the changes
>
> sudo nano
> /home/pentaho/pentaho/pentaho-server/pentaho-solutions/system/
> applicationContext-HVS-SSO.xml
>
> \<!-- YOU CAN CHANGE THIS --\>
>
> \<entry key="hvsApiUrl"
> value="https://your_hvs_api_url:port_number/"/\>
>
> \<entry key="hvsPrincipal" value="HVS"/\>
>
> \# comment out the below line
>
> \<!--entry key="allowedDomainId" value="HVS_DOMAIN_ID"/ --\>
>
> \# Restart pentaho-ba services \# to check status
>
> sudo systemctl status pentaho-ba
>
> \# to stop
>
> sudo systemctl stop pentaho-ba
>
> \# to start
>
> sudo systemctl start pentaho-ba
>
> <img src="media/image11.png" style="width:5.07031in;height:1.35823in" />

## Configure database access

> Update the MONGODB_ENTITIES_HOST and MONGODB_AUDIT_HOST values in the
> properties file to set up the database access.
>
> Use DNS or map the MongoDB IP address in the hosts file. For example,
> you can map the MongoDB IP address with
> mongodb.hitachivisualization.com, and then use
> mongodb.hitachivisualization.com as the value for the
> MONGODB_ENTITIES_HOST and MONGODB_AUDIT_HOST.
>
> \# login as pdi su - pdi
>
> \# update the file for below MongoDB section
>
> \# move cursor to find the row, and update the value
>
> \# YOUR_MONGODB_IP_ADDRESS - replace with MongoDB server DNS if you
> have DNS, or use the URL that maps to the MongoDB IP address in the
> hosts file.
>
> sudo nano /home/pdi/repository/load-events-and-crimes/load-events-and-
> crimes.properties
>
> MONGODB_ENTITIES_HOST = YOUR_MONGODB_IP_ADDRESS MONGODB_AUDIT_HOST =
> YOUR_MONGODB_IP_ADDRESS
>
> \# update the file for below MongoDB section
>
> sudo nano /home/pdi/repository/load-advanced-insights/load-advanced-
> insights.properties
>
> MONGODB_ENTITIES_HOST = YOUR_MONGODB_IP_ADDRESS MONGODB_AUDIT_HOST =
> YOUR_MONGODB_IP_ADDRESS
>
> <img src="media/image12.jpeg" style="width:5.5in;height:4.73333in" />

## Specify the domain for the custom dashboards

> \# login as pdi su - pdi
>
> \# update the domain value (default "demo")
>
> sudo nano
> /home/pdi/repository/load-advanced-insights/postgresql-connections.json
>
> "dedicated_to": "Your_domain_name", (default is "demo")
>
> <img src="media/image13.png" style="width:5.5in;height:2.24667in" />
>
> **Enable scheduled jobs**
>
> The following task requires that you understand basic Cron syntax and
> how to edit it. For related information, see [<u>Setting up a basic
> cron job in
> Linux</u>](https://www.taniarascia.com/setting-up-a-basic-cron-job-in-linux/).
>
> \# login as pdi su - pdi
>
> \# The cron command is known as crontab. We'll set our cron job of
> basic dashboard and custom dashboard
>
> \# Once you SSH into the server, you can check if there are any
> current jobs running with the following command to list all crontabs:
>
> crontab -l
>
> \# installing new crontab crontab -e
>
> \# Uncomment out the first two lines, make it like below (take out '#'
> character)

- \* \* \* \* /usr/bin/flock -n /tmp/scheduled-advanced-job.lck
  /home/pdi/scheduled-tasks/ scheduled-advanced-job.sh

- \* \* \* \* /usr/bin/flock -n /tmp/scheduled-basic-job.lck
  /home/pdi/scheduled-tasks/ scheduled-basic-job.sh

> \# to edit
>
> \# press esc.
>
> \# press i (for "insert") to begin editing the file. \# remove the
> first character of the two lines
>
> \# press esc again to exit editing mode.
>
> \# type :wq to save (w - write) and exit (q - quit) the file.
>
> \# to check pdi job, should find 3 jobs ps -ef \| grep java
>
> \# to check date, make sure date is right date

<img src="media/image14.png" style="width:5.5in;height:0.68in" />

## Enable custom dashboards

### Enable basic dashboards in the Visualization Suite client

> Perform the following steps to enable basic dashboards in the
> Visualization Suite client:
>
> **Procedure**

1.  Log in to the Visualization Suite Web UI server, which is the server
    that hosts the HVS Web UI.

2.  Locate the Visualization Suite web UI config file.

> For example. C:\inetpub\wwwroot\hvs_ui\config.json

3.  Open the config.json file with a text editor.

4.  Set the "DASHBOARD_TYPE" value to "BASIC_DASHBOARD", as shown in the
    following example:

<img src="media/image15.jpeg" style="width:5.5in;height:1.80667in" />

5.  Save the changes.

6.  Restart the Visualization Suite HVS Web UI service.

7.  Log in to Visualization Suite, then click **Dashboards** to view the
    Basic Dashboards with the Pentaho-powered business intelligence and
    enable the custom dashboard.

### Enable basic dashboards using custom dashboard server

> The customer dashboard includes the basic dashboard reports, but they
> are disabled by default. You can perform the following steps to enable
> basic dashboards using the custom dashboard server.
>
> You need to use the HVS CLI tool to update the HVS database entry, as
> the Admin portal site does not have the option to enable the basic
> dashboard.
>
> **Procedure**

1.  Log into Visualization Suite server where the database is installed.

    - If you are using the Visualization Suite system with the OVF
      templates, the CLI tool is located in C:\hvs_cli_HVS_VERSION\cli.

    - If you do not find the file, download the Visualization Suite
      Suite CLI tool from [<u>TISC</u>](http://tisc.hds.com/), then
      extract the ZIP file.

2.  For Windows, open the **Command Prompt** window as administrator.

3.  Navigate to the extracted location.

> For example, C:\hvs_cli_HVS_VERSION\cli.

4.  Run the following command, replacing the HVS_DASHBOARD_SERVER_URL,
    DB_USERNAME, DB_PASSWORD, and HVS_MONGODB_IP_OR_URL variables with
    actual values:

> \# linux
>
> ./hvs db update-readonly-doc -pu
> https://HVS_DASHBOARD_SERVER_URL:8443/pentaho - pp
> /home/HVS/basic_dashboards/hvs_basic_dashboard.xdash hvs -a mongodb://
> DB_USERNAME@DB_PASSWORD:HVS_MONGODB_IP_OR_URL:27017/hvs
>
> \# Windows
>
> hvs db update-readonly-doc -pu
> https://HVS_DASHBOARD_SERVER_URL:8443/pentaho - pp
> /home/HVS/basic_dashboards/hvs_basic_dashboard.xdash hvs -a mongodb://
> DB_USERNAME@DB\_\$PASSWORD:HVS_MONGODB_IP_OR_URL:27017/hvs
>
> In this code:

- HVS_DASHBOARD_SERVER_URL is the HVS custom dashboard URL. For example:
  [<u>https://dashboard.hitachivisualization.com</u>](https://dashboard.hitachivisualization.com/)

- HVS_MONGODB_IP_OR_URL is the IP address or URL of the server where HVS
  MongoDB is installed.

  - If you are using the Visualization Suite system with the HVS OVF
    templates, HVS OVF 1 is the HVS MongoDB. If you are running this
    command on the server where MongoDB is installed, you can use the
    localhost instead of the IP address or URL.

- DB_USERNAME and DB_PASSWORD are the HVS database credentials provided
  in the OVF installation guide. Use hvs as the username and use the
  password that is listed in the OVF installation guide.

> **Result**
>
> The basic dashboard is enabled and you get a document update message.
>
> **Next steps**
>
> If you receive an error with this command, do the following:

- Check the MongoDB service is up and running.

- Log into MongoDB using any database tool to validate the username and
  password.

- Check the command for any typo errors.

### Enable custom dashboards in the admin portal

> Perform the following steps to enable custom dashboards in the admin
> portal:
>
> **Procedure**

1.  Open a browser.

2.  Log in to the Visualization Suite Admin Portal.

> For example,
> [<u>https://portal.hitachivisualization.com/.</u>](http://portal.hitachivisualization.com/)

3.  Select the domain from the left navigation menu.

4.  Navigate to the **License** section.

5.  Click the **license** row for the domain.

6.  Select the **Custom Dashboards** check box, as shown in the
    following example:

<img src="media/image16.jpeg" style="width:5.5in;height:2.18667in" />

7.  Click **Save** or **Update**.

8.  At the bottom of the **Domain** section or just the previous
    **Licese** section, you can see **Custom Dashboard Server Address**
    and **Custom Dashboard Report Path**, enter the value according to
    your dashboard system setting.

> Default value is shown in the following example:

<img src="media/image17.jpeg" style="width:5.25in;height:1.45833in" />

9.  Save the changes.

10. Log out of the Visualization Suite Admin Portal.

11. Log in to the Visualization Suite UI.

12. Go to **Dashboards**.

13. Verify that Basic Dashboards are generated by Pentaho.

14. Verify that the **Custom dashboard** menu is shown after the **Basic
    Dashboards** menu.

### Specify entity data for custom dashboards

> **Procedure**

1.  Open a browser.

2.  Log in to Visualization Suite.

3.  Go to **Map** \> **SETTINGS** \> **ENTITY TYPES**.

4.  From the navigation pane, select **Event Entity Type**.

5.  Click the gear icon to go to **Entity Type Management**.

6.  On the **Detail** tab, verfiy the **Enable Custom Dashboards** check
    box to make the entity data available for the Dashboard.

> The **Enable Custom Dashboards** option is available only for **Event
> Type** and when the custom dashboard license is enabled.

### Disable Apache JServ Protocol

> By default, the Apache Jserv Protocol (AJP) connector is enabled in
> the Apache Tomcat server, which can create security vulnerability
> issues. To avoid such issues, make sure that you disable the AJP
> configuration in the Apache Tomcat server configuration file so that
> unused custom dashboard servers are switched off.
>
> Disable the Apache Jserv Protocol connector as follows:
>
> **Procedure**

1.  SSH to the dashboard server as Pentaho user.

> su - pentaho

2.  Navigate to /home/pentaho/pentaho/pentaho-server/tomcat/conf.

3.  Open the server.xml file.

4.  Find the connector node that contains the **AJP/1.3** protocol
    attributes.

> \<!-- Define an AJP 1.3 Connector on port 8009 --\>
>
> \<Connector port="8009" protocol="AJP/1.3" redirectPort="8443" …/\>

5.  Comment the AJP configuration as shown in the following example:

> \<!--
>
> \<Connector port="8009" protocol="AJP/1.3" redirectPort="8443" …/\>
>
> --\>
>
> If the configuration is already commented, then do not perform any
> action.

6.  Save the file.

7.  Restart the Apache Tomcat server.

### Disable unauthenticated user access

> The instructions to disable unauthenticated users from accessing
> custom dashboards are as follows:
>
> **Procedure**

1.  SSH to the dashboard server as Pentaho user.

> su - pentaho

2.  Navigate to /home/pentaho/pentaho/pentaho-server/pentaho-solutions/
    system/.

3.  Take a backup of the applicationContext-spring-security.xml file.

> cp applicationContext-spring-security.xml applicationContext-spring-
> security.xml.org

4.  Open the applicationContext-spring-security.xml file using a text
    editor.

> vi applicationContext-spring-security.xml

5.  Find and remove the Anonymous string occurrence from the following
    lines:

> The line numbers can vary depending on the system being used.

- 242 - 243

> \<sec:intercept-url pattern="\A/.\*require-cfg.js.\*\Z"
> access="Anonymous, Authenticated" /\>
>
> \<sec:intercept-url pattern="\A/.\*require-js-cfg.js.\*\Z"
> access="Anonymous,Authenticated" /\>

- 301 - 304

> \<sec:intercept-url pattern="\A/plugin/reporting/api/jobs/.\*\Z"
> access="Anonymous,Authenticated" method="OPTIONS" /\>
>
> \<sec:intercept-url pattern="\A/plugin/reporting/api/jobs/.\*\Z"
> access="Anonymous,Authenticated" method="HEAD" /\>
>
> \<sec:intercept-url pattern="\A/api/repos/.\*\Z" access="Anonymous,
> Authenticated" method="OPTIONS" /\>
>
> \<sec:intercept-url pattern="\A/api/repos/.\*\Z" access="Anonymous,
> Authenticated" method="HEAD" /\>

- 326 - 331

> \<sec:intercept-url pattern="\A/plugin/reporting/api/jobs/.\*\Z"
> access="Anonymous,Authenticated" method="OPTIONS" /\>
>
> \<sec:intercept-url pattern="\A/plugin/reporting/api/jobs/.\*\Z"
> access="Anonymous,Authenticated" method="HEAD" /\>
>
> \<sec:intercept-url pattern="\A/api/repos/.\*\Z" access="Anonymous,
> Authenticated" method="OPTIONS" /\>
>
> \<sec:intercept-url pattern="\A/api/repos/.\*\Z" access="Anonymous,
> Authenticated" method="HEAD" /\>
>
> \<sec:intercept-url pattern="\A/api/.\*require-cfg.js.\*\Z"
> access="Anonymous,Authenticated" /\>
>
> \<sec:intercept-url pattern="\A/api/.\*require-js-cfg.js.\*\Z"
> access="Anonymous,Authenticated" /\>

6.  Save the file.

7.  Restart the pentaho-ba service.

> sudo service pentaho-ba restart

8.  Verify that pentaho-ba service status is active.

> sudo service pentaho-ba status

## System references

### Pre-installed software

#### Pentaho Business Analytics Enterprise Edition

> v9.0.0.0.2.544
>
> Version9.0 with 9.0.0.2-544 patch

#### Pentaho Data Integration

> v9.0.0.0.2.544
>
> Version9.0 with 9.0.0.2-544 patch

#### Pentaho CTools Dashboards

> Enabled

#### OpenJDK

> Java is required for Pentaho Data Integration and Business Analytics
> to be able to run.
>
> Environment Variables: JAVA_HOME and PENTAHO_JAVA_HOME set to
> /usr/lib/jvm/java-8-openjdk-amd64
>
> In the log file, you should see Pentaho Data Integration and Business
> Analytics print out the PENTAHO_JAVA_HOME variable when it starts.

#### PostgreSQL

> v9.6
>
> [<u>https://www.postgresql.org/docs/9.6/install-requirements.html</u>](https://www.postgresql.org/docs/9.6/install-requirements.html)

### PostgreSQL database schemas

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr>
<th style="text-align: center;"><strong>Schema</strong></th>
<th style="text-align: center;"><strong>Table</strong></th>
<th style="text-align: left;"><blockquote>
<p><strong>Description</strong></p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr>
<th>Advanced</th>
<td>DOMAINNAME_ENTITYTY PENAME_ENTITYTYPEID</td>
<td style="text-align: left;">The table containing entity data of the
selected entity type.</td>
</tr>
</tbody>
</table>

> **Pentaho Data Integration server folder structure**

#### data-integration

> Folder containing Pentaho Data Integration components

#### license-installer

> Folder containing the license installer tool

#### pentaho_eula.txt

> EULA file

#### repository

> Folder containing the Pentaho Data Integration repository called
> LocalRepository

#### scheduled-tasks

> Folder containing the scheduled scripts

### Log files

> Log Location: /home/pentaho/pentaho/pentaho-server/tomcat/logs

#### Tomcat files catalina.out

> The file containing every Tomcat System.out line. The right place to
> start investigation.

#### catalina.2019-04-16.log

> Catalina historic file

#### host-manager.2019-04-15.log

Tomcat specific log files

#### localhost.2019-04-15.log

> Tomcat specific log files containing list of HTTP requests

#### localhost_access.2019-04-16.log

> Tomcat specific log files containing list of HTTP requests

#### manager.2019-04-15.log

> Tomcat specific log files

#### Pentaho files pdi.log

> The file containing logs from the built in Pentaho Data Integration
> instance which we do not use.

#### pentaho.log

> The file containing logs related to Pentaho Business Analytics server

## Troubleshoot

> Before implementing any troubleshooting measures, complete the
> following:

- Verify the configuration steps and confirm that the specified values
  are correct.

- Make sure that Visualization Suite and the Visualization Suite
  dashboard are communicating.

### Basic dashboards

> The basic dashboards are not available and the Visualization Suite
> Basic Dashboards message shows: The Dashboards is not available,
> please contact your administrator.
>
> <img src="media/image18.png" style="width:5.50083in;height:1.61in" />
>
> Verify the following to fix the issue:

- Make sure that the Time Server is configured correctly and that all
  Visualization Suite related systems share the same date and time.

- Review the configuration steps. When the Dashboard does not open, it
  might be related to the configuration errors.

- SSH to the Dashboard Server:

  - Check the scheduled log files.

  - Make sure license is installed correctly.

  - Check if services are running.

### Custom dashboards

> Use the following instructions to troubleshoot issues related to the
> custom dashboards:

#### Custom dashboard error

> The custom dashboards might not load in Visualization Suite because of
> the following error in the pentaho-server/tomcat/logs/catalina.out
> file: javax.net.ssl.SSLProtocolException: The certificate chain length
>
> \(11\) exceeds the maximum allowed length (10)
>
> Follow these instructions to fix the issue:

1.  Open the start-pentaho.sh file:

> su -pentaho
>
> sudo vi /pentaho/pentaho/pentaho-server/start-pentaho.sh

2.  Find the following parameter:

> -Djdk.tls.maxCertificateChainLength=15
>
> If you do not find the parameter, add the -
> Djdk.tls.maxCertificateChainLength=15 parameter to the
> **CATALINA_OPTS** attribute:
>
> After addition, CATALINA_OPTS="-Djdk.tls.maxCertificateChainLength=15
>
> -Djava.awt.headless=true - Dpentaho.karaf.instance.start.port=11004 -
> Djava.net.preferIPv4Stack=true -Xms4096m -Xmx6144m -
> XX:MaxPermSize=256m -Dsun.rmi.dgc.client.gcInterval=3600000 -
> Dsun.rmi.dgc.server.gcInterval=3600000 -Dfile.encoding=utf8 -
> DDI_HOME=\\\$DI_HOME\\"

3.  Save the changes.

4.  Stop the Pentaho Business Analytics server:

> sudo systemctl stop pentaho-ba

5.  Start the Pentaho Business Analytics server:

> sudo systemctl start pentaho-ba

#### PDI job error

> The following error appears when running the PDI job:
>
> WARNING: javax.net.ssl.SSLProtocolException: The certificate chain
> length (11) exceeds the maximum allowed length (10)
>
> Follow these instructions to fix the issue:

1.  Open the spoon.sh file:

> sudo vi /home/pdi/data-integration/spoon.sh

2.  Find the following parameter:

> -Djdk.tls.maxCertificateChainLength=15
>
> If you do not find the parameter, add the -
> Djdk.tls.maxCertificateChainLength=15 parameter to the **OPT**
> attribute:
>
> After addition, OPT="\$OPT \$PENTAHO_DI_JAVA_OPTIONS -
> Dhttps.protocols=TLSv1,TLSv1.1,TLSv1.2 -Djava.library.path=
>
> \$LIBPATH -Djava.endorsed.dirs=\$JAVA_ENDORSED_DIRS -DKETTLE_HOME=
>
> \$KETTLE_HOME -DKETTLE_REPOSITORY=\$KETTLE_REPOSITORY -
> DKETTLE_USER=\$KETTLE_USER -DKETTLE_PASSWORD=\$KETTLE_PASSWORD -
> DKETTLE_PLUGIN_PACKAGES=\$KETTLE_PLUGIN_PACKAGES -
> DKETTLE_LOG_SIZE_LIMIT=\$KETTLE_LOG_SIZE_LIMIT -DKETTLE_JNDI_ROOT=
>
> \$KETTLE_JNDI_ROOT -Duser.timezone=UTC -
> Djdk.tls.maxCertificateChainLength=15"

3.  Save the changes.

#### Pentaho user console error

> Custom dashboard shows the following error when trying to access the
> <u>Pentaho user</u> <u>console</u>: HTTP Status 404 - Not found
>
> Follow these instructions to fix the issue:

1.  Connect to a custom dashboard server using SSH.

> su - pentaho

2.  Check that the pentaho-ba service is running.

> sudo systemctl status pentaho-ba

1.  If it is not running, start the service.

> sudo systemctl start pentaho-ba

2.  If it is running, stop and restart the service.

> sudo systemctl stop pentaho-ba sudo systemctl start pentaho-ba

3.  Check the status to ensure it is up and running.

4.  Check all the available log files to find any errors. The log file
    location is: /home/ pentaho/pentaho/pentaho-server/tomcat/logs

> If the issue still persists, contact [<u>Hitachi
> Support</u>](https://support.hitachivantara.com/en_us/contact-us.html).

### Time server

> For issues related to the Time Server, review the following:

- Make sure that server time is synchronized with the NTP server.

- Use ntpdate ntp_server_ip_address to synchronize the Visualization
  Suite Dashboard Server with the NTP server.

- Add the NTP server IP address to /etc/ntp.conf then restart the NTP
  server.

### PostgreSQL

> **How to view PostgreSQL Server Access**
>
> nano /etc/postgresql/9.6/main/pg_hba.conf

<table>
<colgroup>
<col style="width: 11%" />
<col style="width: 18%" />
<col style="width: 44%" />
<col style="width: 25%" />
</colgroup>
<thead>
<tr>
<th><p>local</p>
<p>local</p></th>
<th><blockquote>
<p>all</p>
<p>all</p>
</blockquote></th>
<th><blockquote>
<p>postgres</p>
<p>all</p>
</blockquote></th>
<th style="text-align: right;"><p>md5</p>
<p>md5</p></th>
</tr>
</thead>
<tbody>
<tr>
<th>all</th>
<td><blockquote>
<p>all</p>
</blockquote></td>
<td><blockquote>
<p>0.0.0.0/0</p>
</blockquote></td>
<td style="text-align: right;">md5</td>
</tr>
<tr>
<th>all</th>
<td><blockquote>
<p>all</p>
</blockquote></td>
<td><blockquote>
<p>::1/128</p>
</blockquote></td>
<td style="text-align: right;">md5</td>
</tr>
</tbody>
</table>

> **How to verify all tables**
>
> SELECT \* FROM information_schema.tables.

### Business Analytics server

> **How to connect ssh?**
>
> ssh user_name@IP_ADDRESS
>
> **How to verify the Pentaho service status?**
>
> \# login as pentaho user su - pentaho
>
> sudo systemctl status pentaho-ba
>
> **How to start the Pentaho service?**
>
> \# login as pentaho user su - pentaho
>
> sudo systemctl start pentaho-ba
>
> **How to stop the Pentaho service?**
>
> \# login as pentaho user su - pentaho
>
> sudo systemctl stop pentaho-ba
>
> **Cannot connect to the Pentaho User Console (PUC)**
>
> Verify the service status.
>
> \# login as pentaho user su - pentaho
>
> \# check status
>
> sudo systemctl status pentaho-ba

#### Cannot connect to the Pentaho User Console from outside the system

> Try to ping or curl to see if it works.
>
> \# using Chrome window
>
> \# Open chrome browser on HVS system, navigate to the PUC URL
>
> \# Open browser on different client system, navigate to the PUC URL
> Https://DASHBOARD_SERVER_IP_ADDRESS:8443/pentaho
>
> \# Ping test
>
> Open cmd and test the ping works (reachable or not)
>
> \# using curl
>
> curl https://localhost:8443/pentaho/Login

#### Cannot start the Business Analytics server

> Examine the log files:

- Stop the server

- Clean the logs folder in
  /home/pentaho/pentaho/pentaho-server/tomcat/logs

- Start the server

- Test the specific part

- Take a look at clean logs

#### How to retain Pentaho installed licenses after a restart?

> At the beginning of the logs, verify that the
> *PENTAHO_INSTALLED_LICENSE_PATH* variable is pointing to a valid path.
>
> Verify the licenses applied using the following script:
>
> \# login as pentaho user su - pentaho
>
> \# List All Environment Variables, verify the
> PENTAHO_INSTALLED_LICENSE_PATH=/home/
> pentaho/pentaho/.pentaho/.installedLicenses.xml
>
> printenv
>
> \# Set the licenses path in this shell
> PENTAHO_INSTALLED_LICENSE_PATH=/home/pentaho/pentaho/.pentaho/.installedLicenses.xml
>
> \# Install all of the licenses
>
> /home/pentaho/pentaho/license-installer/install_license.sh display

#### Visualization Suite custom dashboard single sign-on does not work

> Try to curl the Visualization Suite API from the custom dashboard BA
> server, as you should be able to reach the Visualization Suite API
> from the machine.
>
> curl https://api.hitachismartcam.com/
>
> ping api.hitachismartcam.com from dashboard server

#### How to check that Pentaho receives an error from the Visualization Suite API?

> Try enabling component logs and verify if HTTP requests to the
> Visualization Suite API are successful or if they fail for some
> reason.
>
> \# open the logging config file.
>
> su - pentaho
>
> sudo nano
> /home/pentaho/pentaho/pentaho-server/tomcat/webapps/pentaho/WEB-INF/classes/
> log4j.xml
>
> \# Add or modify the content so that a new appender is declared and it
> is sending com.hitachivantara.hvs log entries to the hvs.log file
>
> \<!-- ============================== --\>
>
> \<!-- COM HITACHI VANTARA HVS Logger --\>
>
> \<!-- ============================== --\>
>
> \<!-- A time/date based rolling appender --\>
>
> \<appender class="org.apache.log4j.DailyRollingFileAppender"
> name="HVSFILE"\>
>
> \<param name="File"
> value="/home/pentaho/pentaho-server/tomcat/logs/hvs.log"/\>
>
> \<param name="Append" value="false"/\>
>
> \<!-- Rollover at midnight each day --\>
>
> \<param name="DatePattern" value="'.'yyyy-MM-dd"/\>
>
> \<!-- Rollover at the top of each hour
>
> \<param name="DatePattern" value="'.'yyyy-MM-dd-HH"/\>--\>
>
> \<layout class="org.apache.log4j.PatternLayout"\>
>
> \<!-- The default pattern: Date Priority \[Category\] Message\n --\>
>
> \<param name="ConversionPattern" value="%d %-5p \[%c\] %m%n"/\>
>
> \<!-- The full pattern: Date MS Priority \[Category\] (Thread:NDC)
> Message\n
>
> \<param name="ConversionPattern" value="%d %-5r %-5p \[%c\] (%t:%x)
> %m%n"/\>--\>
>
> \</layout\>
>
> \</appender\>
>
> \<category name="com.hitachivantara.hvs"\>
>
> \<priority value="TRACE"/\>
>
> \<appender-ref ref="HVSFILE"/\>
>
> \</category\>

### Pentaho Data Integration

#### How to make sure Pentaho retains installed licenses after a restart?

> At the beginning of the logs, verify that the
> *PENTAHO_INSTALLED_LICENSE_PATH* variable is pointing to a valid path.
> Run the following commands to verify the variables:
>
> \# Execute this as PDI user su - pdi
>
> \# Set the licenses path in this shell
> PENTAHO_INSTALLED_LICENSE_PATH=/home/pdi/.kettle/.installedLicenses.xml
>
> \# Install all of the licenses
>
> /home/pdi/license-installer/install_license.sh display

#### How to change the frequency of the Pentaho Data Integration job execution scheduled tasks?

> \# Execute this as PDI user su - pdi
>
> \# Invoke crontab edit crontab -e
>
> **How to check the Pentaho Data Integration job process status?**
>
> su - pdi
>
> ps -ef \| grep java
>
> The following processes must be running:

- Pentaho Server process

- Custom Dashboard process

- Basic Dashboard process

<img src="media/image19.png" style="width:5.5in;height:1.34in" />

> As a job starts and completes, you might not find that all three
> processes are running, but you should see jobs running, which you can
> stop and restart by running ps -ef \| grep java.
>
> Verify the time server and confirm whether it is not stopping or
> hanging as the time should be synchronized with the current time.
>
> The process status (PS) command is used to provide information about
> the currently running processes, including their process
> identification numbers (PIDs). A process, also referred to as a task,
> is an executing (running) instance of a program.

#### How to issue a kill command for a process id (PID)?

> If a Pentaho Data Integration dashboard job becomes unresponsive,
> identify the process you want to kill using ps. With ps, you are given
> a process id (PID).
>
> \#login as pdi user su - pdi
>
> \# to find PDI (process ID) ps -ef \| grep java
>
> \# Issue a kill command
>
> kill -9 PDI_JOB_ID
>
> \# Check process, after kill command, dashboard jobs will
> automatically start, no need to start job manually
>
> ps -ef \| grep java
>
> **How to verify the log file sizes?**
>
> \# login as pdi user su - pdi
>
> \# to print sizes in a human-readable format. ls -Slhr
>
> OR
>
> ls - lh
>
> **How to verify the scheduled jobs log files?**
>
> \# login as pdi user su - pdi
>
> \# navigate to scheduled-tasks log location cd scheduled-tasks/logs
>
> \# To list information about files and directories within the file
> system \# check file date to validate that job is running and updating
> file
>
> \# if file date is old, consider that job is unresponsive ls - l
>
> \# To open the log file to view vi EXISTING_FILE_NAME
>
> \# check to see whether any error
>
> **How to verify the errors in a log (VI search command)?**
>
> \# login as pdi user su - pdi
>
> \# Open existing file with VI editor vi EXISTING_FILE_NAME
>
> \# Finding a Character String
>
> \# To find a character string, type / followed by the string you want
> to search for, and then press Return. vi positions the cursor at the
> next occurrence of the string. For example, to find the string “meta,”
> type /meta followed by Return.
>
> \# Type n to go to the next occurrence of the string. Type N to go to
> the previous occurrence.
>
> /error (preset Return)
>
> n (to go to the next occurrence)
>
> **How to quit the VI editor without saving any changes?**

1.  If you are currently in insert or append mode, press **Esc**.

2.  Click **:** (colon). The cursor reappears at the lower left corner
    of the window beside the colon prompt.

3.  Enter the following: q!

> **How to disable an advanced job?**
>
> \#login as pdi su - pdi
>
> crontab -e
>
> \# Add "#" like below
>
> \#\* \* \* \* \* /usr/bin/flock -n /tmp/scheduled-advanced-job.lck
> /home/pdi/scheduled- tasks/scheduled-advanced-job.sh
>
> Save changes
>
> **How to apply a license from the Pentaho User Console?**
>
> ManageBusiness Analytics (BA) License using the Pentaho User Console
> (PUC)
>
> You can do this directly in the PUC which can be found when browsing
> http://{OVF IP}:8080/pentaho/Login.
>
> See Credential section for details.
>
> After the login you will be asked to upload the licenses.
>
> Once you are in you can add further licenses by clicking Home \>
> Administration \> Licenses \> Plus sign.
>
> **How to rename a directory?**
>
> mv /home/pdi/oldfolder /home/pdi/newfolder
>
> **How to copy local files to the server?**
>
> Open terminal
>
> Locate to the directory where file located Type sftp USER@IP_ADDRESS
>
> Provide password
>
> Put FILE_NAME

# Set up Single Sign On (SSO) with the Pentaho Business Analytics Server

## Overview of Pentaho SSO

> On-premises Visualization Suite sites can access their Pentaho
> dashboards and reports within the Visualization Suite Dashboards menu
> using their Visualization Suite login. This is done through the
> installation and configuration of the Pentaho SSO plug-in.

#### About the Pentaho SSO plug-in architecure

> The plug-in is an implementation of a custom Spring Security Filter
> that adds middleware to the Pentaho requests and responses pipeline.
>
> If there are any pending authentication requests, this middleware
> validates the provided Visualization Suite token. The validation is
> done by requesting the introspection endpoint of the Visualization
> Suite API. If the request is successful, then a user identity is
> returned; otherwise, the request is marked as unauthorized.
>
> The following diagram shows the validation process.

<img src="media/image20.jpeg" style="width:2.6975in;height:3.51in" />

#### Installation overview

> The general procedure for installing and configuring the Pentaho SSO
> plug-in involves the following tasks:

1.  Reviewing the Pentaho SSO prerequisites.

2.  Copying the SSO package on the remote server.

3.  Extracting the content.

4.  Stopping the server.

5.  Adding the plugin.

6.  Creating a Read only Access User.

7.  Configuring the plugin.

8.  Restarting the server.

## Prerequisites for Pentaho SSO

> Before completing the setup procedures, verfiy and apply the following
> requirements:

#### System Requirements

- Pentaho Business Analytics Server

- License for Pentaho Business Analytics

- Download the SSO package from Technical Information Service Center
  ([<u>TISC</u>](http://tisc.corp.hds.com/)).

#### Environment

> If you are a cloud customer, the Pentaho SSO setup is possible
> provided that all of the following apply:

- Pentaho Business Analytics server is publicly available

- Pentaho Business Analytics server can reach the Visualization Suite
  API

- Pentaho Business Analytics server is accessible from the Visualization
  Suite cloud

#### Qualified System for an on-premises environment

- Pentaho Business Analytics server 9.0.0 with the following patches
  installed:

  - 9.0.0.0.2.544

- Pentaho Business Analytics server which runs on a Ubuntu Server, 18.04
  LTS 64 bit.

- Pentaho Business Analytics server with the following components
  installed:

  - Jackrabbit (authentication system)

  - PostgreSQL

## Installation of Pentaho SSO

> Some tasks require basic familiarity with the Ubuntu operating systems
> and commands. Before you start the installation procedure, ensure that
> you have reviewed and completed the prerequisite tasks.
>
> **Procedure**

1.  Backup your system.

> As a best practice measure, make a backup of your system before
> proceeding with the installation. If your site uses a virtual machine,
> then create a snapshot image.

2.  Set the \$PENTAHO_HOME environment variable.

> The installation requires the \$PENTAHO_HOME variable. To output the
> value of the environment variable from the shell, use the echo command
> and prepend the variable’s name with a dollar (\$) sign.
>
> echo \$PENTAHO_HOME
>
> If the variable is not already set for your system, then set it for
> the installation session using the export command. Give the variable a
> name, which will be used to access it in shell scripts and
> configurations, and then a value to hold whatever data is needed in
> the variable.
>
> export PENTAHO_HOME=VALUE
>
> For example:
>
> export PENTAHO_HOME=/home/pentaho/pentaho

3.  Create a read-only access user.

> Create a user that is associated with a group which has a minimum of
> ‘Read Content’ permissions in the Pentaho User Console (PUC). Ensure
> that you grant access to the report folder that can be viewed from
> Visualization Suite.

4.  Copy the SSO package on the remote server.

> Once the SSO package exists on your machine, you can copy it to the
> remote server. The following example uses scp, although you can use
> another tool:
>
> scp hvs-pentaho-simple-sso-6.4.\*.zip your-pentaho-
> user@yourcustomerdashboards.hitachismartcam.com:/home/your-pentaho-user
>
> To copy local files to the server:
>
> Open terminal
>
> Locate the directory where the file is located Type sftp
> USER@IP_ADDRESS
>
> Provide password Put FILE_NAME

5.  Extract the content.

> Install unzip:
>
> sudo apt-get install unzip
>
> Extract the content from the archive in your user home directory:
>
> unzip hvs-pentaho-simple-sso-6.4.\*.zip
>
> You should now see two new files in your user home directory:

- applicationContext-HVS-SSO.xml

- hvs-pentaho-simple-sso.jar

6.  Stop the server.

> Depending on the Pentaho Business Analytics installation procedure
> that was applied, there are two options to stop the server.

- If daemon was created, use the run command:

> systemctl stop pentaho-ba

- If daemon doesn't exist, use the stop-pentaho.sh script in the
  pentaho-server directory:

> \$PENTAHO_HOME/pentaho-server/stop-pentaho.sh

7.  Add the plug-in.

> Move the plugin JAR file in the Pentaho server libraries directory:
>
> mv hvs-pentaho-simple-sso\*.jar
> \$PENTAHO_HOME/pentaho-server/tomcat/webapps/ pentaho/WEB-INF/lib
>
> Move the plugin config file in the Pentaho installation folder:
>
> mv applicationContext-HVS-SSO.xml
> \$PENTAHO_HOME/pentaho-server/pentaho-solutions/ system/

8.  Configure the plug-in.

> Edit the configuration file using a text editor:
>
> nano
> \$PENTAHO_HOME/pentaho-server/pentaho-solutions/system/applicationContext-
> HVS-SSO.xml
>
> Provide the **hvsApiUrl**, **hvsPrincipal**, and
> **allowedDomainIdvalues** in the section containing
> **id=ssoCustomerSpecificValueMap**, which will look like this:
>
> \<entry key="hvsApiUrl" value="https://HVS_API_URL"/\>
>
> \<entry key="hvsPrincipal" value="hvsuser"/\>
>
> \<entry key="allowedDomainId" value="5e2f08818b426f1754e50499"/\>

#### Table 1 Description of the fields in applicationContext-HVS-SSO.xml

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr>
<th style="text-align: center;"><strong>Field</strong></th>
<th style="text-align: center;"><strong>Description</strong></th>
</tr>
</thead>
<tbody>
<tr>
<th>hvsApiUrl</th>
<td><p>The Visualization Suite API URL.</p>
<p>Change this to address the correct Visualization Suite API which
issued the JWT token that you plan to use.</p></td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr>
<th style="text-align: center;"><strong>Field</strong></th>
<th style="text-align: center;"><strong>Description</strong></th>
</tr>
</thead>
<tbody>
<tr>
<th></th>
<td><p>Note that the token that you will issue to Pentaho needs to be
generated from the same URL that you specify here.</p>
<p>Cloud Staging URL: api.hitachismartcam.com Cloud Production URL:
api.hitachismartcamera.com</p></td>
</tr>
<tr>
<th>hvsPrincipal</th>
<td><p>This represents the name of the Pentahouser that was created at
Step 1. This user will be used to authenticate all of the Visualization
Suite requests.</p>
<p>The value is case-sensitive.</p>
<p>Note that every Visualization Suite user will use the same Pentaho
user so there is a N:1 relation which is a limit of the current
implementation.</p></td>
</tr>
<tr>
<th>allowedDomainId</th>
<td><p>This represents the ID of the domain which is allowed to access
to Pentaho.</p>
<p>Set this if you want to have this instance accepting requests only
from the specified domain.</p>
<p>To find the domain:</p>
<ol type="a">
<li><p>Login to Hitachi Visualization Suite.</p></li>
<li><p>On the left menu, go to <strong>SETTINGS &gt; DOMAIN
DETAILS</strong>. You will find the ID on the Details tab, it is the
unique identifier of the domain.</p></li>
</ol></td>
</tr>
</tbody>
</table>

9.  Configure pentaho-spring-beans.xml file.

> After the file is closed, you can add the newly added configuration
> files inside the pentaho-spring-beans.xml file.
>
> Open the file with a text editor:
>
> nano
> \$PENTAHO_HOME/pentaho-server/pentaho-solutions/system/pentaho-spring-
> beans.xml
>
> Add this line before the closing XML tag:
>
> \<import resource="applicationContext-HVS-SSO.xml" /\>

10. Restart the server.

> Depending on the Pentaho Business Analytics installation procedure
> that was applied, there are two options to restart the server.

- If daemon was created, use the run command:

> systemctl start pentaho-ba

- If daemon doesn't exist, use the start-pentaho.sh script in the
  pentaho-server directory:

> \$PENTAHO_HOME/pentaho-server/start-pentaho.sh

11. Check the Pentaho server.

> Log in to the Pentaho User Console (PUC) with the Visualization Suite
> user that was previously created, and verify that the user can view
> the reports that you specified. If you see any issue, troubleshoot it
> by checking the log files. Previous functionality that Pentaho had
> should remain unchanged.

## Troubleshoot Pentaho SSO

#### Is it possible to refresh the Pentaho Business Analytics token?

> Pentaho Business Analytics does not use the refresh token.
>
> The Hitachi Visualization Suite access token expires after 15 minutes
> and Pentaho Business Analytics validates this token once through a
> Visualization Suite API call. After Pentaho Business Analytics uses
> the token to retrieve a successful response from the Visualization
> Suite API, a new Pentaho session is started and its identifier is set
> in the browser cookies.
>
> Pentaho's session duration is configured in the server’s config files
> where the expiration is set to 15 minutes.

#### What occurs when the access token expires?

> The Pentaho session expiration and the Visualization Suite access
> token expiration are not related--they are independent.
>
> To end a Pentaho session from Visualization Suite, we call the logout
> endpoint of the Pentaho Business Analytics server.

#### Where do I locate the problem source when the Pentaho User Console returns a tomcat error after the changes?

> See the log files:
>
> \# login as pdi user su - pdi
>
> \# Open existing file with VI editor vi EXISTING_FILE_NAME
>
> \# Finding a Character String
>
> \# To find a character string, type / followed by the string you want
> to search for, and then press Return. vi positions the cursor at the
> next occurrence of the string.
>
> For example, to find the string “meta,” type /meta followed by Return.
>
> \# Type n to go to the next occurrence of the string. Type N to go to
> the previous occurrence.
>
> /error (preset Return)
>
> n (to go to the next occurrence)

#### Which log files I should verify to troubleshoot Pentaho Server issues?

> See the "Log files" section in [<u>Set up and configure the custom
> dashboards (on page
> 194)</u>](#set-up-and-configure-the-custom-dashboards).

# Configure storage for your domain

> After installing an HCP-VM system, you must configure the domain to
> use the HCP as storage.

## Visualization Suite storage options

> Visualization Suite offers various options for storing customer files,
> such as blueprints, alert images, map markers, and other digital
> assets related to entities that are uploaded to the system. Storage
> needs vary depending on customer environment in terms of size, costs,
> and infrastructure. With the Visualization Suite's flexible storage
> options, you can choose one that is right for your customer. The
> following table lists the supported storage types:

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
</colgroup>
<thead>
<tr>
<th><blockquote>
<p><strong>Storage</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Visualization Suite cloud</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Visualization Suite on-premises</strong></p>
</blockquote></th>
<th style="text-align: center;"><strong>Supported in Visualization Suite
release</strong></th>
</tr>
</thead>
<tbody>
<tr>
<th>Azure Storage</th>
<td>Supported</td>
<td>Not Supported</td>
<td>5.4.0 or later</td>
</tr>
<tr>
<th>Hitachi Content Platform (HCP)</th>
<td>Not Supported</td>
<td>Supported</td>
<td>5.4.0 or later</td>
</tr>
<tr>
<th>File system</th>
<td>Not Supported</td>
<td>Supported</td>
<td>6.1.0 or later</td>
</tr>
</tbody>
</table>

## Data migration

> Data migration from one storage type to another is not supported.
> Configuring a new back end storage while the files are stored in the
> existing, different storage prevents the existing files from showing.

## Azure storage

> Azure storage is managed by Hitachi. No configuration is required by
> customers.

## Configure Hitachi Content Platform as storage

> For on-premises configurations, you can configure a domain to use an
> HCP-VM system as storage.
>
> You will create a domain and configure storage for the domain using
> Visualization Suite API. You can use Postman or the integrated Swagger
> interface to use the API.
>
> **Before you begin**

- Administrative privileges are required to configure storage for your
  domain.

- An HCP-VM system has been installed and set up. The following figures
  show the HCP namespace settings.

<img src="media/image21.png" style="width:5.5in;height:3.03333in" /><img src="media/image22.png" style="width:5.41406in;height:3.44531in" />

> **Procedure**

1.  Create a domain.

2.  Configure the domain storage using the domainId. The HTTP request
    syntax (URI) is as follows:

> PUT
> https://*\<hvs-api-server-address\>*/admin/domains/*{domainId}*/storageConfig
>
> The following table describes the parameters:

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
</colgroup>
<thead>
<tr>
<th><blockquote>
<p><strong>Parameter</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Required</strong></p>
</blockquote></th>
<th style="text-align: center;"><strong>Type</strong></th>
<th><blockquote>
<p><strong>Description</strong></p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr>
<th>password</th>
<td>No</td>
<td>-</td>
<td>Leave blank (not supported)</td>
</tr>
<tr>
<th>third_party_name</th>
<td>Yes</td>
<td>String</td>
<td>Enter upload_service as the name of the third party for HCP</td>
</tr>
<tr>
<th>third_party_provide r</th>
<td>Yes</td>
<td>String</td>
<td>Enter hs3 as the name of the provider for HCP</td>
</tr>
<tr>
<th>username</th>
<td>No</td>
<td>-</td>
<td>Leave blank (not supported)</td>
</tr>
<tr>
<th>connection</th>
<td>Yes</td>
<td>String</td>
<td><p>Enter the following attributes:</p>
<ul>
<li><p>clusterurl=&lt;hcp_ domain_name&gt;</p></li>
<li><p>tenant=&lt;hcp_te nant_name&gt;</p></li>
<li><p>username=&lt;hcp</p></li>
</ul>
<blockquote>
<p>_user_name&gt;</p>
</blockquote>
<ul>
<li><p>password=&lt;hcp</p></li>
</ul>
<blockquote>
<p>_password&gt;</p>
</blockquote></td>
</tr>
</tbody>
</table>

> The following is an example response structure:
>
> {
>
> "password" : null,
>
> "third_party_name" : "upload_service", "third_party_provider" : "hs3",
> "username" : null,
>
> "connection" : "clusterurl=hvs-ap.hvs.com;tenant=hvshcp;
> username=\<hcp_user_name\>;password=\<hcp_password\>"
>
> }
>
> The following shows an example response:
>
> {
>
> "data": "5ad7b06ecb53c30a14ff2ef8", "totalCount": 1,
>
> "ok": true
>
> }

3.  Add the HCP namespace entry into both the API server host file and
    the client machine host file as follows:

> HCP_IP_ADDRESS \<hvs_domain_id.hcp_tenant_url\>
>
> The following shows an example namespace:
>
> 123.11.12.123 59dc03c73c64e4335c5c9b81.hvshcp.hvs-ap.hvs.com
>
> where:

- 123.11.12.123 is the HCP server IP address

- 59dc03c73c64e4335c5c9b81 is the namespace, which is the Visualization
  Suite domainId

- hvs-ap.hvs.com is the hcp_domain_name

- hvshcp is the hcp_tenant_name

4.  Restart the API service (Windows service or IIS per your system).

## Configure a new domain with a file system

> For on-premises configurations, Visualization Suite can be configured
> to store files on the Visualization Suite Web API servers. Note that
> the recommended storage described in the Installation Guide does not
> take into consideration system scaling for file storage. When
> configuring a domain with a local file system, you must carefully
> plan, monitor, and manage the storage as storage requirements vary
> depending on the application environment. If the domain is integrated
> with event alert-generating applications, such as Live Face Matching
> and Video Analytics, it can accelerate the data growth.
>
> Use the following instruction to configure a new domain with a file
> system.
>
> **Note:** File system storage is not supported for the cloud instances
> of Visualization Suite.
>
> **Procedure**

1.  Open the API configuration file appsettings.json with a text editor.
    For example: C:\inetpub\wwwroot\api\appsettings.json.

2.  Update the storage section with the required file system
    information. The following shows an example storage configuration
    for a file system:

"Storage": {

"UseSsl": false,

"Provider": "filesystem", "Username": "",

"Password": "", "TokenExpirationInMinutes": 120,

"Connection": "Path=C:\\hvs-fsstorage",

},

#### UseSsl

> Set to "true" if using SSL. Set to "false" if not using SSL.

#### Provider

> Enter files ystem for configuring a file system.

#### Username

> Leave blank (not supported)

#### Password

> Leave blank (not supported)

#### TokenExpirationInMinutes

> Access token authentication expiration time in minutes (default is
> 120)

#### Connection

> File system path (example: Path=C:\\hvs-fsstorage)

3.  Restart the API service.

> Windows service or IIS per the system.

4.  Create a new domain.

> **Result**
>
> <img src="media/image23.png" style="width:5.41406in;height:2.33625in" />A
> folder is created with the name of domainId in the specified
> directory. The following figure shows an example file system
> configured for a new domain.

## Configure a shared network drive for file storage

> When needed, you can configure a shared drive as storage when the
> Visualization Suite API is hosted by Internet Information Services
> (IIS). The procedure involves the following key steps:

- Creating users to run IIS and to access the password-secured drive.

- Granting access to the network share.

- Configuring IIS to run as a custom user.

- Changing the Visualization Suite API storage connection.

### Create duplicate users

> To ensure that the network share is accessible from the machine where
> the API is installed and where IIS is located, users must be created
> to run IIS and to access the password- secured drive.
>
> In the following procedure, you will create a user to exist on the
> machine where the API is installed. Then, you will repeat the
> procedure to create another user with the same name and the same
> password to exist on the machine where IIS is installed.
>
> **Procedure**

1.  From the Windows Control Panel, locate **Edit locale users and
    groups**.

2.  Right-click on the **Users** folder and select **New User**.

3.  Specify a **Username** and **Password**.

4.  Clear the setting, **Ask to change password at the next login**.

5.  Select **Password never expires**.

### Grant access to the network share

> After the users have been created, you can grant access to the network
> share.
>
> **Note:** As recommended by Microsoft, only use Universal Naming
> Convention (UNC) names to access resources, as shown in the following
> example format:
>
> \\MyServer\filesharename\directoryname\filename
>
> **Procedure**

1.  From the Windows IIS machine, map the drive in Windows with a letter
    of your choice.

2.  When prompted for credentials, specify administrative level
    credentials so that rights to change the drive permissions exist.

3.  To check which users and groups are allowed to perform operations on
    the network share, run the **icacls** command by passing the path as
    the argument.

> This will list the users, and the groups that have rights to them:
>
> icacls \\IP_ADDRESS\sample\share\\

4.  To add the newly created user (in this example, USER_NAME), run the
    following command, ensuring that the example user name is replaced
    with the actual name that you previously specified:

> icacls \\IP_ADDRESS\sample\share\\ /grant "USER_NAME":(OI)(CI)F /T

### Configure IIS to run as a custom user

> In order for IIS to run the Visualization Suite API as the newly
> created user, the Identity field for the APIs advanced settings needs
> to change to the Custom Account of that user.
>
> **Procedure**

1.  Open Internet Information Services Manager and locate **Application
    Pools**.

2.  Locate the application which is used by the Visualization Suite API
    web site, then right- click on it and select **Advanced Settings**.

3.  From **Advanced Settings**, go to the **Process Model** section and
    locate the **Identity**

> field.
>
> By default, this field is set to **ApplicationPoolIdentity**.

4.  Click **Set** to enter information about the newly created user and
    password, then click

> **OK**.

5.  Click **Recycle** on the application pool to verify that the new
    identity is in use.

6.  Restart the Visualization Suite API web site.

### Change the Visualization Suite API storage connection

> Once the network share can be reached, you must configure the storage
> section of the appsettings.json file of the API with correct values,
> as shown below.
>
> Afterward, save the file, then restart the web site in IIS.
>
> "Storage": {
>
> "UseSsl": false, "Provider": "filesystem",
>
> "\_comment": "Available Providers : filesystem, azure, hcp",
> "Username": "",
>
> "Password": "", "TokenExpirationInMinutes": 120,
>
> "Connection": "Path=\\\\IP_ADDRESS\\sample\\share", "\_comments":
> "this connection is for local server machine"
>
> },

> This article provides information about the Hitachi Visualization
> Suite mobile app for the iOS and Android<sup>™</sup> devices.

# Overview

> Hitachi Visualization Suite includes a mobile app, which is available
> for iPhone<sup>®</sup> and Android<sup>™</sup> devices.
>
> Using the Visualization Suite mobile app, you can do the following:

- View real-time (or live) events and incidents on Map

- View incident list and incident detail

- View media such as video clips or photos

- Work on incidents through standard operation procedure (SOP)

- Upload photos and video clips to an incident

- View nearest cameras and correlated events

> You can download the Visualization Suite mobile app based on your
> device:

- <img src="media/image1.png" style="width:1.5676in;height:0.52604in" />App
  Store<sup>®</sup>:
  [<u>https://apps.apple.com/us/app/hitachi-visualization-suite/id1598341524</u>](https://apps.apple.com/us/app/hitachi-visualization-suite/id1598341524)

> The Visualization Suite app requires iOS 11 or later.

- <img src="media/image2.jpeg" style="width:1.5625in;height:0.5in" />Play
  Store:
  [<u>https://play.google.com/store/apps/details?id=com.hitachivantara.hvs.mobile</u>](https://play.google.com/store/apps/details?id=com.hitachivantara.hvs.mobile)

# Onboarding

> You can log into the Visualization Suite mobile app using the login
> credentials used for the Visualization Suite web application.
>
> When you log into the mobile app for the first time, your mobile
> device is registered in the Visualization Suite web application. You
> can find the device ID information in the Visualization Suite web
> application at **Settings \> Memberships \> Users \> Details \> Users
> management** page.
>
> **Procedure**

1.  Open the **Visualization Suite** app on your mobile device.

> <img src="media/image3.png" style="width:2.8125in;height:5.92708in" />The
> **Welcome to Hitachi Visualization Suite** screen appears.

2.  Tap **Let's get started!**.

3.  Complete the following fields:

#### Domain Name

> Type your Visualization Suite domain name. The domain name is the
> first word in the Visualization Suite instance URL after the HTTPS://
> protocol. For example, if the URL is
> [<u>https://demo.hitachismartcamera.com</u>](https://demo.hitachismartcamera.com/),
> the domain name is *demo*.

#### Identity Management URL

> Type the Visualization Suite Identity Management URL.
>
> For example, following are the Identity Management URLs:

- Cloud Production:
  [<u>https://identity.hitachismartcamera.com</u>](https://identity.hitachismartcamera.com/)

- Cloud Staging:
  [<u>https://identity.hitachismartcam.com</u>](https://identity.hitachismartcam.com/)

#### API URL

> Type the API end point of your Visualization Suite application.
>
> For example, following are the API end points:

- Cloud Production:
  [<u>https://api.hitachismartcamera.com</u>](https://api.hitachismartcamera.com/)

- Cloud
  Staging:[<u>https://api.hitachismartcam.com</u>](https://api.hitachismartcam.com/)

<img src="media/image4.png" style="width:2.8125in;height:5.875in" />

4.  Tap **Next**.

5.  Type the email address associated with your account username and
    password.

> <img src="media/image5.png" style="width:2.8125in;height:5.84375in" />

6.  Tap **Login**.

7.  Tap **Next** to enable notifications so that Visualization Suite can
    access real time data.

> <img src="media/image6.png" style="width:2.8125in;height:5.84375in" />

8.  Tap **Next** to enable location services.

> <img src="media/image7.png" style="width:2.8125in;height:5.82292in" />

9.  Allow Visualization Suite to access the mobile location. The
    following options are available:

    - **While using the app**

    - **Only this time**

    - **Don't allow**

> <img src="media/image8.png" style="width:2.8125in;height:5.84375in" />
>
> **Note:**

- Visualization Suite does not track your mobile location but only uses
  it when using the **Locate me** feature to display where you are
  located.

- If you choose **Don't allow**, the location services are not enabled.
  To use the **Locate me** feature, make sure to enable the location
  services from your mobile's **Settings** screen.

10. Tap **Get started!**.

> <img src="media/image10.png" style="width:2.8125in;height:5.90625in" />
>
> The map view is displayed.
>
> If you are unable to log in or get an error upon logging in, see
> [<u>Troubleshoot (on</u>](#troubleshoot) [<u>page
> 336)</u>](#troubleshoot) to resolve the issue.

# Map view

> You can visualize integrated event and incident data from multiple
> sources using the map view. The **Map** menu enables you to view every
> entity related to a crime, event, incident, or object in real-time.
>
> You can see a map marker for every entity selected under the
> **Filter**
> <img src="media/image11.png" style="width:0.18333in;height:0.20833in" />
> option in the map view. For example, **Incidents** list the incidents
> related to fire, burglary, vehicles, and so on.
>
> When you tap fire incidents, Visualization Suite displays the fire
> incident map markers on the map. To remove the fire incident map
> markers from the map view, tap fire incidents again.
>
> <img src="media/image12.png" style="width:2.8125in;height:5.77083in" />
>
> By default, Visualization Suite is configured to use Google Maps.
> Using **Map**, you can gain quick insights into the following
> entities:

- **Crimes**: View historical crimes.

- **Events**: View events from multiple sources, including analytics
  applications and sensors.

- **Incidents**: View incidents that impact normalcy of the business
  operations.

- **Objects**: View the stationary items, such as buildings and cameras.

## Search

> You can use the **Search** location function to quickly find locations
> on the map view.
>
> In the map view, type the desired location in the **Search** field and
> tap the **Search** icon
> <img src="media/image13.png" style="width:0.1875in;height:0.1875in" />.
> The map view refreshes to display the specified location.

## Filters

> You can use the **Filter** function to clear the map view of all map
> markers and display only those that are required.
>
> In the map view, tap the **Filter** icon
> <img src="media/image11.png" style="width:0.18333in;height:0.20833in" />
> and select the items under different entities, such as **Events**,
> **Incidents**, and **Objects**. The map view displays the map markers
> for the selected items.
>
> For example, select **Fire Incident** under **Incidents** to display
> the fire incident map markers on the map. To remove the fire incident
> map markers from the map view, tap **Fire Incident** again.

<img src="media/image14.png" style="width:2.8125in;height:5.79167in" />

## Map markers

> The map marker is used to mark the location of the crime, event,
> incident, or object on the map view. The incident map marker's shape
> is rectangle, while the other map markers are in a circle shape.
>
> <img src="media/image15.jpeg"
> style="width:2.22917in;height:1.67708in" />
>
> Tap the map marker to get an information summary of the entity on the
> map view.

## Summary view

> You can get information about any entity displayed on the map. To see
> the **Summary View** of an entity, tap the map marker of that entity.
>
> For example, the **Summary View** of an incident map marker provides
> information on the priority, severity, and date timestamp of the
> incident. You can further swipe up the **Summary View** pane to see
> more details of the entity, such as address, description, assignee,
> status, and so on.
>
> <img src="media/image16.png" style="width:2.8125in;height:5.80208in" />

### Camera status

> When you tap the **Camera** icon on the map view, the **Summary View,
> Camera List and Detail** screens provides quick information about the
> camera name, address, and camera status.
>
> The camera status is visually identifiable, which helps to determine
> which cameras are active. The following table provides information on
> the status and its description:

<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 22%" />
<col style="width: 57%" />
</colgroup>
<thead>
<tr>
<th><blockquote>
<p><strong>Status</strong></p>
</blockquote></th>
<th style="text-align: center;"><strong>Icon</strong></th>
<th style="text-align: center;"><strong>Description</strong></th>
</tr>
</thead>
<tbody>
<tr>
<th>Green</th>
<td><img src="media/image17.jpeg"
style="width:0.16646in;height:0.16646in" /></td>
<td>camera is online</td>
</tr>
<tr>
<th>Red</th>
<td><img src="media/image18.jpeg"
style="width:0.16646in;height:0.16646in" /></td>
<td>camera is offline</td>
</tr>
<tr>
<th>Yellow</th>
<td><blockquote>
<p><img src="media/image19.jpeg"
style="width:0.15583in;height:0.16646in" /></p>
</blockquote></td>
<td>camera does not exist</td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 22%" />
<col style="width: 57%" />
</colgroup>
<thead>
<tr>
<th><blockquote>
<p><strong>Status</strong></p>
</blockquote></th>
<th style="text-align: center;"><strong>Icon</strong></th>
<th style="text-align: center;"><strong>Description</strong></th>
</tr>
</thead>
<tbody>
<tr>
<th>Grey</th>
<td><img src="media/image20.jpeg"
style="width:0.16646in;height:0.16646in" /></td>
<td>camera status is not available</td>
</tr>
<tr>
<th>Purple</th>
<td><blockquote>
<p><img src="media/image21.jpeg"
style="width:0.14521in;height:0.14875in" /></p>
</blockquote></td>
<td>video gateway is offline</td>
</tr>
</tbody>
</table>

## Locate me

> After enabling the location services on your device, you can tap the
> **Locate Me** icon
> <img src="media/image22.png" style="width:0.19792in;height:0.1875in" />
> to show your current location on the map.
>
> **Note:** Visualization Suite does not track the mobile location but
> only displays where you are located when the location service is
> enabled.
>
> If **Summary View** is open, the **Locate Me** icon is not available
> on the map view.

# List view

> The list view displays all the available incidents in Visualization
> Suite. Each incident record provides a quick summary of the incident,
> such as priority, severity, status, standard operating procedure
> progress, and date timestamp of the incident.
>
> <img src="media/image23.png" style="width:2.8125in;height:5.84375in" />
>
> To open the list view, tap **List** from the bottom navigation bar. If
> you want to get more details of the incident, tap the incident record.
> For more information, see [<u>View incident details
> (on</u>](#view-incident-details) [<u>page
> 324)</u>](#view-incident-details).

## Search

> You can use the **Search** option in the list view to find and display
> only specific incident records.
>
> Enter the keyword from the incident name or description in the
> **Search** field to view the relevant results. For example, enter fire
> as shown in the image to view fire-related incidents:
>
> <img src="media/image24.jpeg"
> style="width:2.23427in;height:4.42219in" />

## Filters

> You can use the **Filter** option in the list view to refine the
> displayed incident records.
>
> <img src="media/image25.png" style="width:2.8125in;height:5.80208in" />
>
> Tap the **Filter** icon
> <img src="media/image11.png" style="width:0.18333in;height:0.20833in" />
> and select the date range, incident type, priority, severity, status,
> or assignee to display incident records as per your filter criteria.

## Sort

> You can use the **Sort** icon
> <img src="media/image26.png" style="width:0.11384in;height:0.16071in" />
> in the list view to sort the incident records according to the
> incident's created date, updated date, name, type, assignee, priority,
> severity, or status.
>
> You can further sort the listed records in ascending or descending
> order.
>
> <img src="media/image27.png" style="width:2.8125in;height:5.85417in" />

# Incidents

> An incident is an event that affects the confidentiality, integrity,
> and availability (CIA) of an organization, and impacts the business
> and its operations. For example, an attacker leaves an unknown object
> in a city, and the city needs to evacuate residents, reroute traffic,
> and so on.
>
> Incident management in Hitachi Visualization Suite enables you to
> restore normal service operations and minimize the impact on business
> operations. Normal service operations are those within the
> Service-Level Agreement (SLA).

## View incident details

> You can tap the incident record in the list view to see the incident
> details.
>
> The **Details** screen provides information on the incident name,
> address and location, description, assignee, members responsible for
> managing the incident, priority, severity, status, incident type, and
> other useful information related to the incident.

<img src="media/image28.png" style="width:2.8125in;height:5.80208in" />

> From the **Details** screen, you can use the **Camera** icon to
> capture and upload new photos or videos of the incident, or browse and
> upload existing photos or videos. The captured photos or videos are
> displayed in the **Media** section of the incident detail record. For
> more information, see [<u>Upload Media (on page
> 325)</u>](#upload-media).

## Upload Media

> You can upload media content such as photos or videos to an incident.
> The uploaded media will be available for Visualization Suite users who
> monitor organization via Visualization Suite mobile app or web
> application to evaluate the incident.
>
> The **Details** screen displays the captured photos or videos in the
> **Media** section of the incident detail record.
>
> <img src="media/image29.jpeg"
> style="width:2.23427in;height:4.37583in" />
>
> **Note:** The Visualization Suite app supports up to 1GB of media
> content for upload.
>
> The **Camera** icon is displayed in the **Details**, **SOPs**,
> **Events**, and **Cameras** screens of the incident record.
>
> <img src="media/image30.jpeg"
> style="width:2.23427in;height:4.37583in" />
>
> Using the **Camera** icon, you can perform the following actions:

- Tap **Take Photo** or **Take Video** to capture new shots or videos
  for upload. If camera access is not enabled on your device, a message
  appears prompting for camera access. Tap **OK** to continue.

- Tap **Browse Photos or Videos** to browse and upload existing photos
  or videos from your device.

> <img src="media/image31.png" style="width:2.8125in;height:5.83333in" />

## View media

> Visualization Suite displays the uploaded photos and videos in the
> **Media** section of the incident record.
>
> <img src="media/image29.jpeg"
> style="width:2.23427in;height:4.37583in" />
>
> To open the **Media** section, tap **List** from the bottom navigation
> bar, tap on any incident record, and then scroll down. From the
> **Media** section, you can:

- Navigate through multiple photos and videos.

- Tap photo, pinch in and out to zoom in and out.

- Play video, rewind or fast forward for up to 10 seconds.

- Tap the **Full Screen** icon on the video to view the video in full
  size.

- Flip the mobile to view the photos or videos in the portrait or
  landscape mode.

- Increase or decrease the audio volume.

## Standard Operating Procedure

> A Standard Operating Procedure (SOP) in Hitachi Visualization Suite is
> a set of instructions compiled to help a workforce carry out routine
> operations for incident management.
>
> Individuals responsible for incident management must be made aware of
> SOPs that include objectives, roles, and procedures involved in every
> phase of the process.
>
> Tap **List** from the bottom navigation bar to open the list view, tap
> the incident record, and then tap **SOPs** to see the SOP steps
> associated with the incident.
>
> <img src="media/image32.png" style="width:2.8125in;height:5.80208in" />
>
> Following are some key points that you must know when working on SOPs:

- Each SOP step flows in a sequential order. For example, until step 1
  is completed, step 2 is disabled.

- Only incident assignees can work on the SOP steps.

- If an SOP step is already taken by another incident assignee, then you
  cannot select the **Assign it to me** option. Doing so results in an
  error message This step has already been assigned to *user name*.

- If you navigate to other screens without saving your comments for an
  SOP step, a prompt is displayed indicating that the comments will be
  lost. You can either select **Save**, **Discard**, or **Keep
  Editing**.

### Work on an SOP

> Only incident assignees can work on the SOP steps. To work on an SOP,
> complete the following instructions:
>
> **Procedure**

1.  Tap **List** from the bottom navigation bar. The incident records
    are displayed.

2.  <img src="media/image33.png" style="width:2.8125in;height:5.78125in" />Tap
    the incident record and tap **SOPs** from the bottom navigation bar.
    The SOP steps associated with the incident are displayed.

3.  Tap the available SOP step and select **Assign it to me**.

> If an SOP step is already taken by another incident assignee, then you
> cannot select the **Assign it to me** option. Doing so results in an
> error message This step has already been assigned to *user name*.

4.  Follow the instructions associated with the step, add your comments,
    and tap **Save as draft** to save your progress.

5.  Tap the tick mark next to the SOP step to complete the step. For
    example, select the tick mark next to **Re-enter** as shown in the
    following image to complete the SOP step.

> <img src="media/image34.png" style="width:2.8125in;height:5.83333in" />

6.  Repeat instructions from step 3 to work on other SOP steps.

### Unassign an SOP

> If you cannot work on an SOP step from your queue, you can unassign
> and release that SOP step. Other incident assignees can self-assign
> and work on that SOP step.
>
> **Procedure**

1.  Tap **List** from the bottom navigation bar. The incident records
    are displayed.

2.  Tap the incident record and tap **SOPs** from the bottom navigation
    bar. The SOP steps associated with the incident are displayed.

3.  Tap the SOP step that you want to unassign and clear the **Assign it
    to me** check box. The SOP step is unassigned and available for
    other incident assignees.

## Events

> You can tap **Events** from the bottom navigation bar to view the
> events associated with the selected incident.

<img src="media/image35.png" style="width:2.8125in;height:5.80208in" />

> The **Correlated Events** screen provides information on the event
> name and date timestamp of the event occurrence. To get more details
> about the event, tap the event record.
>
> <img src="media/image36.png" style="width:2.8125in;height:5.80208in" />
>
> From the **Correlated Events** screen, you can use the **Camera** icon
> to capture and upload new photos or videos of the incident, or browse
> and upload existing photos or videos. The captured photos or videos
> are displayed in the **Media** section of the incident detail record.
> For more information, see [<u>Upload Media (on page
> 325)</u>](#upload-media).

## Cameras

> You can tap **Cameras** from the bottom navigation bar to view the
> nearest cameras located within a specified radius from the incident
> location.
>
> <img src="media/image37.png" style="width:2.8125in;height:5.83333in" />
>
> **Note:** Live video streaming is not supported with the current
> version of Visualization Suite.
>
> The **Nearest Cameras** screen provides information on the number of
> cameras available near the incident, camera name, camera address,
> distance from the incident, and so on. To get more details about the
> camera, tap the camera record.
>
> From the **Nearest Cameras** screen, you can use the **Camera** icon
> to capture and upload new photos or videos of the incident, or browse
> and upload existing photos or videos. The captured photos or videos
> are displayed in the **Media** section of the incident detail record.
> For more information, see [<u>Upload Media (on page
> 325)</u>](#upload-media).

# User and support

> Using **More** from the bottom navigation bar, you can perform the
> following actions:

- Tap **Personal Information** to view information about the logged in
  user, such as name, email address, and associated groups.

- Tap **Help and Documentation** to open the Knowledge Portal and access
  the Visualization Suite documentation.

- Tap **About HVS** to view the version and application details.

- Tap **Legal Terms & Conditions** to open the **Privacy Policy** page
  within the Hitachi Vantara website.

# Troubleshoot

> You can log in to the Visualization Suite mobile app using the same
> login credentials used for the Visualization Suite web application.
>
> If you are unable to log in or get an error after logging in, refer to
> the various scenarios provided in this section to find a workaround.

#### Scenario 1: Unable to register the device with HVS

> You can get this error if your mobile device is already registered
> with HVS.
>
> <img src="media/image38.png" style="width:2.8125in;height:5.86458in" />
>
> You can either contact your administrator or delete the registered
> mobile from the HVS web application to resolve the issue. To delete
> the registered mobile, perform the following actions:

1.  Log into the HVS web application.

2.  Navigate to **Map \> Settings \> Memberships \> Users**.

3.  Select the user, click **Details**, and then delete the registered
    device.

4.  Uninstall the HVS mobile app.

5.  Reinstall the HVS mobile app.

6.  Follow the onboarding instructions. For more information, see
    [<u>Onboarding (on</u>](#onboarding) [<u>page
    308)</u>](#onboarding).

#### Scenario 2: Mobile license not enabled

> You can get this error if your mobile license is not enabled.
>
> <img src="media/image39.png" style="width:2.8125in;height:5.90625in" />
>
> Contact your administrator to resolve this issue.

#### Scenario 3: Incorrect login credentials

> You can get this error if your email address or password is incorrect.
>
> <img src="media/image40.png" style="width:2.8125in;height:5.86458in" />
>
> Perform any of the following actions to resolve this issue:

- Validate your login credentials.

- Check if you are able to log into the HVS web application. If the
  problem persists, contact your administrator.

#### Scenario 4: Incorrect values

> You can get this error if you have entered incorrect values in the
> input fields. To resolve this issue, validate your input values. If
> the issue persists, contact your administrator.
>
> <img src="media/image41.png" style="width:2.8125in;height:5.88542in" />

# Log out

> You can tap **More** from the bottom navigation bar and tap **Log
> Out** to log out of the Visualization Suite mobile app.
>
> When you are not actively using Visualization Suite, the mobile
> application will timeout and display the login screen.
>
> <img src="media/image42.png" style="width:2.8125in;height:5.80208in" />

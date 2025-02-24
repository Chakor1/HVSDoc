> The guide describes the features of Hitachi Visualization Suite and
> provides step-by-step instructions for using it.

# Overview

Hitachi Visualization Suite is a state-of-the-art software solution
that provides geospatial mapping of data from multiple sources to
provide operational insights. Visualization Suite provides
comprehensive integration capabilities with video and data devices,
analytics, and private entities. The integrated event data is
visualized over the map for easy access to real- time data.

Visualization Suite integrates with all major law enforcement systems,
including third-party video management systems, computer-aided
dispatch (CAD) or 911 systems, license plate readers, gun-shot
detection, and third-party sensors. This solution benefits both public
safety officials and private entities.

## Geospatial visualization of data from multiple sources

In today’s digitized world, both public and private organizations must
analyze a large amount of data coming from a multitude of sources. For
these organizations, accessing, correlating, and analyzing the data
can be a challenging task. Visualization Suite provides a “single pane
of glass” for geospatial visualization to gain the situational
awareness required to better respond to problems or even prevent them
from occurring.

<img src="media/image1.png" style="width:5.4375in;height:3.015in" />

## Cloud and on-premises solutions

Visualization Suite offers multiple deployment options. You can use
Visualization Suite as software as a service (SaaS), software deployed
on premises, or hybrid to match your IT infrastructure strategy.

## Video surveillance interoperability

The Visualization Suite video connectors allow you to integrate with
the existing video management systems (VMSs) and Hitachi Video
Management Software (HVMS), which gives a comprehensive, all-in-one
solution that simplifies video system deployment and management.

## Intelligent inspections

Hitachi Intelligent Infrastructure Monitoring (HIIM) solution helps in
remote inspection and monitoring of infrastructures. HIIM includes
thermal and visual spectrum cameras, rugged computers, edge and cloud
applications, video and data analytics, and HVS inspection engine
service.

The HIIM solution is integrated with HVS using the **Inspection
Automation** feature.

HIIM automates remote monitoring tasks, including temperature
tracking, digital and analog gauge readings, and overall health. It
ensures that critical components function optimally and within normal
operating ranges. This real-time monitoring helps identify potential
issues before they escalate into major problems, thereby minimizing
downtime and enhancing infrastructure safety and efficiency.

For more information, see <u>Administer intelligent inspections (on
page 82)</u>.

## Incident management and Standard Operating Procedure (SOP)

An incident is an event that is unplanned and can adversely affect an
organization and its business. For example, flooding of a building,
fire accident, or system failure.

Incident management in Visualization Suite enables you to create a
process that can help in restoring the normalcy within the designated
SLA and, thereby minimize the impact on the business operations.

You can classify incidents into the right incident type and manage
incidents based on the assigned priority, severity, and SOPs. See
<u>Manage incidents (on page 91)</u> for more information.

Visualization Suite allows you to create SOPs or guided responses for
every incident type. These step-by-step instructions help workers
responsible for incident management to carry out the routine
operations while following the necessary protocols. SOPs helps to
achieve efficiency and uniformity in performance, while reducing
miscommunication. See <u>Standard</u> <u>Operating Procedure (on page
93)</u> for more information.

## Dashboards

> The Dashboard feature provides visualization of historical event data
> and allows you to analyze event statistics. A custom dashboard add-on
> (available in release 6.0.0) extends the native analytics capability
> of Visualization Suite by allowing organizations to leverage Pentaho,
> Hitachi's industry-leading business intelligence software, to generate
> and publish custom reports to Visualization Suite.

## Entity management

Organizations rely on a variety of data from disparate sources in real
time to improve situational awareness. Visualization Suite lets you
tailor geospatial mapping of different types of data, or *entities*.
For example, you might want to view gunshots only within the past 12
hours, instead of all gunshots that have ever been reported. On the
other hand, stationary entities, such as buildings and cameras, are
persistently visualized as they provide important data points to
improve situational awareness.

## Data integration

> Visualization Suite integrates data from multiple sources, including
> analytics applications and sensors. The majority of events are
> ingested data that is aggregated automatically in Visualization Suite,
> eliminating the need for manual entry of each event. Events such as
> computer aided dispatch (CAD) events coming directly from 911 calls,
> gunshot detections coming from directory sensors, license plate
> recognitions, and social media events are immediately available from
> the map view.

## Data mapping

> Using the Data Mapping feature, HVS can seamlessly integrate with IoT
> sensors and process real-time data from various sources. For example,
> external sensors that detect alerts can transmit their data to the HVS
> ETL engine using either the HTTPS or MQTT protocol.
>
> The source data is then translated into HVS data using a data map
> created by the administrator, eliminating the need for a dedicated
> connector. This enables external IoT devices to send their data to HVS
> in real-time. This flexibility helps administrators to make data
> available on HVS independently.

## Slew to cue

> The automated workflows, "slew to cue," enable a sequence of actions
> triggered by an event. For instance, in the event of a gunshot, HVS
> can quickly locate the nearest camera, direct it to the scene,
> bookmark the event, and send a list of nearby cameras to the field
> responder. When the responder logs into the system, the camera is
> already focused on the incident scene, eliminating the manual process
> of finding and moving the camera. With one click, responders can play
> back the scene from 10 seconds prior. This feature is crucial in
> urgent situations where every second counts, allowing responders to
> act swiftly and effectively.
>
> Additionally, the bookmark feature enables investigators to identify
> and analyze the event later.

## Advanced configurable workflow

> Advanced configurable workflow helps HVS administrators to build
> custom conditions and select actions triggered by HVS entities. Each
> organization has unique assets and situations to manage, whether it is
> responding to gunshots, detecting intruders, or monitoring data
> anomalies during inspections.
>
> The highly configurable workflow accommodates these differences,
> enabling administrators to create conditions tailored to their
> specific needs. Administrators can use 'and' or 'or' conditions and
> group by expressions to build and execute actions when conditions are
> met.
>
> This automation streamlines processes and saves time compared to
> manual methods. For example, an operator will be notified when a gas
> meter anomaly is identified, a field responder will be alerted when a
> gunshot is detected, or an HVS entity will be pushed to an external
> system when emergency events are detected.

## Identity management

> Hitachi Visualization Suite users are now managed by a common identity
> management service that enables single-sign on across other Hitachi
> applications. In addition, this service enables integration with the
> customer’s active directory service. The existing HVS user management
> service is still used for service accounts for third party system
> integrations.

## Role-based user permissions

> HVS role-based permissions are highly configurable. You can use groups
> to associate users by organization and control their access to
> specific entities and actions within HVS domain. For example, a police
> department group can have cameras located within their district, with
> no visibility outside of that area. Some officers might have live
> viewing capabilities, while investigator officers might only have
> playback access to view past incidents. Field responders might have
> access to car accident scenes, while operators within a building might
> have visibility over building management assets and events, such as
> stolen cards or broken doors. This allows each operator to focus on
> their specific responsibilities. To set this up, you first define
> rules that specify the level of access users will have to various
> entities, and then assign these rules to each group.

## Timeline feature

> The Timeline feature can be used to view historical data. Using
> Timeline, you can go back and view a snapshot of entities (events,
> inspections, incidents) for a specific time of day. Timeline also
> gives easy access to archived footage and event data, enabling you to
> view scenes for a specific time around the event. See [<u>View entity
> timelines (on page 158)</u>](#view-entity-timelines).

## Search capabilities

> Visualization Suite allows you to search for particular events and
> objects by setting a search area. For example, you can look for all
> burglaries and CAD calls for the last three days within the city
> limit. Results that match these criteria are displayed on the map view
> and the list view. For details, see [<u>Use search (on page
> 162)</u>](#use-search).

## Language options

> The HVS user interface is designed to be globally accessible, offering
> support for multiple languages. This ensures that users from diverse
> linguistic backgrounds can easily navigate and utilize the software.
> For more information about how to select your preferred language, see
> [<u>User preferences (on page 183)</u>](#user-preferences).

## Security

> Visualization Suite is designed with advanced security features to
> ensure the safety and security of the sensitive data. Because the data
> processed by the visualization system can be classified, all data
> going from the client network to Visualization Suite is
> unidirectional. Traffic going from behind the client secure network to
> the encrypted HVS Cloud Services is secured through Hitachi Vantara
> LLC Visualization Platform (HVP). See <u>Security overview (on</u>
>
> <u>page 16)</u> for details.

## Gateways

> Hitachi Vantara LLC Edge Gateway for Video is an intelligent edge
> device that integrates third-party video systems and performs
> transcoding for optimal cloud livestreaming and recording. Edge
> Gateway for Video also acts as a data ingestion service for external
> sensor data. Depending on the number of simultaneous livestreams
> anticipated from the source systems, several gateway options are
> available. A gateway combined with the Visualization Suite software
> enables a seamless integration into private-entity security assets.
>
> For details about the Visualization Suite video gateway, see the
> Installation Guide using the OVF templates.

## End-to-end IoT solution for smart cities

> As one of the Hitachi's Smart Spaces and Video Intelligence solution
> offerings, Visualization Suite gives end-to-end, adaptable, and
> intelligent solutions for smart cities. These solutions use
> integration of big data, including video feeds, event data, and social
> media, to give real- time analytics that public safety officials can
> act on.
>
> <img src="media/image2.png" style="width:5.33333in;height:3.32667in" />
>
> All solution components in the Smart Spaces and Video Intelligence
> solution stack are modular, functioning as building blocks for smart
> cities. They help all areas and organizations become safer and more
> effective, so they can thrive. The following video intelligence
> solutions are available for integration with Visualization Suite or
> for standalone deployment:

- [<u>Hitachi Video Analytics
  (HVA)</u>](https://knowledge.hitachivantara.com/Documents/Industry_Specific/Smart_Spaces_and_Video_Intelligence/Video_Analytics)

- [<u>Hitachi Video Management Software
  (HVMS)</u>](https://knowledge.hitachivantara.com/Documents/IoT/Smart_Spaces_and_Video_Intelligence/Video_Management_Software/HVMS)

- [<u>Hitachi Video Management Software Base (HVMS
  Base)</u>](https://knowledge.hitachivantara.com/Documents/IoT/Smart_Spaces_and_Video_Intelligence/Video_Management_Software/HVMS_Base)

# Get started

> The Visualization Suite administrator creates your user account and
> provides access to log in to the application.
>
> You receive an email from your administrator with a link to update
> your account. Click the link and reset the password. See [<u>Password
> reset (on page 144)</u>](#password-reset) for more details.
>
> After resetting the password, you can access the Visualization Suite
> application.

## Password reset

> You must reset the user account password in the following scenarios:

- User account is created.

- User account expired.

- User account is locked.

- Forgot user account credentials.

> Perform the following steps to reset the password:

#### Procedure

1.  Click **Forgot your credentials?** in the Hitachi Visualization
    Suite login window.

<img src="media/image3.jpeg" style="width:5.8in;height:2.83052in" />

> The **Recover Credentials** page appears.

2.  Enter the email address associated with your account username.

3.  Click **Recover**.

<img src="media/image4.jpeg" style="width:5.6in;height:2.73292in" />

> An email with "Hitachi Visualization Suite Manage account" as the
> subject is sent to your specified email address.

4.  Check your inbox for the email.

> **Note:** If you do not receive the confirmation message within a few
> minutes of submission, check your **Junk E-mail** folder to see if the
> confirmation email was delivered to that folder instead of your inbox.
> If yes, select the confirmation message and click **Not Junk** to
> receive future messages directly in your inbox.
>
> <img src="media/image6.jpeg" style="width:5.5in;height:2.08in" />

5.  Click **Reset Password** link or copy the link and paste it into a
    browser.

> **Note:** The reset password process automatically expires after a
> period of time. Default time is 5 minutes.

6.  Enter **New Password**, then enter **Confirm Password**. Provide a
    password that meets with Visualization Suite password policy.

7.  Click **Recover** and access the Visualization Suite application.

# Use the map

> You can visualize integrated data from multiple sources using the map
> view. Map enables you to view every entity related to events,
> inspections, incidents, and objects in real-time.
>
> By default, HVS is configured to use Google Maps. However, it supports
> other custom map configurations as well. Contact your administrator
> for more information.
>
> **Map** displays the available entities in the left pane. Each entity
> is categorized based on the entity type. For example, **Objects**
> lists the stationary and camera related entities. When you click the
> camera entity, HVS displays the map markers related to all cameras on
> the map. To remove the map markers from the map view, click camera
> again.
>
> You can use the left pane to filter the map markers on the map view.
> To get quick information about an entity in the **InfoWindow**, click
> the map marker.

## Map view

> The map view includes several key components to help you visualize
> every entity in HVS.
>
> <img src="media/image7.jpeg" style="width:4.92281in;height:2.53208in" />

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr>
<th style="text-align: center;"><strong>Items</strong></th>
<th style="text-align: center;"><strong>Description</strong></th>
</tr>
</thead>
<tbody>
<tr>
<th>Left pane</th>
<td style="text-align: left;"><p>Contains the entity types and menu
items. A few entities in the entity type show heat map and view detail
icons.</p>
<p>Expand the entity type and select the entity you want to display on
the map:</p>
<ul>
<li><p><strong>Events</strong>: Displays events that can occur suddenly,
such as gunshots or 911 calls under different event types.</p></li>
<li><p><strong>Incidents</strong>: Displays incidents that impact
normalcy of business operations.</p></li>
<li><p><strong>Inspections</strong>: Displays inspections created for
monitoring infrastructure.</p></li>
<li><p><strong>Objects</strong>: Displays the stationary items, such as
buildings and cameras.</p></li>
<li><p>Heat map icon: Shows the intensity of the entity.</p></li>
<li><p>View Details icon: Takes you to the entity detail page.</p></li>
<li><p><strong>Maps and Layers</strong>: Displays the available layers
and map options such as ESRI, Google Maps configured in the
system.</p></li>
<li><p><strong>Settings</strong>: Displays the settings that are
available for configuration based on your access permissions. For
example, domains, memberships, audit, and others.</p></li>
<li><p><strong>Timeline</strong>: Displays historical data for the
events.</p></li>
</ul></td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr>
<th style="text-align: center;"><strong>Items</strong></th>
<th style="text-align: center;"><strong>Description</strong></th>
</tr>
</thead>
<tbody>
<tr>
<th>Top pane</th>
<td>Contains the core entity types that are available for configuration
based on your access permissions. For example, entity types, entities,
gateway, and others.</td>
</tr>
<tr>
<th>Utility menu</th>
<td><p>Contains the following options:</p>
<ul>
<li><p>Help: Enables access to documentation.</p></li>
<li><p>Open new HVS window: Enables you to open multiple HVS windows to
display Map view, Videowall, and more side-by- side.</p></li>
</ul></td>
</tr>
<tr>
<th>Incident KPIs</th>
<td>Provides a quick overview of the incidents logged in HVS.</td>
</tr>
<tr>
<th>Map markers</th>
<td>Displays the location of the event, incident, inspection, or object
on the map view.</td>
</tr>
<tr>
<th>InfoWindow</th>
<td>Provides a quick summary of an entity on the map view.</td>
</tr>
</tbody>
</table>

## Display entities on the map

> You can show all or only select entity types on the map. For example,
> you may only want to see the gunshot incidents on the map to get
> real-time gunshot summaries for your domain. With this map you have
> instant access to event reports describing when and where the gunshots
> occurred on the live map (including physical addresses), system
> generated log entries, and nearest cameras. When viewing the map you
> can visualize and analyze the location of gunshots, cameras, and other
> assets in the area.

#### Procedure

1.  Click **Map**.

2.  From the left pane, expand the required entity types, and select one
    or more entities you want to display on the map.

## Use InfoWindows

> An **InfoWindow** provides a quick summary of an entity on the Map
> view. You can view information related to date and time, description,
> images, live stream, and so on depending on the entity such as
> **Events**, **Incidents**, and **Objects**.
>
> Within the **Map** view of the HVS, you can display the **InfoWindow**
> using one of the following methods:

- From the left pane, click the entities under **Events**,
  **Inspections**, **Incidents**, and **Objects**.

- On the map, click the map marker related to these entities.

> <img src="media/image8.jpeg" style="width:5.46833in;height:4.73167in" />
>
> The **InfoWindow** includes the following key features:

- Draggable

- Selectable

- Automatic live stream for cameras

- Display camera status in color on the top bar of the **InfoWindow**

- Action buttons vary depending on the entity. For example, incident
  **InfoWindow** includes action buttons to expand the image or video,
  view incident details, and close the info window.

- Remain open during the active session

- Highlight selected InfoWindow for visual ease and identification

- Display the selected InfoWindow automatically in the front

- Open up to 10 camera InfoWindows and 10 other entity InfoWindows at a
  time

- Remain intact in the map view irrespective of map zoom in, zoom out,
  and pan action

> **Note:** The **InfoWindow** persists during an active session.
> Leaving the map view does not close the **InfoWindow**. When you
> return to the map view, any previously opened **InfoWindow** is
> restored during the active session. The **InfoWindow** closes when you
> log out of the HVS. When you log back in, the map view does not
> display the **InfoWindow**.

### Action buttons

> The **InfoWindow** provides the following actions buttons based on the
> selected entity on the map:

|  |  |
|----|----|
| <img src="media/image9.png" style="width:0.20854in;height:0.20854in" /> | Displays the floor plan for the entity. You can also view **InfoWindow** from the floor plan view. |
| <img src="media/image10.png" style="width:0.18802in;height:0.15833in" /> | Expands the image or video added for an entity. Hover over an area to magnify and see it in detail. |
| <img src="media/image11.png" style="width:0.1875in;height:0.1875in" /> | Closes the **InfoWindow**. |
| <img src="media/image12.png" style="width:0.1875in;height:0.17708in" /> | Opens the entity details page. |
| <img src="media/image13.png" style="width:0.1875in;height:0.1875in" /> | Displays the live stream with additional camera details in a separate window. |
| <img src="media/image14.png" style="width:0.18833in;height:0.18833in" /> | Opens the videowall list window to add camera to selected videowall. |
|  | Expands and collapses the image view. |

### Move InfoWindows

> The **InfoWindow** can be moved within the map view. You can easily
> drag an **InfoWindow**
>
> within the current map view.

#### Procedure

1.  Move the mouse pointer to the **InfoWindow**.

2.  When the cursor changes to pointer cursor, press and hold down.

3.  Drag the **InfoWindow** to the required location by moving the
    pointer.

### View multiple InfoWindows

> You can open up to ten camera **InfoWindows** and ten other entity
> **InfoWindows** per **Map** window during an active session. If you
> have multiple map windows by using the new Visualization Suite window
> icon, you can open up to 10 **InfoWindows** in each of your map
> windows.

- The maximum number of the InfoWindow value is system parameter, and it
  is not per domain.

- Default value is ten camera **InfoWindows** and ten other entity
  **InfoWindows** for both the on-premises and cloud environments.

#### A snack-bar message

> When you reach the maximum number of **InfoWindows**, the snack-bar
> message shows up, as shown in the following example:

<img src="media/image17.jpeg" style="width:5.555in;height:3.08in" />

> The message appears only for 5 seconds. If you must stream a different
> video camera or other entity, close one of the **InfoWindows**, then
> open another **InfoWindow** to stream live video.

#### Opening multiple windows to view more live streaming

> You can click the Open a New Visualization Suite Window icon from the
> menu bar to include additional map views in a new window, as shown in
> the following example:

<img src="media/image18.jpeg" style="width:5.6in;height:2.49375in" />

### View camera InfoWindow

> You can click on a camera map marker to display the camera
> **InfoWindow**.
>
> The **InfoWindow** identifies the camera status, the name of the
> camera, the camera's location (address), and has features that support
> automatic video streaming, PTZ control and action buttons to link to
> video wall lists, snapshot, a preview panel, camera details, and an
> option to close the **InfoWindow**.
>
> The camera **InfoWindow** includes the following key features:

- [<u>View live video streams (on page
  152)</u>](#view-live-video-streams)

- [<u>Use PTZ camera (on page 152)</u>](#use-ptz-camera)

### View live video streams

> You can click camera map marker from map view to stream live video on
> **InfoWindow** in your domain. You can enable up to 10 windows and
> view live videos on the map view. You can move and place the
> **InfoWindow** as required and organize the map view with live
> streams.
>
> You can click the play icon to view additional information for the
> camera, such as address and description.

<img src="media/image19.jpeg"
style="width:5.46833in;height:2.62083in" />

#### Procedure

1.  Click **Map**.

2.  Expand **Objects** to view the available object entity types.

3.  Select **Camera** to view the available cameras.

4.  Click the camera name to highlight the selected camera map marker on
    map view.

5.  Click the camera map marker to view the **InfoWindow**.

6.  Click the collapse icon to close the left pane and extend the map
    view area with multiple

> **InfoWindows** to stream live video.

### Use PTZ camera

> A pan-tilt-zoom (PTZ) camera is capable of remote directional and zoom
> control. When a PTZ camera is selected, the **InfoWindow** shows the
> PTZ controls for moving the camera up, down, right, left, zoom in, and
> zoom out:
>
> <img src="media/image20.jpeg"
> style="width:3.64583in;height:4.03125in" />
>
> Preconfigured camera positions, called a **Preset**, are listed in the
> **InfoWindow.** A **Preset** is created in the camera and listed in
> the HVS system. Camera presets can be selected from the **InfoWindow**
> to change the camera view. For example, you can select Preset1 looking
> north, Preset2 looking south, Preset3 looking east, and so on. You can
> select a preset to make it easy for an operator to monitor an event in
> a specific direction.

### Play audio

> Before you proceed, contact your system administrator to enable the
> Microphone option for the camera and provide permissions to use the
> video. For more information, see <u>Enable live</u> <u>audio (on page
> 71)</u>.
>
> When audio is enabled on a camera, the audio control is available for
> turning on, turning off, or adjusting the volume of the video. The
> following figure shows an example of a live video with the audio
> control in the preview pane. When viewing multiple videos on a
> videowall, you can only have one audio session at a time. If an
> existing audio is active in a session, turning on audio for another
> video automatically turns off the current audio session.
>
> <img src="media/image21.jpeg"
> style="width:5.52812in;height:4.37719in" />

## View event details

#### Procedure

1.  To view event details, do one of the following:

    - From the left pane, click the view details icon next to the event
      entity.

    - On the map, click the event entity map marker. From
      **InfoWindow**, click the view details icon to view the event
      details page

2.  In the event details page, you can:

    - View event details, location, and nearest cameras (if configured).

    - Zoom in and out of an image.

    - Download images and videos.

    - Hover over an area to magnify and see it in detail.

    - In the **Nearest Cameras** section, you can:

      - Click the play icon to view live stream in **InfoWindow**.

      - Open up to ten **InfoWindow** at a time.

      - If the camera is PTZ enabled, you can view the PTZ controls in
        **InfoWindow**.

      - Click playback icon to view recorded videos.

## View inspection details

#### Procedure

1.  To view inspection details, do one of the following:

    - From the left pane, click the view details icon next to the
      inspection entity.

    - On the map, click the inspection entity map marker. From
      **InfoWindow**, click the view details icon to view the inspection
      details page

2.  In the inspection details page, you can:

    - View inspection details and location.

    - Zoom in and out of an image.

    - Download images and videos.

    - Hover over an area to magnify and see it in detail.

## View incident details

#### Procedure

1.  To view incident details, do one of the following:

    - From the left pane, click the view details icon next to the
      incident entity.

    - On the map, click the incident entity map marker. From
      **InfoWindow**, click the view details icon to view the incident
      details page

2.  In the incident details page, you can:

    - View incident details, location, SOP, events, and nearest cameras
      (if configured).

    - In the **Nearest Cameras** section, you can:

      - Click the play icon to view live stream in **InfoWindow**.

      - Open up to ten **InfoWindow** at a time.

      - If the camera is PTZ enabled, you can view the PTZ controls in
        **InfoWindow**.

      - Click playback icon to view recorded videos.

## View object details

> Objects can be stationary, moving, or camera.

#### Procedure

1.  To view object details, do one of the following:

    - From the left pane, click the view details icon next to the object
      entity.

    - On the map, click the object entity map marker. From
      **InfoWindow**, click the view details icon to view the object
      details page

2.  In the object entity details page, you can:

#### Objects (stationary):

- View object details and location.

- View the floorplan associated with the object.

- If the floorplan has cameras, click the camera icon to view the video
  streams in

**InfoWindow**. You can open up to ten **InfoWindow** at a time.

- **Objects (moving)**: In the object entity detail page, view object
  details and location.

- **Objects (camera)**: In the camera detail page, view camera details,
  status, and location.

## View nearest cameras

> Visualization Suite lists the cameras available within the specified
> distance for event and inspection entities.

#### Before you begin

> Contact your administrator to enable this feature for event and
> inspection entity types. For more information, see <u>Enable find
> nearest cameras (on page 75)</u>.

#### Procedure

1.  Click **Map**.

2.  From the left pane, expand the event or inspection entity types, and
    select one or more entities you want to display on the map.

3.  Click the event or inspection map marker.

4.  In the **InfoWindow**, click the view details icon.

5.  In the entity detail page, click **Nearest Cameras**.

<img src="media/image22.jpeg"
style="width:4.74458in;height:1.94208in" />

6.  In the **Nearest Cameras** section, click **here** from the **To
    show the nearest cameras, please click here** message.

> The cameras nearest to the event entity are displayed. If the camera
> is online, click the play icon to view the live camera stream in
> **InfoWindow** and playback icon to view recorded videos.
>
> By default, the playback automatically starts 10 seconds before the
> event timestamp.

## View an event-triggered snapshot

> When an event occurs, one of the most common ways to investigate it is
> to check video recordings from the surrounding area. Visualization
> Suite takes a snapshot of nearby PTZ and non-PTZ cameras within a
> maximum one-mile radius. A snapshot can be accessed from the event
> details page where you can view a list of all cameras from the
> surrounding area with PTZ camera preset information and a quick
> playback link to each recording.
>
> **Note:** Contact your system administrator if you want to receive
> email notifications when certain events occur. Email notifications
> include the same list of PTZ and non-PTZ cameras that you can access
> in the Visualization Suite Web interface.

#### Before you begin

> Contact your system administrator to enable the slew-to-cue option for
> event entity types.

#### Procedure

1.  Perform any of the following tasks:

    - From the left pane, click the view details icon next to the event
      to view the entity details page.

    - Or, on the map, click the map marker of an event. From the
      **InfoWindow**, click the view details icon.

2.  In the **Nearest cameras** section, playback videos from the nearest
    PTZ and non-PTZ cameras found within the set radius from the event
    are displayed.

> **Note:** The **Cameras** tab is not available if there are no cameras
> in the range. Additionally, make sure permissions are configured for
> the camera.

3.  Click the icons under **Live** to view live streaming or
    **Playback** to view the video recording of the event.

## Track a moving entity status

> By default, tracking is enabled for moving entity type in
> Visualization Suite.
>
> By hovering your mouse over the Status icon in the map, you can
> quickly identify the tracked status of the entity. Color coding, which
> can be customized in the Settings menu, provides a helpful visual cue
> of the entity's status.
>
> In the following example, information about a selected metro train
> (highlighted within the blue square) is displayed in the right panel.
> Clicking the train opens the right panel, which displays a
> corresponding 'dot' color status, which is orange in this example.
> When you hover your mouse over the dot indicator, a status description
> is provided.
>
> Clicking the view details icon provides more information about the
> train, and its status.

<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 60%" />
</colgroup>
<thead>
<tr>
<th><blockquote>
<p><strong>Status</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Description</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Tracking conditions</strong></p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr>
<th>Unknown</th>
<td>The entity has no tracking data.</td>
<td>Hitachi Visualization Suite is not receiving GPS data. The entity
might not be configured correctly (for example, router data is
missing).</td>
</tr>
<tr>
<th>Online</th>
<td>The entity is being actively tracked.</td>
<td>Hitachi Visualization Suite is receiving GPS data.</td>
</tr>
<tr>
<th>Offline</th>
<td>The entity is not being tracked.</td>
<td>Hitachi Visualization Suite is not receiving GPS data because the
duration that was set for the entity offline status has expired. The
offline status is specified by the Watchdog timer within the Settings
module.</td>
</tr>
<tr>
<th>Parked</th>
<td>The entity location is known and is stationary.</td>
<td>Hitachi Visualization Suite is receiving GPS data, the current
location is within the parked Distance Threshold values that were
specified for the entity.</td>
</tr>
</tbody>
</table>

## View entity timelines

> Timeline allows you to see the entities over time, daily or monthly.
>
> **Note:** Timelines as displayed in the Map cannot be exported.
> However, if you create custom reports using the advanced reporting
> feature (requires a Custom Dashboards license), they can be exported.
> For more information about the advanced reporting in Visualization
> Suite, see the dashboard related documentation in the Administrator
> Guide.

#### Procedure

1.  From the left pane, click **Timeline**.

> <img src="media/image23.jpeg"
> style="width:5.47542in;height:3.01042in" />

2.  Click anywhere on the timeline bar graph to switch to the monthly
    view.

<img src="media/image24.jpeg" style="width:5.4825in;height:3.08833in" />

3.  Click **Back to monthly view** to return to the monthly view.

<img src="media/image25.jpeg"
style="width:4.99229in;height:1.06562in" />

## View incident KPIs

> The Incident Key Performance Indicators (KPI) provides a quick
> overview of the incidents logged in the Visualization Suite.
>
> You can view the incident KPIs on the map view and get information on
> the number of open incidents, today's total incidents, unassigned
> incidents, and overdue incidents for a given geographic area. For
> example, an entire city or a specific district.

<img src="media/image26.png" style="width:4.74458in;height:0.46708in" />

> To view the incidents list, click the list icon next to Overdue
> Incidents. You can find your incident records by using the search
> function, applying filters, or based on the incident created date.
>
> You can switch back to map view by clicking the map icon. To view the
> incident detail record, click the view details icon.

<img src="media/image27.png" style="width:4.74458in;height:0.94646in" />

## Use map markers

> The map marker is used to mark the location of the entity, inspection,
> incident, or object on the map view. Click the map marker to open the
> **InfoWindow**, which provides an information summary of the entity on
> the map view.
>
> The cluster map marker indicates the presence of multiple entities in
> the same location. The cluster map marker displays a number indicating
> the number of entities available in the cluster.

<img src="media/image28.jpeg"
style="width:3.33667in;height:3.58312in" />

> Zoom in or click the cluster map marker to expand the cluster. When
> expanded, you can view the individual map markers for each entity. The
> map markers display the color associated with the entity type.
>
> When you zoom out, the application displays the cluster map marker.
> The cluster map marker displays the color associated with the event.

## Open multiple windows

> You can open multiple HVS windows to display Map view, Videowall,
> Insights, and more side- by-side.
>
> Click the Open new HVS Window icon from the Utility menu to review
> information in a new window.

<img src="media/image29.jpeg"
style="width:4.34146in;height:3.83906in" />

> The multiple window view helps you manage and monitor events in
> real-time with map, video, and reporting information side-by-side. It
> provides one complete view of all critical information for seamless
> event management.
>
> When you log out of Visualization Suite in one window (newly opened or
> the original) it ends your session in all open windows.
>
> The following is an example of multiple open windows on a desktop
> monitor.
>
> <img src="media/image30.png" style="width:4.28667in;height:2.29333in" />

## View HVS connection status

> The HVS application connects to the RabbitMQ, a messaging broker to
> transfer messages.
>
> The message status indicates the connection status between
> Visualization Suite and RabbitMQ messaging broker. Green indicates
> that it is connected and red indicates otherwise.

## Use search

> Using the Search function, you can quickly collect and correlate data
> for an investigation, such as CAD incidents, records, LPR hits,
> recorded surveillance, and body worn videos. You can use keyword and
> other metadata to find relevant information from several entities
> registered in your Visualization Suite domain.
>
> For example, if you are investigating a hit-and-run incident, you can
> search for CAD events, LPR hits, and video recording from the cameras
> near the location of the incident based on the time of the event.
>
> The following figure shows the Visualization Suite search window.

<img src="media/image31.jpeg"
style="width:5.46833in;height:2.62792in" />

#### Filter Icon

> <img src="media/image32.png" style="width:0.18333in;height:0.20833in" />
> Opens the search window.

#### Search pane

> Provides the search input fields.

#### Search map

> Displays search results on the map with markers that indicate
> locations. Markers are color coded by entity type.

#### Zoom in/out

> <img src="media/image33.png" style="width:0.56227in;height:0.22872in" />
> Zooms in (+) to narrow down (-) or out to expand the search area.
> Click
>
> Search to refresh and apply new zoom settings on an existing search.

#### Go to location

> <img src="media/image34.png" style="width:0.1875in;height:0.19602in" />
> The Go to location icon displays the selected entity in center of the
> map and zooms in automatically.

#### Search result pane

> The left pane lists the search results and shows a breakdown by entity
> type and statistics (total and aggregate).

#### Hide or show results

> <img src="media/image35.png" style="width:0.32857in;height:0.15714in" />
> Click the Collapse and Expand icon on the bottom left corner of the
> map window to hide or show the search results.

### Create a search

> Search results are filtered based on the location, entity types,
> specified date or time range.

#### Procedure

1.  (Optional) On the search window, set the search area by entering a
    location or using the

> **Zoom In** and **Zoom Out** icons located at the bottom of the map .
>
> **Tip:** You can also change the location after the search displays
> results. Refresh the search to reflect the new location settings.
>
> <img src="media/image37.jpeg" style="width:5.475in;height:2.81875in" />

2.  Click the Search icon and set the search criteria by entering one or
    more of the following parameters:

> <img src="media/image38.png" style="width:2.76792in;height:6.00979in" />

#### Keyword

> Enter a keyword or a phrase. You can enter a minimum of three words
> and the search is not case-sensitive. Visualization Suite searches
> only entity names and descriptions.

#### Match exact phrase

> Select the **Match exact phrase** check box to find the exact match of
> a keyword or phrase.
>
> If you know the search phrase, it is suggested to use the **Match
> exact phrase**
>
> option for faster search results.
>
> For example, the table provides details on the search time with and
> without using the **Match exact phrase** option for a system with the
> following MongoDB server sizing specifications:

- Environment: Azure

- Type: Standard D4s v3

- vCPUs: 4

- Memory: 16 GiB

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr>
<th><blockquote>
<p><strong>Number of HVS events in your domain</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>With Match exact phrase</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Without Match exact phrase</strong></p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr>
<th>1 million</th>
<td>0.3 seconds</td>
<td>10 seconds</td>
</tr>
<tr>
<th>5 million</th>
<td>0.3 seconds</td>
<td>55 seconds</td>
</tr>
<tr>
<th>10 million</th>
<td>0.3 seconds</td>
<td>2 minutes</td>
</tr>
<tr>
<th>15 million</th>
<td>0.3 seconds</td>
<td>3 minutes</td>
</tr>
<tr>
<th>30 million</th>
<td>0.3 seconds</td>
<td>NA. The HVS is unable to return the result and is timed out.</td>
</tr>
<tr>
<th>50 million</th>
<td>0.3 seconds</td>
<td>NA. The HVS is unable to return the result and is timed out.</td>
</tr>
</tbody>
</table>

> For records greater than 30 million, without **Match exact phrase**
> the HVS API is unable to return the results and shows 500 - request
> timed out error in the response body and HTTP/1.1 500 Internal Server
> Error in the response header. It is recommended that you increase the
> MongoDB server size to mitigate such issues.

#### Search in current map view

> Select the check box to search the area shown on the map (includes the
> left side of the map covered under the result pane). Clear the check
> box to search the entire continent.

#### Entity types

> Select all entity types that apply. Moving entity types cannot be
> selected and are excluded from search criteria.

#### Incident types

> Select all incident types that apply.

#### Time interval

> Select a time interval from the last 2, 8, 12, 24 hours, or a specific
> date range. To specify a date range, select **Date range** from the
> list, then enter a **From** (start) date and a **To** (end) date.

#### Sort by

> Select the sort order. You can sort by date or name in the ascending
> or descending order.

3.  Click **Search**.

#### Result

> Visualization Suite searches the domain for entities that match the
> criteria and displays results both on the map and in the result pane.
>
> **Note:** A search you create in Visualization Suite persists during a
> session. Leaving the search window does not cancel or clear the search
> filters. The search is lost when you log out of Visualization Suite.

### View search results in the search map

> The search map uses markers to show the location of entities from
> search results (markers are color-coded by entity type). It provides
> an at-a-glance view of key locations for an investigation.
>
> Clicking on a marker displays the entity information in the preview
> pane on the right. From the preview pane, you can:

- View the details by clicking on the View Details button.

- Click x to exit the preview pane and return to the search pane.

<img src="media/image39.jpeg"
style="width:5.71698in;height:2.64031in" />

### View search results in the search result pane

> The search result pane provides a list of entities grouped and
> color-coded by entity type. The pane provides a breakdown and the
> statistics of the search results.
>
> <img src="media/image40.png" style="width:1.68396in;height:1.9175in" />
>
> The following list describes the information and the functions
> available in the search result pane:

#### Entities

> All entities that matched the search criteria are shown with the time
> and address metadata (the metadata availability depends on the entity
> types).
>
> If address is not shown for an entity, click the entity to see address
> in the preview pane.
>
> Clicking on an entity shows the entity information, such as address
> and case ID, in the preview pane. From here, you can:

- Click View Details.

- Click x to close the preview pane and return to the search pane.

#### Entity type

> When expanded, an entity type shows entities.
>
> Each entity type shows two numbers in parenthesis, such as (10 of
> 435). For example, 10 of 435 means the only the first 10 out of 435
> that match the search criteria are listed. This is because the system
> limits the number of results to display per search (the display upper
> limit is configurable by administrator).
>
> Note that stationary entities, such as buildings, do not have
> timestamps.

#### Go to the entity on the map

> Use the Go to location icon next to the entity to zoom in.

#### The time of search

> The time the search query was sent.
>
> Note that the displayed results are static. To update the results,
> refresh the search by clicking Search on the search pane.

#### Total number of search results

> The total number of entities displayed. The aggregate total of the
> results is displayed for each entity type.

#### View details

> Use the View Details icon to view the event details.

# Use cameras

> Use **Cameras** to watch live streams, playback videos, take snapshots
> from videos, set up recording on your camera, view archived videos,
> and so on.

## Camera status

> Within Visualization Suite's **Map view**, **InfoWindow**,
> **Videowall**, **Search Map**, and **Camera list** areas, the camera
> status is visually identifiable, which helps users determine which
> active camera can be used to stream video.
>
> Camera status is the online status of Video Management System (VMS)
> and IP cameras.

#### Camera status

<table>
<colgroup>
<col style="width: 10%" />
<col style="width: 6%" />
<col style="width: 58%" />
<col style="width: 25%" />
</colgroup>
<thead>
<tr>
<th><blockquote>
<p><strong>Status</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Ico n</strong></p>
</blockquote></th>
<th><strong>Description</strong></th>
<th><blockquote>
<p><strong>Video Streaming</strong></p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr>
<th>Green</th>
<td><img src="media/image41.jpeg"
style="width:0.16646in;height:0.16646in" /></td>
<td>camera is online</td>
<td>Streams the video</td>
</tr>
<tr>
<th>Red</th>
<td><img src="media/image42.jpeg"
style="width:0.16646in;height:0.16646in" /></td>
<td>camera is offline</td>
<td>Does not stream the video</td>
</tr>
<tr>
<th>Yellow</th>
<td><blockquote>
<p><img src="media/image43.jpeg"
style="width:0.15583in;height:0.16646in" /></p>
</blockquote></td>
<td>camera does not exist in VMS</td>
<td>Streams the video</td>
</tr>
<tr>
<th>Grey</th>
<td><img src="media/image44.jpeg"
style="width:0.16646in;height:0.16646in" /></td>
<td>camera status is not available</td>
<td>Might not stream the video</td>
</tr>
<tr>
<th>Purple</th>
<td><blockquote>
<p><img src="media/image45.jpeg"
style="width:0.14521in;height:0.14875in" /></p>
</blockquote></td>
<td>video gateway is offline</td>
<td>Does not stream the video</td>
</tr>
</tbody>
</table>

> **Camera status on left panel and InfoWindow on Map view**

<img src="media/image46.jpeg"
style="width:5.46833in;height:2.62792in" />

1.  Camera list with camera status icon.

2.  Online camera status on InfoWindow sample.

#### Camera status on camera search on Videowall

<img src="media/image47.jpeg" style="width:5.46833in;height:2.72in" />

> Camera search result with camera status icon on videowall.
>
> **Camera status on search result panel on search map view**

<img src="media/image48.jpeg"
style="width:5.46833in;height:2.62083in" />

> **Camera status on camera list**

<img src="media/image49.png" style="width:5.56875in;height:2.74875in" />

## View videos

> Save, export, and archive video footage from within Visualization
> Suite.
>
> For video snapshots of video events (motion detection or line crossing
> as examples) from Orchid IP Configure cameras.

### View archived videos

> You can view live video from cameras in your domain. If the camera is
> set up to record, you can also view archived recorded video from it.

#### Procedure

1.  On the map, select the camera corresponding to the video you want to
    view.

2.  In the video, click the **Play** icon to open the live video in a
    separate window.

<img src="media/image50.png" style="width:5.46833in;height:2.635in" />

3.  Do any of the following:

    - <img src="media/image51.jpeg"
      style="width:5.44781in;height:2.76469in" />To view live video,
      click the **Live** tab and use the controls to zoom in or out and
      change viewing angles.

    - <img src="media/image52.jpeg" style="width:5.58562in;height:2.205in" />To
      view recorded video, click the **Archive** tab, choose the date
      and time of the video you want to view, then click **Playback**.
      The following figure shows archived video from the selected
      camera.

    - To view recorded video from an event that occurred in the
      proximity of the camera, go to the **Archive** tab and select an
      event in the **Latest events** near the camera list.

### Export video snippets

> You can export video snippets from cameras that support video exports.
> To export a video, do the following:

#### Procedure

1.  From the top pane, navigate to **Settings** \> **Camera**.

2.  Click the edit icon for the camera you want to export archived
    videos.

3.  Click **Archive**.

4.  Enter details regarding the **Clip title**, **Start date and time**
    , and **End date and time**.

5.  Click **Export**.

> A system notification confirms the success of the export along with
> the location of the exported file.

## Integrated video player

> Hitachi Visualization Suite provides video management system (VMS)
> capabilities from within the Visualization Suite user interface
> through seamless integration with Hitachi Video Management Software
> (HVMS). The embedded HVMS Base video player controls allow full
> control of video playback.
>
> Depending on your environment, you can use the HVMS Base connector to
> connect Visualization Suite with your HVMS Base instances or the HVMS
> connector to connect with a centralized VMS management system. For
> more information about possible configuration scenarios, see Hitachi
> Video Management Software documentation.

### Video Management Software player features within Visualization Suite

> For full descriptions of each video control feature, see Hitachi Video
> Management Software Base User Guide and Hitachi Video Management
> Software User Guide.

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
<th colspan="2"
style="text-align: center;"><strong>Feature</strong></th>
<th><blockquote>
<p><strong>Preview pane</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Full screen</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Video wall</strong></p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr>
<th>Live view</th>
<td>Supported</td>
<td>Supported</td>
<td>Supported</td>
<td></td>
</tr>
<tr>
<th>View recorded video</th>
<td>N/A</td>
<td>Supported</td>
<td>N/A</td>
<td></td>
</tr>
<tr>
<th>View player statistics <img src="media/image53.png"
style="width:0.14029in;height:0.11589in" /></th>
<td>Supported</td>
<td>Supported</td>
<td>N/A</td>
<td></td>
</tr>
<tr>
<th rowspan="2">Change player mode</th>
<td>High-bandwidth mode <img src="media/image54.png"
style="width:0.12199in;height:0.12199in" /></td>
<td>Supported</td>
<td>Supported</td>
<td>Supported</td>
</tr>
<tr>
<td>Low-bandwidth mode <img src="media/image55.jpeg"
style="width:0.25618in;height:0.12199in" /></td>
<td>Supported</td>
<td>Supported</td>
<td>N/A</td>
</tr>
<tr>
<th>Control a PTZ player <img src="media/image56.png"
style="width:0.11589in;height:0.12199in" /></th>
<td>Supported</td>
<td>Supported</td>
<td>N/A</td>
<td></td>
</tr>
<tr>
<th>Timeline bar</th>
<td>N/A</td>
<td>Supported</td>
<td>N/A</td>
<td></td>
</tr>
<tr>
<th>Basic player controls <img src="media/image57.png"
style="width:0.30497in;height:0.12199in" /></th>
<td>N/A</td>
<td>Supported</td>
<td>N/A</td>
<td></td>
</tr>
<tr>
<th>Playback speed control <img src="media/image58.png"
style="width:0.12199in;height:0.12199in" /></th>
<td>N/A</td>
<td>Supported</td>
<td>N/A</td>
<td></td>
</tr>
<tr>
<th>Playback directions <img src="media/image59.png"
style="width:0.15249in;height:0.12199in" /></th>
<td>N/A</td>
<td>Supported</td>
<td>N/A</td>
<td></td>
</tr>
<tr>
<th>Calendar picker <img src="media/image60.png"
style="width:0.10369in;height:0.10979in" /></th>
<td>N/A</td>
<td>Supported</td>
<td>N/A</td>
<td></td>
</tr>
<tr>
<th>In-cell search <img src="media/image61.png"
style="width:0.12199in;height:0.11589in" /></th>
<td>N/A</td>
<td>N/A</td>
<td>N/A</td>
<td></td>
</tr>
<tr>
<th>Snapshot</th>
<td>Supported</td>
<td>Supported</td>
<td>N/A</td>
<td></td>
</tr>
<tr>
<th>Audio</th>
<td>N/A</td>
<td>N/A</td>
<td>N/A</td>
<td></td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 40%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
</colgroup>
<thead>
<tr>
<th style="text-align: center;"><strong>Feature</strong></th>
<th><blockquote>
<p><strong>Preview pane</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Full screen</strong></p>
</blockquote></th>
<th><blockquote>
<p><strong>Video wall</strong></p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr>
<th>Video export</th>
<td>Supported</td>
<td>Supported</td>
<td>N/A</td>
</tr>
</tbody>
</table>

# Use videowalls

> Using **Videos**, you can configure the videowalls and decide on the
> number of video feeds for monitoring. You can choose the layout and
> pull the available cameras for monitoring the video stream.
>
> Videowalls allow you to monitor up to 64 camera feeds in one view.
> After videowalls are saved, you can toggle between sets of video feeds
> with a click, or monitor several videowalls at a time with multiple
> monitors.

<img src="media/image62.jpeg"
style="width:5.46833in;height:2.76958in" />

> The Video menu consists of the following features:

#### Videowalls

> Lists previously saved videowalls. Select New videowall to add a new
> videowall.

#### Cameras

> List cameras from the search result.
>
> The camera status icons are used to show the online status of VMS and
> IP cameras.

#### New Videowall

> Displays the videowall name. Click the pencil icon to edit the name.

#### Change layout

> Provides the following list of the wall layout options:

- 1 big

- 2 \* 2

- 3 \* 3

- 4 \* 4

- 8 \* 8 (not enabled by default)

- 1 big \| 4 small

- 1 big \| 6 small

- 1 big \| 12 small

- 2 big \| 8 small

- 3 big \| 4 small

> **Note:** The 8 \* 8 layout is optional with special hardware
> requirements.

## Create a videowall

> Perform the following steps to create a new videowall:

#### Procedure

1.  From the top pane, select **Video**.

2.  Click **New videowall**.

<img src="media/image63.png" style="width:5.6in;height:2.56667in" />

3.  Enter a name for the videowall by clicking on the pencil icon next
    to the label **New Videowall** and then click the checkmark to
    confirm the new name.

4.  Change the layout based on your requirement.

5.  Click **Save videowall**.

6.  Add cameras by performing the following steps:

    1.  Click **Cameras** which opens search panel.

    2.  Type text in the search box to search for a camera by name and
        click **Search**.

> The search box must contain at least two letters. If less than two
> letters are typed, the **Search** is not enabled.

3.  Drag and drop the cameras from the camera list result to the
    videowall.

> **Tip:** You can also add cameras to an existing videowall from
> Videowall or [<u>Action buttons (on page 150)</u>](#action-buttons).
>
> **Note:** The camera status is visually identifiable. For example, a
> green dot indicates an active status, which helps you to determine
> which active camera can be used to stream video. For camera status
> information, see [<u>Camera status (on page 169)</u>](#camera-status)

7.  Click **Save videowall**.

# Monitor and manage alerts

> You can examine events reported from a computer aided dispatch system
> (CAD), or "911 calls", license plate readers (LPR), and other
> incidents. If your system is integrated with additional surveillance
> systems, such as Hitachi Live Face Matching and Hitachi Video
> Analytics, events detected by those systems can generate event alerts
> and be displayed on the map in Visualization Suite.

## Overview

> Visualization Suite manages alerts and helps you to stay on top of new
> and important events, such as gunshots, CAD calls, LPR hits, and
> alerts from the Video Analytics software. You can view, acknowledge
> and close alerts within Visualization Suite. Individuals with
> permissions can update the alert status, allowing your team to stay
> informed when the status is updated.
>
> You must have view permission to view event alerts for a specific
> entity type. In addition, your administrator must enable alerts for
> each entity type. For more information, see the Administrator Guide
>
> The following figure is an example map showing alerts within
> Visualization Suite.

<img src="media/image64.jpeg" style="width:5.40333in;height:2.82in" />

1.  Alert icon

> Opens and closes the alert pane. The number on the icon is the sum of
> all alerts and system notifications (updated live).

2.  Alert pane

> The alert pane has two tabs:

- The Event Alerts tab, which displays event alerts.

- The Notifications tab, which displays system messages.

## View alerts and notifications

> The Event Alerts tab displays 100 alerts per page. The number in red
> on the tab is the total number of alerts that are updated live.
>
> Each alert shows two timestamps:

- Occurred at indicates the time the event actually occurred.

- Received at is the time the event was reported to Visualization Suite.
  In addition, the Event Alerts tab allows you to:

- Sort the events by the time the event occurred or the entity type
  (descending or ascending). Changing the sort order resets the page to
  show the first 100 alerts.

- Refresh the alert list to update the alert status.

> **Note:** A search you create in Visualization Suite persists during a
> logon session. Leaving the search window does not cancel or clear the
> search filters. The search will be lost when you log out of
> Visualization Suite.

- Acknowledge alerts (see [<u>Acknowledge alerts (on page
  177)</u>](#acknowledge-alerts)).

- Close alerts (see [<u>Close alerts (on page 178)</u>](#close-alerts)).

- <img src="media/image65.jpeg" style="width:3.99in;height:1.67635in" />View
  the event on the map. Click the Go to button on the alert to view the
  event in an exploded map view. The Go to button is highlighted in the
  given image:

## Acknowledge alerts

> You can acknowledge new alerts generated by Visualization Suite.

#### Procedure

> **1.** To acknowledge alerts, select one or more alerts and click
> **Ack**
> <img src="media/image66.png" style="width:0.35417in;height:0.16667in" />.
> This changes the alert status to acknowledged.

<img src="media/image67.jpeg" style="width:5.27333in;height:3.66in" />

## Close alerts

> You can close and remove the alerts that are not required from the
> alert list.

#### Procedure

> **1.** To close alerts, select one or more alerts and click **Close**.
>
> This changes the alert status to closed and removes that alert from
> the list, reducing the total alert count.
>
> **Note:**

- Closed alerts are removed from the alert database in 30 days.

- Closing alerts does not remove the events from Visualization Suite.
  You can still access the events in the event lists.

## View notifications

> Use the Notifications tab in the alert pane to display system
> messages. System messages are sent to the Visualization Suite client
> interface during every session. Some system messages indicate problems
> with the system while others are purely informational. System messages
> are cleared after each session.

## Monitor alerts

> A notification appears on the alerts icon when there is a system or
> event alert.

- Event Alert examples are when a new gunshot was detected, or a license
  plate of interest was captured by a camera.

- System Alerts include adding a new video management system or camera.

# Analyze dashboards

> **Dashboards** provide graphical representation of historical event
> data and allows you to analyze event statistics.
>
> Based on your access permissions, you can view basic and custom
> dashboards. The basic dashboard lists the available entities and
> associated entity types. Select the entity and entity type for which
> you want visualize the data, gather insights, or create reports.
>
> Hitachi Visualization Suite provides graph reports that visualize data
> integrated from multiple sources in real time. The types of reports
> you see depends on your system. For more information about the types
> of reports, see the Overview of Basic and Custom dashboards section in
> the *Administrator Guide*.
>
> Custom dashboards enable you to create custom reports based on your
> requirements.

## View dashboards

> Use Dashboards to view Event Statistics.

<img src="media/image68.png" style="width:5.6in;height:2.73292in" />

#### Procedure

1.  From the top pane, click **Dashboards**.

2.  Choose the **Events** dashboard. You can view basic event analytics
    reports.

# Use maps and layers

> Map layers can come from various sources. For example, if a server in
> your department manages a subway map layer, you can overlay that layer
> with common maps from the Internet, such as Google<sup>®</sup> maps
> and ESRI layers and Tiled layers. This allows you to personalize your
> maps and include as much information as you want.

<img src="media/image69.png" style="width:5.46833in;height:2.62083in" />

## Add a map

#### Procedure

1.  From the left pane, navigate to **Settings** \> **Maps & layers** .

2.  From the left pane, click the add icon next to **Maps**.

3.  In the **Create Map** page, name the map, enter the URL where the
    map is hosted, and provide a description.

4.  Click **Save**.

## Select a map

#### Procedure

1.  Click **Map**.

2.  From the left pane, expand **Maps and layers** and then expand
    **Map** to view the available maps.

3.  Choose a map.

#### Result

> The selected map is displayed in the map view.

## Add a layer

> You can display layers from different sources on the map, such as
> overlaying basic maps with your internal maps. Your site can layer
> weather, freeway exits, subway stations, population densities, city
> districts, and many other types of map data.

#### Procedure

1.  From the left pane, navigate to **Settings** \> **Maps & layers** .

2.  From the left pane, click the add icon next to **Layers**.

3.  In the **Create Layer** page, select a layer type. The available
    options are:

    - **Tiled layer**: A tiled layer is a set of web-accessible tiles
      that reside on a server. The tiles are accessed by a direct URL
      request from the web browser. Because the tiles in a tile layer
      are not available as a service, they must be in a specific format
      for a web app (such as the map viewer) to display the layer on a
      map.

    - **ESRI layer**: A layer represents geographic data in ArcMap, such
      as a particular theme of data. Examples of map layers include
      streams and lakes, terrain, roads, political boundaries, parcels,
      building footprints, utility lines, and orthophoto imagery. Each
      map layer is used to display and work with a specific GIS dataset.

    - **Upload layer**: KML, Shapefile, Image. The supported image types
      are: png, jpg, jpeg, bmp, and gif.

4.  Enter **Name** and **Description** of the selected layer.

5.  If you choose **Tiled layer** or **ESRI layer**, complete the
    following fields:

<!-- -->

1.  Enter the **URL** details to pick the layer.

2.  Enter **Default fields**. The default fields are optional and must
    be separated by semicolon. Each geographical shape such as point,
    area or line contained into a shape file might not embed a series of
    data fields. Specify one or more field names such as **Name**,
    **Description** to see the value when clicking on the shape inside
    Visualization Suite.

<!-- -->

6.  If you choose **Upload layer**, complete the following fields:

<!-- -->

1.  Select the layer **Type**. The available layer types are:

    - **KML**: Keyhole Markup Language (KML) is an XML notation for
      expressing geographic annotation and visualization within
      Internet-based, two-dimensional maps and three-dimensional Earth
      browsers. KML was developed for use with Google Earth, which was
      originally named Keyhole Earth Viewer.

    - **Shapefile**: Zip files that contains shape files. A shapefile is
      a simple, nontopological format for storing the geometric location
      and attribute information of geographic features. Geographic
      features in a shapefile can be represented by points, lines, or
      polygons (areas).

    - **Image**: Image file. The supported image types are: png, jpg,
      jpeg, bmp, and gif.

2.  Enter **Default fields**.

3.  Upload the layer.

<!-- -->

7.  Click **Save**.

## Select a layer

#### Procedure

1.  Go to **Map**.

2.  From the left pane, expand **Maps and layers** and then expand
    **Layer** to view the available layers.

3.  Select one or more layers to display on the map.

#### Next steps

- Select or clear the Layer option to toggle between the default layer.

- Clear the Layer check box to clear the layer selection.

# View user profile and preference

> You can set your preferred user settings.
>
> Click the **User** icon to set your preferred currency, distance type,
> language, speed, temperature, and view your user settings.

## User profile

> You can view the user profile such as your group in the Visualization
> Suite. You cannot edit these settings.

#### Procedure

> **1.** Click the **User** icon on the upper right corner. The user
> dialog box appears:
>
> <img src="media/image70.png" style="width:3.185in;height:5.26094in" />

## User preferences

> The user interface of the Hitachi Visualization Suite is available in
> several languages.
>
> To change the language, click User and select the Configuration tab.
> If the interface is in a language you do not understand and are trying
> to change the settings, see the following image:
>
> <img src="media/image71.png" style="width:2.99208in;height:4.80167in" />

# Access help

> Click the **Help and Documentation** icon to access the Visualization
> Suite documentation.

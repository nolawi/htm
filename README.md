# Caseflow Team Updates

## Appeals PM Update for August 1, 2017

### Work Currently in Progress
**Implementation Plans**:  We have been executing the Implementation Plans for following projects:

> ## Certification – v2
> 
> 1.   Requested and obtained the enabling of V2 feature flag for Southeast District ROs. 
> 2.   We have sent out rollout announcement emails to each District and requested a list of users who will need to attend the training.  As  the names are coming back in, we are also checking to see who currently doesn’t have access.  If the RO has users without access, an email notification of users without access along with the Certification User Access Guidance is sent so that they can request access if necessary.
> 
> 3.  Requested and obtained the enabling of V2 feature flag for Southeast District ROs. 
> 4.   Training:  Invites to attend the upcoming training session have been sent to all users of the Southeast District.  These invites included the following training materials:  FAQ, Training Guide, and Quick Reference Guide.
 
> ## Reader
> 1. Created Reader User Access Guidance document.  
> 2. Initiated and obtained access for the users that will be participating in the Beta Pilot.
> 3.  Training:  Completed training materials - Instructor-Led-Training and FAQs.  An engineering story has been created to update the Help page FAQs.
> 4.Training:  Conducted training for the Beta Pilot users.
 
> ## eFolder Express – VVA
> 1.  Requested the VVA feature flag enabled for the BVA pilot users.  This will be continuing for the remainder of the week as the team wants to observe how the coach marks are received.  Additionally, we want to monitor VVA’s load balance with these additional users pulling the documents.
> 2.  Training:  Continuing to work on remainder of training materials (Training Guide and Quick Reference Guide (QRG)).
> 3.  Training:  Completed training materials: - FAQs.  An engineering story has been created to update the Help page FAQs.  
 
> ## Hearing Prep
>1.  We have requested the new function “Hearing Prep” to be added to Caseflow’s list of functions in CSEM.  This function is now available and ready for us to test.
 
**Security Controls Assessment**: We are continuing to respond to the identified issues.  Currently, we have created control documents for each issue.  
 
**System User Access Process**: We are working towards changing the current process for how users gain access to Caseflow.  Our first step was to provide guidance to all necessary parties on the proper options to select when requesting access.  Our next step is to gain access to all stations within the CSEM application allowing us to control who gets access as well as approving access.  We currently have achieved access to our station (101).  We are seeking approval to gain access the other stations.  
 
### Impact on Caseflow Products
- **User Access Guides**: Created individual product User Access Guidance documents that provide instructions on how to request user access to that product.  This guide is available to be given to supervisors who may need to request access for their team.  Additionally, a Caseflow User Access Guidance was created to be used by CSEM Initiators and ISOs. This guidance has instructions for all Caseflow Products. The Caseflow User Access guidance has been given to National ISOs and published on OBPI’s site.
 
- **TMS**: We are exploring the process for uploading training materials to TMS.  This material can be PowerPoint, PDF, or video presentations.  
 
### Concerns
**System Admin Permissions**:  We currently still have a few stragglers with System Admin permissions.  We are escalating these people.

## Whiskey Update for August 1, 2017

### Work currently in progress
In addition to a handful of UI enhancements, the Whiskey team is wrapping up a few new features leading up to the beta release of Reader on 8/2:
- **Welcome Gate**: We held feedback sessions with current Reader users and learned that attorneys and judges would like to see cases checked in to their station (rather than DAS case assignments) as a more relevant reflection of their "to do" list. We also added a column to show users all the issues on appeal for each checked in case. We released and tested an updated landing page last sprint, and are working toward displaying CAVC/AOD status on this page as well.
- **Claims folder details**: In addition to the Welcome Gate, we're now showing the issues on appeal (from VACOLS) in a "Claims Folder Details" section on the documents list page, as well as in the annotations menu.
- **eFolder Express integration**: We're ALMOST ready to use the eFolder Express API to retrieve documents from VBMS! This update will pave the way to pre-fetch all of the documents in an attorney's assigned cases – reducing the time it takes to load a claims folder and our reliance on VBMS uptime (read: downtime) overall.

### Collaboration with other Caseflow tools
- Our research sessions last sprint led us to consider if/how we might further enhance the Welcome Gate. In particular, attorneys would like to see due dates for their assigned cases, and VLJs are interested in knowing the date a case was "charged" to their station in VACOLS. In general, distinguishing between user roles may become more useful as VLJs begin using Reader to prepare for hearings.
- As we refine and develop the "Claims folder details", we should continue to collaborate with the Hearing Prep team to identify gaps and/or inconsistencies in existing information and layout.
- The Welcome Gate may serve as a bridge between Reader and a more robust attorney/judge work queue in the future.
- Virtual VA rollout (in an eFolder Express integrated world, we should decide if/when we want to "turn on" VVA for some or all users).

### Concerns
- eFolder Express integration has been trickier than we anticipated. We're still relying on Certification to retrieve documents and using a feature flag until development work is complete. After we've flipped the flag, we should keep an eye on it to make sure everything is working as expected. Pending some outstanding engineering work/investigation, we may have to either a) decide to increase our load on Certification as our backend or b) delay our official launch date for all ~50 users by a few days (the kickoff will go on regardless). We'll make a decision by EOD Tuesday. [_editor's note: the beta launch has been pushed to Wednesday, August 9, 2017._]


## Tango Update for August 1, 2017

### Work currently in progress:
Team Tango is working toward the pilot of Hearing Prep starting end of August, a few more Dispatch tickets to resolve some Sentry errors, and the rollout of eFolder Express + VVA.
- **Hearing Prep Daily Docket**: We're finishing up both the frontend and backend of the Daily Docket page by adding save functionality and the ability to update hearing dispositions in VACOLS.
- **Hearing Prep UI Changes**: We are making a few small UI changes to ensure the product matches its designs and is ready for pilot users, including adding a button for users to access Reader at the bottom of Hearing Worksheet, making sure the saving header is consistent, and making sure users are scrolled to the top of each page upon navigation.
- **Hearing Scheduling Research**: We plan to meet with Scott and Hearing branch coordinators this sprint to better understand the process of scheduling video, CO and travel board hearings from the BVA perspective. This will also help us craft a Hearing Scheduling Pilot calendar.
- **Dispatch: Responding to Sentry Errors**: We are working on some Dispatch tickets to resolve repeated Sentry errors, including the ability to route an EP to RO70, which was not previously in our list of ROs. We also identified that Appeals Status API was generating appeals without a VBMS-ID and are working on a fix.
- **eFolder Express + VVA Rollout**: We are conducting usability sessions on VVA coach marks and turning on eFolder Express + VVA access for BVA FOIA, and OGC users this sprint in accordance with a slow rollout schedule.

### Collaboration with other Caseflow tools:
- **Case Summary**: We are adding a new "Case Summary" category to Reader that will automatically be applied to documents judges review when preparing for a hearing. Reader will be pre-filtered to this category when the user navigates to it from the Hearing Worksheet. These documents were selected after interviews with judges. Tango and Whiskey will continue to collaborate on the layout of the "Claims folder details" from Reader and top portion of the Hearing Worksheet because Hearing Prep users will navigate from the Hearing Worksheet into the Veteran's eFolder.
- **User Permissions**: We are granting Hearing Prep users access to the Reader CSEM function so they can navigate from Hearing Prep to view the Veteran's eFolder.

### Concerns:
We are planning for Hearing Prep pilot training with judges on Thursday, August 24. We will monitor progress on the tickets this week and during Hearings Advance Team Sync on Monday, August 7, evaluate if that training needs to be pushed later.


## Foxtrot Update for August 1, 2017

### Work currently in progress:
Team Foxtrot is finishing up bugs and small improvements that came out of the St Pete pilot, rolling out V2 remotely to each district of ROs, and working with the intake team to measure V2's success.
- **Loading spinner**: Nemo and Alex are finishing up a spinner that appears when V2 is initially loading. If VBMS is taking longer than usual to respond, the spinner displays an additional message. If the process times out, V2 shows a generic error message. https://github.com/department-of-veterans-affairs/caseflow/issues/2666
- **Removing POA address copy from Confirm Case Details page**: During pilots at 3 different ROs, we learned that updating the representative's address in VACOLS is not part of VSR and DRO workflows. We are no longer asking them to manually update VACOLS, as it is not currently a priority for POA addresses to be up to date in VACOLS for the flag flip step of BVA intake. In a future update to V2, we'll prioritize adding POA and Veteran address fields, so that RO staff will not need to update it manually in VACOLS. https://github.com/department-of-veterans-affairs/caseflow/issues/2739
- **Multiple Form 9s**: A small but significant percentage of eFolders contain Form 9s with the same date. This feature displays Form 9s with the same date with tabs, so that RO staff can review all of them and use the correct Form 9 to answer V2's hearing preference question. https://github.com/department-of-veterans-affairs/caseflow/issues/2673
- **Sample of V2-certified cases**: We sent a sample of 50 V2-certified cases (from the 3 pilot ROs) to Ivy at BVA intake. She reviewed them and noted errors that would prevent her from flipping the flag. She identified a handful of POA inconsistencies that we will follow up about in person, when she's back from vacation the week of 8/7.

Phillip, Lauren, and Shelly are 1 sprint into work queue discovery. By the week of 8/14, we plan to share initial findings about pain points, workflows, systems, and process changes. So far, we've:
- **Interviewed the Lit Support team (Brianne and Theo)**: uncovered extensive and imminent plans to remove brief faces and reduce the number of VACOLS locations that an appeal can be charged to. These are changes that might happen at the end of August or the start of October. They sound like a step in the right direction for managing and tracking appeals at the Board!
- **Interviewed Jed**: he is a champ and helped us understand ~60 VACOLS locations – what they were, if they were currently used, and who to ask to learn more.
- **Interviewed Eugene from co-located support**: learned about admin workflows and pain points.
- We're currently assembling findings and a plan for the next set of interviews.

### Collaboration with other Caseflow tools:
- Spinner code and generic error page copy can be used by other tools for loading pages and error messages.
- RO pilots highlighted how helpful Reader could be to RO staff. Once Reader works well at BVA, it would be great to discuss Reader beyond BVA.

### Concerns
- We're interviewing BVA staff before upcoming brief face and VACOLS process changes, to understand their current pain points and overall workflows. We think that workflows will change after brief faces go away, and are planning to interview key teams after the change. If the change is delayed until the start of October, we may need to delay the last piece of Work Queue discovery accordingly. We'll know more as the weeks pass, just raising this flag early.

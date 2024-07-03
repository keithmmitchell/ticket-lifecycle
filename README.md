<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to create, work, and resolves tickets within osTicket](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Lifecycle Stages</h2>

In this lab we are going to create some tickets and resolve them.

In the Edge browser go to localhost/osticket/ and click Open A New Ticket.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/2ee2129d-2ad0-489f-bb76-a609321518c8)

Enter the following:

- Email Address: karen@osticket.com 
- Name: Karen Karen
- Topic: Business Critical Outage
- Issue Summary: Entire Mobile Online Banking Is Down. Customers are reporting they are getting a 404 error when browsing to online banking.

Then click Create Ticket

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/726d4474-4c78-43d2-9f3c-f6a68ee90b94)

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/a9207ad1-a284-4ef4-ae90-671a8d0353d7)

Create another ticket with the following:

- Email Address: ken@osticket.com 
- Name: Ken Ken
- Topic: Personal Computer Issues
- Issue Summary: Entire Accounts Dept. Adobe Reader Not Working. Ever since the upgrade last night, nobody in Accounting has been able to use Adobe Reader.

Email Address: karen@osticket.com 
- Name: Karen Karen
- Topic: General Enquiry
- Issue Summary: When are we getting a hardware refresh? Most of my department is having issues with their current tablets, we need this ASAP.  Please provide info.

<br />

Next we need to log in as an agent to resolve the tickets so go to http://localhost/osTicket/scp/login.php and log in with the username jane.doe with the password Password1.  

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/4bd3cbcd-65c4-4f6c-8dbc-19fe1263772c)

We can now see a list of open tickets.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/f1f7d473-3707-495b-9559-7dd3f088600c)

Click on entire mobile banking is down to view it.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/5a990140-89d0-4ed8-8ac0-bca85844cd54)

You can see the priority is normal.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/d65f0d27-c0f0-4daf-b0d6-d5aee8930215)

Click on this to change it to Emergency and enter the note "Business impacting event" and click Update.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/f10a33ed-1c8c-47ef-8fef-f267ff017766)

The ticket is currently unassigned.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/36bc337d-7f48-4d28-a8ed-a99313f9cae2)

Click on it, assign to jane doe and click Assign.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/604b6fc6-62d5-4040-bdf9-fc45d47ab111)

The default SLA isn't appropriate for an emergency so click on it and change it to SEV-A. Add the note "Business impacting, critical incident." Click Update.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/a5264cd2-44b1-4ed8-b3c1-a5513eea727b)

The department is currently set to Support.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/51e7aba5-af05-44e8-9a75-329fc32688e9)

Click on it and change it to System Administrators and enter the note "Sys Admins responsible for mobile banking infrastructure." then click Transfer.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/a3b191f2-215a-4245-a587-c27f4fb691b4)

Post a reply "Coordinating with Sys Admin team to bring mobile banking back online." then click Post Reply.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/3109bea2-888f-4d45-9847-b8ba94764df5)

We can now see the ticket has been updated in the list of tickets.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/742defb0-ff24-4543-9540-022f75248eb7)

We can now go back into the ticket and enter "Jerry from Systems Engineering found and corrected a failed load balancer. Mobile banking should be back up."  Change the status to Resolved and click Post Reply.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/6a0e0394-1a95-42f6-af09-f70c0267999e)

We can now see the ticket has disappeared.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/7a33852e-9274-42ab-be99-a85bab0e187b)

Clicking on closed lets us see it there.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/20db65f8-39b8-48c0-8c7d-6c38b04122e3)

Select the Entire Accounts Dept. Adobe Reader Not Working ticket.  Change Priority to High.  

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/0fa14ead-4c36-41cc-9dd1-06d0262be665)

Update the SLA Plan to SEV-B.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/b097008d-22b8-4bfb-abbb-5cea9c77a22d)

Assign the ticket to John Doe.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/77d24ea2-4652-401b-86fc-8c977c174956)

Enter a reply "Re-assigned to SEV-B, reached out to John for a warm hand." and click Post Reply.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/d49de5da-4187-48e8-aafc-f2508d9ab794)

We can now see the changes made in the list of tickets.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/e77649f4-6102-4303-95b1-8479e2fd46d7)

Click on When Are We Getting A New Hardware Refresh ticket.

<br />

Change the Priority to Low and click Update.

<br >

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/022b7310-6fe5-4b85-912f-32c87bc78243)

Assign the ticket to Jane.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/86173c72-a72d-4ae5-81fa-c4c28d6c3488)

Change the SLA to SEV-C.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/d3d56f01-3e04-4180-a4e7-5e5925ae980f)

Post hte reply "Hardware refresh is slated for Q1.  If you like, you and your dept can start testing the new units today. Just send me an email." then mark the ticket as resolved.

<br />

![image](https://github.com/keithmmitchell/ticket-lifecycle/assets/174253055/145a4999-00f2-4f17-840e-60e067dc68cc)

We can now see the ticket is not in the list of open tickets.

<br />

There's one ticket left which is assigned to John so to resolve it we need to sign out as Jane and sign back in as John.

<br />






















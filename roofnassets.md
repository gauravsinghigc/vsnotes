# roofnassets

@24_11_2022

_*Previous Changes*_

1. Done => Name and number search option for everyone so that a user need not to check each number.
2. Done => Lead person's name Filter is not working. It should search the data irrespective of the date.
3. Done => Font of feedback to be highlighted at multiple locations.
4. Done => Ringing numbers to be displayed separate from follow ups.
5. Done => Ringing to be displayed separate on dashboard.
6. Done => BH name to be mentioned when BH transfers the leads to its team member.
7. Done => While transferring the leads, create an option to select multiple leads with just one click with "a slot of 10, 25, 50, 100" leads at a time.
8. Done => When a BH or TH transfers leads from his account, He/she is not able to select the leads. Instead all of the Bh or TH account leads get transferred to one person particularly. Display an option to select the leads so that BH or TH can transfer the leads to multiple users.
9. Done => If there is no team member under any user, Please deactivate the transfer option.
10. Done => Display the project name with every lead. _(*Need to be update project name with linked with leads*)_
11. Done => Display Fresh Leads count under "My Team" tab.
12. Done => BH or TH should be able to transfer the leads to their respective team members only. Other team members should not be displayed to them.
13. Already Provided => Provide an option to edit the feedback, If a user wants to edit the feedback. _(*Feedback edit option result in un organised leads folloups record, for wrong or in correct feedback, there is also a option for new feedback, that helps in tracking every feedback correctly*)_

_*New Modules*_

1. HR Module is completed
2. digital module and login is completed

_*Note*_ :

1. new module will be affact some section of application, so it will provided after proper testing and setup by our end
2. Previous changes are lived please check one by one.
3. changes are live at http://core.roofnassets.com/

---

## New changes @ 24-11-2022

_*HR-MODULE-UPDATES*_

1. HR module is completed
2. hr can created, edit, remove, users
3. hr can see today or future birthday-msg
4. hr can make attadance for all users ab-b-l
5. hr now can manage user documents,
6. hr now can manage user salary records
7. hr now can active or inactive any user in the crm

## 26-NOV-2022

1. Lead transferre between users now enhanced with pagination and search senstivity that help to get actual data after appliying filters.

## 29-NOV-2022

1. Group wise team display. (BH->TH->SM)
2. For BH and TH, today's followps for of respective SM.

## 30-NOV-2022

1. Receptions Module for walkins
2. Pagination & Search for person name for lead transfer
3. Project Name at Uploaded leads
4. Fresh leads count not working in team
5. next page view for leads not showing action from main dashboard
6. transferred highlights
7. today count in some users
8. lead transfer notifications pop-up

## 13-DEC-2022

Android App is updated now, updates contain.

1. calling button is working now
2. mail button is working
3. whatsapp direct chat is working now
4. share on whatsapp is working now
5. share to other app is also added

Note : we have release the updates to play store, they are under review, app update option will available after review...which take 3-4 hr for play store to verify the changes

## 15-dec-2022

1. Pagination & Search for person name for lead transfer
2. Project Name at Uploaded leads
3. Fresh leads count not working in team
4. next page view for leads not showing action from main dashboard
5. transferred highlights
6. today count in some users
7. Digital account login

## 16-dec-2022

=> Live Changes

1. User list under [All-Users] and [All-Team] is enhanced for desktop view.
2. Under Team List Today follow up count is also added!
3. Digital profile is developed and can be access via appointing/converting an user into Digital via primary info update in user details page.
4. Digital can move leads from one user to other with full access.
5. digital can move leads via search option by entring lead person name than select and transfer.
6. digital can upload bulk leads and transfer to any user
7. In header login person Usertype is now visible

=> Under development & backend is completed

8. HR new provided documents
   8.1 backend is developed for leave Application.s
   8.2 backend for Assets Modules that includes.
   {
   -> Assets Lists.
   -> Assets categories.
   }
   8.3 backend for On Duty passes is developed

## 14-FEB-2023

=> CRM CHANGES

1. REG0## is now auto created during new registrations.
2. Registration/Booking Header is changed as per requirements
3. Payment Status is percentage is displayed in booking listing.
4. Booking Day counter is added and if days count exceed limit of 30days then bg color will be changed to warning(yellowise+organe).
5. member list in booking/registration is enhanced for desktop view
6. unit cost calculation as per unit rate is added during registration process.
7. send notification and alert to customer is added via CRM::Customer->Dashboard->Send Notification button.

=> HR Updates

1. HR Database is designing is completed.
2. working on CRUD operation for HR Module

## 16 Feb 2023

1. Plc yes or no {
   => Yes ke case main 1 to 10 percentage aa jaye
   => Or no hai to receipt main no ka status dikh jaaye
   => Or yes hai to uska amount dikh jaaye
   }

#CIF-FORM {
=> CIF Form is now dynamically generated!
=> Nominee details are also auto picked if have during booking process
=> document auto picked and attached if uploaded
=> team data and id auto picked and attached
=> document auto attached in the cif end section
=> required signature section with name also created dynamically
}

Edit Registration {
=> ROOT://All Customers -> Click On Customer Name -> Registration Tab -> View Details for Require Registration
=> Regsitration Pop-up form will be displayed for update
=> update and save record
}

EDIT REFUND {
=> ROOT://All Customers -> Click On Customer Name -> Refund Tab -> View Details for Require Refunds
=> Registration and refund details will be saved
=> update and save record
}

# 23-FEB-2023

CRM {
=> Pay Status is now compulsory and by default pending/issued is selected
=> net paid amount is correct
}

HR @ OD Request {
=> OD Request module is completed excluding filters/reports
=> Now All user send OD Requests to HR and Reporting Manager
=> HR and Reporting Manager can approve or reject OD requests
=> HR, USER and Reporting Manager can update OD details before and after approval.
=> User can update OD details before approval after approval they can't update details.
=> Sent, Approved, rejected, Active, and completed OD status be will automatically updated as per requesting date and details will be mail to user automatically or user primary email id.
=> OD is automatically update from approved to active and active to completed.
=> Reporting manager also view their team ods and for this view Team ods option will be displayed in reporting manager ods dashboard.
}

# 24-feb-2023

CRM @ {
=> Customer having Name Santosh (tel: ['9416427162', '9416427182']) is removed with all relational data.
=> Booking for customer named as JAGMINDER SINGH having ACKCODE : BK001 is removed with all relational data.
=> after booking update bug is solved
=> Ack from registration is copied to booking ack code during registration to booking creation
=> Registration amount in now added into cif form
}

# 28-FEB-2023

HR @ CIRCULARS {
=> Circular creation is completed
=> admin and HR can create circulars
=> circulars can aslo be mail to all user on email as well as in crm
=> user have to mark as read in case of view
=> user only view circulars
=> admin or hr both update circulars and sent details on mail also
}

Registrations @ {
=> OLD Customers {
:- Go to Home->All Customers->Search Customer (enter customer name) + Enter
:- search data will be shown
:- click on customer name and open customer dashboard
:- Click on New Registration
}
}

# 30-march-2023 {

updates @ {

- Birthday Pop-Up issue is solved and now its working!
- Reminder pop-up issued is solved and now its working!
- Customer Update option during registration update like active is now available.
- no dashboard change during sidebar/access change issue is resolved
- speed is option upto 1.9sec on first load! you can check this at https://pagespeed.web.dev/analysis/https-roofnassets-com/3pqo3utny8?form_factor=desktop
- visitor status update options are updated ['Selected', 'Rejected','Please Wait', 'Approved']
- visitor duplicacy is resolved
- User Work location issue during registration/create is resolved!
- circular read/view count order is changed as #counts/#AllUsers.
- user filter active/inactive issue is resolved!
- circular send on mails is enabled!
- File Upload option added in circulars
- Rewards, PIPs, Appraisals, Circulars mark as read/view attachment option is added!
- counter in ridesidebar is added for circulrs, rewards, pips, and appraisals

}

}

# 07-April-2023 {

HR Updates are live @ [
-> Birthday pop-up and fixed birthday view
-> Employee ID auto increament issue also solved
-> OD and Leave count in sidebar is added
-> OD pop-up for Business head is added and fast approval/rejection of od request
-> Leave pop-up for HR is added for fast view, update and approve/reject leave requests
-> leave default view is current month and then filter is added with status
-> od filter for status is added
-> OD is approved by which member is added and solve for wrong approvals
-> all rewards of other users is also shown in myrewards section
-> my leave option for hr is added
]
}

# 02-May-2023 {

@Digital [
-> Multiselect during lead move from one to other
-> bug during lead export
-> total at bottom of team leads
-> create for in campaign export

@CRM {
done -> dashboard counter display clicked data with birthday of customers count
-> unit size, total price, total units in export export for bookings
-> report paid amount not including regi amount
-> summary of exports
}

@HR {
-> Full Reporting Left
}
]
}

-> total leads => distributed
-> digital campaign
-> created for filters in digital and news papers
-> news paper campaign
-> 
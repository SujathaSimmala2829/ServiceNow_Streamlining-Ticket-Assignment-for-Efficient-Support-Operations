🎫 Streamlining Ticket Assignment for Efficient Support Operations
This project showcases the implementation of an automated ticket routing system in ServiceNow for ABC Corporation. The primary goal is to enhance support efficiency by automatically assigning incoming support tickets to the appropriate teams based on the issue type—eliminating manual intervention and reducing resolution time.

📌 Objective
To automate ticket routing and:

✅ Minimize resolution delays

✅ Increase customer satisfaction

✅ Optimize support team resource utilization

🛠️ Features Implemented
👤 User & Group Management
Users: Two support users created using the System Security module.

Groups:

Certificate Group

Platform Group

🔐 Role Management
Roles defined and associated with each group for proper permission control.

🗃️ Custom Table – Operations Table
A dedicated table created to manage support tickets.

Contains predefined issue types:

Unable to login to platform

404 error

Regarding certificates

Regarding user expired

🧑‍💼 Role Assignments
Users assigned appropriate roles and added to either the Platform or Certificate group based on their function.

🛡️ Application Access Configuration
Read/Write permissions enabled based on assigned roles for secure access to the Operations table.

🔐 Access Control List (ACL)
Custom ACLs created to secure access to four key fields.

Admin-level rules defined for controlled access.

🔄 Flow Designer – Ticket Automation
⚙️ Flow 1: Certificate Issues
Automatically routes tickets with the issue "Regarding certificates" to the Certificate Group.

⚙️ Flow 2: Platform Issues
Routes the following to the Platform Group:

Unable to login to platform

404 error

Regarding user expired

🧩 Technology Stack
Component	Description
Platform	ServiceNow
Modules Used	User Management, Role & Group Management, Table & Form Design, Flow Designer, ACL Configuration

🧪 How to Test
Create a new record in the Operations table.

Select an issue type from the dropdown.

Save the record.

Confirm that the record is automatically routed to the correct support group via Flow Designer.

✅ Conclusion
The automated ticket routing system greatly reduced manual work, streamlined operations, and ensured timely resolution of support tickets.
Leveraging ServiceNow’s powerful tools like Flow Designer and ACLs, this project successfully demonstrated a rule-based and efficient ticket management solution.

🔗 Demo Video: https://drive.google.com/file/d/1yuNCH4EUO3thLfLmsmfdJgJ2ON3FLHCj/view 

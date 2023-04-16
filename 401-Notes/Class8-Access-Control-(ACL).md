# Access Control (ACL)

## 5 steps to RBAC

What is Role Based Access Control (RBAC) and why do we care?

RBAC is the idea of assigning system access to users based on their role within an organization. The system needs of a given workforce are analyzed, with users grouped into roles based on common job responsibilities and system access needs. Access is then assigned to each person based strictly on their role assignment. With tight adherence to access requirements established for each role, access management becomes much easier.

The question therefore is why, with an achievable and time-honored approach, we can’t seem to get a handle on access control. We are certainly being pushed in that direction of RBAC, with all of the major standards, including PCI DSS, HIPAA and Gramm-Leach-Bliley all requiring some form of it.

Describe a Role/Permission heirarchy that you might implement using RBAC.

Access control lists (ACL) — An ACL is a means of defining access rights by a given user or user group, to a specific object, such as a document.  As a simple example, an ACL could be used to allow users from one department to make changes to a document, while only allowing users from other departments to read the document.

Attribute-based access control (ABAC) — ABAC, sometimes known as policy-based access control, can use a variety of attributes, including user department, time of day, location of access, type of access required, etc. to determine whether a user’s access request should be granted.

Both of these options provide additional granularity of controls beyond the basic concept of RBAC, but can also greatly expand the effort required to create and maintain the necessary permissions.  RBAC arguably offers a more simplified and manageable approach, given that the privileges of a user in a given position are granted with a simple effort, to all others in the same role.  These methods can, however, be used in tandem to increase control.

What approach might you take to implement RBAC?

The users only get the specific access they are granted according to their role.

## wiki - RBAC

If Authentication is “you are who you say you are,” what is Authorization?

Role authorization: A subject's active role must be authorized for the subject. With rule 1 above, this rule ensures that users can take on only roles for which they are authorized.
Permission authorization: A subject can exercise a permission only if the permission is authorized for the subject's active role. With rules 1 and 2, this rule ensures that users can exercise only permissions for which they are authorized.

Name three primary rules defined for RBAC.

- Role assignment: A subject can exercise a permission only if the subject has selected or been assigned a role.
- Role authorization: A subject's active role must be authorized for the subject. With rule 1 above, this rule ensures that users can take on only roles for which they are authorized.
- Permission authorization: A subject can exercise a permission only if the permission is authorized for the subject's active role. With rules 1 and 2, this rule ensures that users can exercise only permissions for which they are authorized.

Describe RBAC to a non-technical friend.

Role based access allows you to decide which users have access to certain informationa and permissions based on their role.

## RBAC tutorial

What Are access rights Associated with? The User? or The Role? Explain.

Access right are associated to the users role when they're added to the database.

Access Rights, or Authorization, is activated after a user successfully does what?

In role-based access control (RBAC), access rights or authorization are activated after a user has successfully authenticated themselves. This means that the user has provided valid credentials such as a username and password, and the system has verified that the credentials are correct.

Once the user has been authenticated, the system can then assign them one or more roles based on their job responsibilities or other factors. Each role is associated with a set of permissions or access rights that define what the user is allowed to do within the system. These permissions might include reading or writing data, creating or modifying records, or executing specific functions or tasks.

When the user attempts to access a resource or perform an action within the system, the RBAC system checks their assigned role and associated permissions to determine whether they are authorized to perform the requested action. If the user's role does not include the necessary permissions, the system will deny the request and prevent the user from performing the action.

Explain how RBAC might benefit a business.

Role base access allows businesses to keep their employees from accessing information on a need to know basis and or role basis. A normal worker will not have the same access as a manager has.

[link-to-reading-notes](https://www.csoonline.com/article/3060780/security/5-steps-to-simple-role-based-access-control.html).
[link-to-reading-notes](https://en.wikipedia.org/wiki/Role-based_access_control).
[link-to-reading-notes](https://www.youtube.com/watch?v=C4NP8Eon3cA).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?
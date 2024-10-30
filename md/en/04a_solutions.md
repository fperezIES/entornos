# Software analysis and design

## Requirements specification - Exercise solutions


> **Exercise 1:** 
> 
> Determine if the following statements are true or false, and why:

> *Solution*:

> * Interviews are generally the most effective method for gathering information for a software project.

We can say both FALSE (because it depends on the project itself) or TRUE (because it is the most complete way of getting the user needs for some projects).

> * JAD is a quick method for specifying requirements in projects involving multiple departments.

As with previous assertion, we can both say TRUE (because it is a suitable method when more than one department from the customer company is involved in the project) and FALSE (because it is not quick, meetings may last some days).

> * Questionnaires are useful when gathering information from customers who are geographically distant.

TRUE

> * Observation and documentation alone can produce a highly accurate SRS.

FALSE. If we don't get any information from people working on the company, we can barely get useful and complete requirements.

> **Exercise 2:** 
> 
Read the following scenario and identify the system, functional, and non-functional requirements:
> 
> *A blog has three types of users: administrators, editors, and visitors. All users must log in to access the application. Administrators can register other users, editors can publish posts, and visitors can comment on them. The website is expected to handle a large volume of daily traffic, so high availability is crucial. Several servers will be used to balance the load and distribute client access. Since the editors are inexperienced, the user interface must be simple. All posts and comments will be stored in a MySQL database with daily backups, and passwords will be encrypted to prevent security breaches.*

> *Solution*:

<table>
<tr>
    <th>System req.</th>
    <th>Functional req.</th>
    <th>Non-functional req.</th>
</tr>
<tr>
    <td>
        <ul>
            <li>Several servers with load balance</li>
            <li>Internet connection</li>
            <li>MySQL database</li>
        </ul>
    </td>
    <td>
        <ul>
            <li>Three user roles (admins, editors and visitors)</li>
            <li>Admins can register other users</li>
            <li>Editors can publish posts</li>
            <li>Visitors can comment posts</li>
            <li>User login</li>
            <li>Store every post and comment in the database</li>
        </ul>
    </td>
    <td>
        <ul>
            <li>High availability</li>
            <li>Ease of use</li>
            <li>Make daily backups of the database</li>
            <li>Passwords must be encrypted</li>            
        </ul>
    </td>
</table>

> **Exercise 3:** 
> 
> For the following software proposal, identify the system, functional, and non-functional requirements:
> 
> *A cultural organization manages loans of two types of items: music discs and books. The application should allow users to add new items of both types. Users must log in with a username and password, and they can search for items by type (disc/book) or by title. Users can request items that are not currently available, with a limit of 5 items on loan simultaneously. Since the organization is located in a small town, user activity is expected to be low, so only one computer and a small database are needed. If a user forgets their password, the system will email it to the registered email address.*

> *Solution*:

<table>
<tr>
    <th>System req.</th>
    <th>Functional req.</th>
    <th>Non-functional req.</th>
</tr>
<tr>
    <td>
        <ul>
            <li>A single computer is enough</li>
            <li>A small database</li>
        </ul>
    </td>
    <td>
        <ul>
            <li>Users must log in</li>
            <li>Users must be able to recover their password by email</li>
            <li>Add new books and disks to the collection</li>
            <li>Search objects by type and/or by title</li>
            <li>Check object availability</li>
            <li>Allow up to 5 objects per user simultaneously</li>
        </ul>
    </td>
    <td>
        <ul>
            <li>We could encrypt the passwords to increase the security of the system. In this case, password should not be recovered, but renewed instead.</li>
            <li>System should be easy to use (it is not specified in the requirements, but as it is going to be used by many different people, it could be necessary).</li>
        </ul>
    </td>
</table>

> **Exercise 4:** 
> 
> Classify the following requirements into system requirements, functional requirements or non functional requirements:

> *Solution*:

> * The application must save the data before closing

FUNCTIONAL

> * The database server must be hosted on a separate computer.

SYSTEM

> * If the connection to the remote server is lost, the application should display an error message and close.

FUNCTIONAL

> * Response time must not exceed 10 milliseconds.

NON-FUNCTIONAL

> * Sufficient bandwidth is required for real-time video streaming.

SYSTEM (internet connection) and NON-FUNCTIONAL (enough bandwidth)

> * The system must verify the user's entered name, ID, and phone number.

FUNCTIONAL

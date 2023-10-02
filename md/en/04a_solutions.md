# Software analysis and design

## Requirements specification - Exercise solutions


> **Exercise 1:** 
> 
> Determine if the following statements are true or false, and why:

> *Solution*:

> * Interviews are the most suitable way of getting information for a software project, in general

We can say both FALSE (because it depends on the project itself) or TRUE (because it is the most complete way of getting the user needs for some projects).

> * JAD is a quick way of specifying the requirements of an application in projects where several departments of the customer company are involved

As with previous assertion, we can both say TRUE (because it is a suitable method when more than one department from the customer company is involved in the project) and FALSE (because it is not quick, meetings may last some days).

> * Questionnaires are useful when we try to gather information from the customer and the components are far from each other geographically

TRUE

> * Only with the observation of the company or the study of its documentation we can get a SRS very accurate.

FALSE. If we don't get any information from people working on the company, we can barely get useful and complete requirements.

> **Exercise 2:** 
> 
> Read the following text about the development of a software product, and then identify the system, functional and non functional requirements:
> 
> *A blog has three types of users: administrators, editors and visitors. Any of them must log in in order to enter the application. Administrators can register other users, editors can publish posts, and visitors can comment them. We expect that this web site has lots of visits per day, so the availability of the service must be high. We must also have several servers in order to balance the load and distribute client accesses. Besides, as we don't have very experienced editors, the user interface for them must be as simple as possible. Every post and comment will be stored in a MySQL database, with daily backups. Passwords will be encrypted in order to prevent possible attacks.*

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
> From the following proposal for a software product, try to identify the system, functional and non functional requirements.
> 
> *A cultural organization is focused on the loan of two type of objects: music discs and books. We need an application aht lets us add new objects to the system from both types. Besides, there are many users that come to this organization. They will need to log in with a user name and password. Then, they may be able to search any disc or book, either by object type (disck/book) and/or by object name (title). Once the object is chosen, they can ask for it if it is not available. Users can have up to 5 objects on loan simultaneously. As this organization is settled in a small town, we don't expect to have many users asking for books or disks at the same time, so we just need a single computer and a small database to store the information. In case a user does not remember his password, the system will send it by email to the same account that he entered when he registered.* 

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

> * The database server must be in a separate computer

SYSTEM

> * If there is no connection with the remote server, the application must show an error message and then close

FUNCTIONAL

> * The response time must not exceed 10 milliseconds

NON-FUNCTIONAL

> * We must have enough bandwidth to send the video in real time streaming

SYSTEM (internet connection) and NON-FUNCTIONAL (enough bandwidth)

> * We must verify that the information entered by the user (name, id and phone number) are correct

FUNCTIONAL

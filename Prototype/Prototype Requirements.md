# Authentication
### Requirements

- Users cannot create accounts through the application.
    
- No public sign-up functionality exists.
    
- User accounts are created and managed by the school system.
    
- Access to the application is restricted to users who have been provided with valid credentials by the school.
    

---

## Authentication Methods

Different user groups may use different authentication methods.

### Staff Accounts

The following roles are considered staff accounts:

- Admin
    
- Supervisor
    
- Teacher
    

#### Requirements

- Staff members authenticate using traditional credentials.
    
- Each staff member has a unique username.
    
- Each staff member has a password.
    
- Credentials are managed internally by the school.
    

---

### Parent and Student Accounts

To simplify access for less technical users, parent and student accounts may use a simplified authentication system.

#### Proposed Prototype Implementation

- Phone number is used in place of a username.
    
- Date of birth is used in place of a password.
    

#### Example

|Username Equivalent|Password Equivalent|
|---|---|
|Phone Number|Date of Birth|

#### Notes

- This approach is intended only for the prototype.
    
- The final implementation may use a more secure authentication system.
    
- Parent and student accounts primarily provide access to informational and read-oriented functionality.
    

---

# User Roles

## Permission Hierarchy

The exact hierarchy may evolve during development.

### Current Prototype Structure

1. Admin
    
2. Supervisor
    
3. Teacher
    
4. Parent
    
5. Student
    

### Permissions

#### Admin

- Highest level of permissions in the system.
    
- Can create and manage user accounts.
    
- Has system-wide access.
    
- Can manage all classes and users.
    

#### Supervisor

- Has authority over assigned classes.
    
- Has a higher level of access than Teachers.
    
- May have access to class-management functionality that is unavailable to Teachers.
    
- The exact set of Supervisor-exclusive permissions has not yet been finalized.
    

#### Teacher

- Can access assigned classes.
    
- Can create posts within assigned classes.
    
- Can interact with classroom-related functionality available to teaching staff.
    

#### Parent

- Can view information related to their child.
    
- Can access posts and updates relevant to their child's class.
    
- Primarily has read-oriented access.
    

#### Student

- Can view information made available to them.
    
- Can access posts and updates for their class.
    
- Primarily has read-oriented access.
    

### Notes

- Supervisors and Teachers primarily operate at the class level rather than the system level.
    
- Supervisors have a higher level of authority than Teachers within the prototype.
    
- Permission details may continue to evolve as requirements become clearer.
    
- The prototype should be designed with enough flexibility to accommodate future changes to role permissions.
    

---

# Class Feed

Each class contains a dedicated feed similar to a social media timeline.

### Requirements

- Every class has its own separate feed.
    
- Content posted in one class should not appear in another class.
    
- Teachers can create posts within their assigned classes.
    
- Students can view posts belonging to their class.
    
- Parents can view posts relevant to their child's class.
    
- Supervisors may have additional moderation or management permissions related to class content.
    

### Notes

- The feed is intended to function similarly to a Facebook-style timeline where users can scroll through class-related posts and updates.
    
- The exact set of posting and moderation permissions may evolve as requirements become clearer.
# Backend Developer (PHP, WordPress) Handson

## Instructions

```
1. Create a new PRIVATE Github repository.  Type in your email in the README in your private repo for understanding.  Add "idteam-at-onecom" as a collaborator.
2. Read and understand the questions carefully before attempting them.
3. Record your assumptions about anything in a file for interviewers to consider.
4. This is a CONFIDENTIAL material of one.com and should not be shared with anyone else.
```

## Assignment

**Objective** - To develop a WordPress plugin to implement REST APIs

### Instructions

1. **WordPress Setup**
   - Install a test WordPress setup on localhost
2. **Database**
    - Setup a new database named `storefront` in addition to test WordPress database
    - Create a table `users`: ID, name, email, contact_no
    - Create a table `orders`: ID, user_id, subscription_term (user_id of `users` table)
2. **WordPress Plugin**
    - Create a new WordPress plugin named `rest-api` under `/wp-content/plugins`
    - Create the necessary PHP files inside the plugin directory
3. **Register custom namespace**
    - Use the `register\_rest\_route` function to create a namespace named `storefront`
    - Create two routes: One to submit data and another to retrieve the data
4. **Authentication**
    - Implement JWT based authentication on above routes.  Do not use `is_user_logged_in`.
5. **REST APIs**
    - Implement one REST API endpoint to receive following data in JSON format: `name`, `email`, `contact_no`, `subscription_term`
    - Ensure proper validation
    - Store the data in the tables `users` and `orders` of `storefront` DB
    - Implement another REST API endpoint to fetch all the data from `orders` table
    - Ensure you do not use `$wpdb` default object to do database operations.  Use core PHP database functions to execute sql queries.
    - Ensure proper error handling
6. **Testing**
    - The APIs should be testable through tools like Postman or curl
7. **Documentation**
    - Ensure proper documentation on how to run the project locally
    - Ensure proper documentation on how to use the REST APIs    
8. **Requirements**
    - Please make an effort to use custom PHP code instead of relying on WordPress built-in functions whenever it's feasible



## FAQs

Q: Where do I have to solve the assignment?

A: Implement it on your local system or use any virtual server on the cloud/VPS, etc. We will need this system again during the panel interview, so do not destroy your work.

Q: Do I have to use a particular operating system?

A: It is up to you to choose operating system of your choice.

Q: Can I make the repository public?

A: No, you should not do that.

Q: Can I purge stuff on my system once changes are pushed to repo?

A: No, you should not do that. If you are selected for the panel interview, then the panel will ask you to show it live.

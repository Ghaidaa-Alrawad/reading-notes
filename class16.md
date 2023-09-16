# Spring Security overview

## What does it mean to authenticate a user?

It is the process of confirming the user's identity (verifying the identity of a user), typically by checking their credentials, such as a username and password, to ensure they are who they claim to be. 

## What does it mean to authorize a user?

It's determining what actions or resources a user is allowed to access or perform after they have been authenticated. It involves checking the user's permissions and roles to ensure they have the necessary rights to perform a specific action or access certain resources.

## What are the three possible outcomes of the AuthenticationManager’s authenticate() method?

- Return an Authentication with authenticated=true: This outcome indicates that the authentication was successful, and the input represents a valid principal (user), the user is authenticated.
- Throw an AuthenticationException: If the authenticate() method believes that the input represents an invalid principal, it throws an AuthenticationException, and this means the authentication failed, and the user is not authenticated.
- Return null: If the authenticate() method cannot decisively determine whether the input represents a valid or invalid principal, it returns null, so in this case, the authentication result is inconclusive, and further processing or authentication checks may be needed.

---

# Spring Auth cheat sheet

## Reviewing the cheatsheet:

The Spring Auth Cheat Sheet outlines the steps to set up authentication and authorization in a Spring application. Let's review each step briefly:

**Step 1:** Set up a user model and repository for user data.

**Step 2:** Create a controller for user-related operations (e.g., registration and login).

**Step 3:** Implement UserDetailsService to load user details by username.

**Step 4:** Implement UserDetails in the user model.

**Step 5:** Configure security in WebSecurityConfig:

- Set up a UserDetailsService.
- Define a password encoder bean.
- Configure authentication and security rules.
- Set up form-based login and logout.

**Step 6:** Create a registration page with a form for user registration.

**Step 7:** Create a login page with a form for user authentication. Display user information from the Principal.

---

## Things I want to know more about

- Advanced Spring Security Features
- Authentication and Authorization Mechanisms

 
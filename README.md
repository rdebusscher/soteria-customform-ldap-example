# soteria-customform-ldap-example
Custom form authentication with JSF PrimeFaces and LDAP

## Demo

Demonstration of a Custom Form implementation with JSF/PrimeFaces and LDAP authentication/Authorization

## License

[http://www.apache.org/licenses/LICENSE-2.0](Apache License, Version 2.0)

## Compatibility

The code should work on all Java EE 7 servers which support Soteria (Payara 4.1.1.161, JBoss WildFly 10 and TomEE 7.0.0-SNAPSHOT (from 05-05-2016 or later) ) but is only tested on WildFly for the moment. 

## Important snippets

### login.xhtml

The custom login form.

### index.xhtml

Public available landing page.

### unauthorized.xhtml

Page when the user isn't authorized to see the application.

### LoginBean.login()

Programmatic authentication of user with supplied credentials (Using the Security Context)

### LoginBean annotations

CDI annotation Definition for the Authentication Mechanism and LDAP authentication.
 
### web.xml security constraints

Defines that all urls with the format /pages/** are protected with the role devgroup2.
 
### UserBean

Shows the Authorization and Authentication information. 
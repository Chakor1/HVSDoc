# Authentication scheme

## Basic authentication

Basic HTTP authentication: For the Authorization header, specify a Base-64-encoded string of a user ID and password delimited with a colon (:). The following is an example of the Authentication header when the user ID is sample-user, and the password is sample-password.
**Example:** <br>Authorization: Basic c2FtcGxlLXVzZXI6c2FtcGxlLXBhc3N3b3Jk
Also, when you use the curl command to send an HTTP request, you can use the -u option of the curl command to assign a username and password. However, if special characters are included, they must be enclosed in double quotation or single quotation marks. The following shows an example of using the curl command option.
**Example:** <br>-u "sample-user: sample-password"

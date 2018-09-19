'''
GC.Collect		//Dont use
StreamWriter		//Stream close
SqlConnection		//connection Close
value="*"			//Dont use wildcard(overly permission cors)
HtmlInputHidden		//check for sensitive hidden filed
Console.WriteLine		//Dont use (use console.log or console.out)
maxRequestLength		//check the size in web.config file
X-XSS-Protection		//It must be true
timeout			//check for long timeout
httpOnlyCookies		//Must be true
debug="true"
		//Must be false (Display debug information)
customErrors mode	//Must not be false
connectionStrings		//Check for hardcoded password (XML Config File)
requireSSL		//Must be true in the form
start			//check the parameter for user input(command execution)
.Text			//check RHS value (XSS)
sleep			//Check the time(DOS)
readline			//DOS (Limit the read size)
Request[			//Injection & Not safe to use
Request.Form[		//Injection
Response.Write		//Dont use(Sensitive information leakage)
DirectorySearcher		//check for authentication (username & password)
DirectorySearcher		//check the parameter for user input (LDAP Injection)
DirectoryEntry		//check for authentication (username & password)
DirectoryEntry		//Check the parameter for user input(LDAP manipulation)
FileUpload		//Restrict the file type(Misuse file upload)
.Redirect			//Check the parameter for open redirect
HttpCookie		//check secure flag enabled or not
HttpCookie		//check httponly enalbed or not
HttpCookie		//check cookie expires time
HttpCookie		//check for broad path and domain name
useUnsafeHeaderParsing	//It must be false
NetworkCredential		//check the parameter for hardcoded password,username
.WriteLine		//check parameter for sensitive information
'''

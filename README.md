ManageEngine Multiple Products Authenticated File Upload

[CVE', '2014-5301'],
['OSVDB', '116733'],
['URL', 'http://seclists.org/fulldisclosure/2015/Jan/5']

Description from original exploit:
        This module exploits a directory traversal vulnerability in ManageEngine ServiceDesk,
        AssetExplorer, SupportCenter and IT360 when uploading attachment files. The JSP that accepts
        the upload does not handle correctly '../' sequences, which can be abused to write
        to the file system. Authentication is needed to exploit this vulnerability, but this module
        will attempt to login using the default credentials for the administrator and guest
        accounts. Alternatively, you can provide a pre-authenticated cookie or a username / password.
        For IT360 targets, enter the RPORT of the ServiceDesk instance (usually 8400). All
        versions of ServiceDesk prior v9 build 9031 (including MSP but excluding v4), AssetExplorer,
        SupportCenter and IT360 (including MSP) are vulnerable. At the time of release of this
        module, only ServiceDesk v9 has been fixed in build 9031 and above. This module has been
        been tested successfully in Windows and Linux on several versions.

Ported by: Jeff Berry
Tested on: MS Windows 2008 Server and ManageEngine Service Desk Plus 7.6.0

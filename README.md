# mongodb
mongodb university labs
Outgoing port tester

This server listens on all TCP ports, allowing you to test any outbound TCP port.
You have reached this page on port 27017.
Your network allows you to use this port. (Assuming that your network is not doing advanced traffic filtering.)
Network service: unknown
Your outgoing IP: 139.5.50.237

Test a port using a command

$ telnet portquiz.net 27017 
Trying ...
Connected to portquiz.net.
Escape character is '^]'.
$ nc -v portquiz.net 27017 
Connection to portquiz.net 27017 port [tcp/daytime] succeeded!
$ curl portquiz.net:27017 
Port 27017 test successful!
Your IP: 139.5.50.237
$ wget -qO- portquiz.net:27017 
Port 27017 test successful!
Your IP: 139.5.50.237
# For Windows PowerShell users
PS C:\> Test-NetConnection -InformationLevel detailed -ComputerName portquiz.net -Port 27017
Test a port using your browser

In your browser address bar: http://portquiz.net:XXXX

Examples: 
http://portquiz.net:8080 
http://portquiz.net:8 
http://portquiz.net:666 
I got complains that portquiz is not working on port 445. My hosting company OVH is probably blocking this port. Sorry about that. Feel free to contact them. See my blog post and OVH forum post (french).

Your browser can block network ports normally used for purposes other than Web browsing. In this case you should use the telnet or netcat commands to test the port.

Please also note that this server uses some port for real services (22, 25), so testing with your browser on those ports will not work.

Contact/feedback:


Marc MAURICE

See also:
Blog post on this topic and How it works
Firebind, a commercial tester. javascript test
outPorts, a tiny program to test a range of ports using portquiz

In order to continue in this course, you must be able to make outgoing requests from your computer to database servers we have set up in MongoDB Atlas. Those servers run on port 27017 in Amazon AWS.

Please confirm that port 27017 is not blocked by clicking http://portquiz.net:27017.

If successful, you will see a page load that indicates you can make outgoing requests on port 27017.

If a page does not load and your request eventually times out, outgoing traffic to port 27017 is probably blocked on your local network. If this is the case, please contact your IT department to see if there is a workaround or try to make the request from another location.

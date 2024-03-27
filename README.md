# Ex-01-SOAP-based-Web-Services

## Aim:

To create and execute SOAP-based web service program using server, client and client- side remote invocation.

## Procedure:

### Server-side:
#### Step 1:
Open NetBeans IDE.
#### Step 2:
Click File->New Project. Choose Java Web and then Web Application and click Next.
![image](https://github.com/DhareeneRK/Ex-01-SOAP-based-Web-Services/assets/119434052/42102d83-1500-42e4-8083-d3673cc836c1)





#### Step 3:
Give your Project a suitable Name and then click Next.
#### Step 4:
In the next window, make sure you have selected Server as “GlassFish Server” and Java EE Version as “Java EE 7 Web”. Click Finish.
 ![image](https://github.com/DhareeneRK/Ex-01-SOAP-based-Web-Services/assets/119434052/55f2a995-fc9b-40fb-b4cb-287358cbf9aa)


 


#### Step 5:
Your new project will appear in the Projects tab in the left-most part of NetBeans.

#### Step 6:
Right click your Project and select New->Web-Service.





#### Step 7:
In the new window, give your web service a name and a package name. Click Finish.
 




#### Step 8:
A new coding tab will open that contains your web service.

#### Step 9:
Expand the folder “Web Services” under your project. You should see your newly created web service. Right-click on it and choose “Add Operation”.






#### Step 10:
A new window to add operation will appear. In that give Name, Return Type to your operation. Then click the Add button to add necessary arguments/parameters for that
 
operation. (Since we are demonstrating simple addition, we use two arguments/parameters.) Once you are happy with your parameters/arguments, click OK.




#### Step 11:
NetBeans will automatically generate the skeleton for the operation which will be like,

![image](https://github.com/DhareeneRK/Ex-01-SOAP-based-Web-Services/assets/119434052/37bda11f-2a88-4142-befb-5c19117e8d63)




#### Step 12:
. Replace return 0.0 with return (a+b)

#### Step 13:
Save your project. Right-click on the project, select “Clean and Build”. Once the Building process is successful, again Right-click on the project, select “Deploy”.
Deploying might take time depending on the size of the project. 

### Step 14:
Once your project is successfully deployed, right-click on your web service name and select “Test Web Service”
![image](https://github.com/DhareeneRK/Ex-01-SOAP-based-Web-Services/assets/119434052/d0dfb36c-0455-4712-a03a-d772945806cf)


 


#### Step 15:
A new browser window will appear which will look like this





#### Step 16: 
You can give inputs to your web service and check whether it is working properly or not. If it is working properly, you will get a page like this


 
### Client-side:


#### Step 1:
Create a new Java Web Project in NetBeans. (Follow Steps 1-5 as in section 1.1)
#### Step 2:
Right-click on the project and select New->Web Service Client.





#### Step 3: 
A new window will appear. Select “Project” under the heading “Specify the WSDL file of the Web Service.” and click Browse

#### Step 4: 
A new window will appear, in that carefully choose appropriate web service and click OK.


 
#### Step 5:
The Project file will be filled with the location to the WSDL file of the web service. If you prefer, you can give a package name. Or else click Finish




#### Step 6:
In the Output Window at the bottom of NetBeans, you can notice that the client gathers the operations available in the web service.

#### Step 7:
Once it is done, you should see “BUILD SUCCESSFUL”.

#### Step 8:
Right-click on “Web Pages” under your Project and select “JSP”.



#### Step 9: 
A new window will appear, give a name to your jsp page and click Finish.

#### Step 10: 
Expand the folder named “Web Service References”-> “Addition” “Addition” “AdditionPort”. Once expanded you should see all the operations available in your web service.

#### Step 11: 
Carefully drag “add” operation and drop it into the JSP page. NetBeans will automatically create the code for invoking this operation which will be like,
 




#### Step 12: 
Give values to your arguments and run the JSP file. 

#### Step 13:
A new browser window with the output will appear. 

### Client-Side Remote Invocation

#### Step 1: 
Follow Step 1 and Step 2 as in Client-side (section 1.2).

#### Step 2:
A new window will appear. Select “WSDL URL” under the heading “Specify the WSDL file of the Web Service.” and type the URL of the web service’s WSDL file. (Typically, the URL of the form http://ip:8080/Proj_name/Webservice_name?wsdl)
 



#### Step 3: 
The remaining procedure is the same as the Client-side.


## Result:
Thus, the SOAP based addition program using Web service is executed successfully.

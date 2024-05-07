# osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- IIS & Management Console
- PHP and Rewrite Module
- MySQL
- HeidiSQL
- osTicket

<h2>Installation Steps</h2>

<p>


  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/9ae32d84-90c7-4a06-8ec0-92e40e480d58)
  Create a Resource Group on azure.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/b75db335-15eb-4b2d-b1d1-541087094126)
  From this picture. Go ahead and type in RG-Osticket for resource group name. You can set the region to anything.
  After doing that, hit the review and create button and the resource group will begin to start downloading.
  
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/a9a27c1f-3126-4d60-ab4f-6dc2e8cc3a23)
  Now we can also create our VM (Virtual Machine). Make sure to check the box under the word LICENSEING before moving onto the next step and creating and reviwing the VM. 
  Also don't forget to write down username and password that was created while creating the VM.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/6f08222d-2221-4a99-8edc-6927aae3ebe2)
  Once the Resource Group and VM are created. We can now go to the VM tab and copy the public IP address.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/50353da9-3790-44e5-acb6-b087992a6144)
  
  Type in the search bar remote control connection and click that app. It will bring up the box in the picture up there. Paste the public IP address and click connect.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/00d5558b-4aa5-4024-ba55-09a052763342)
  
  This pop up box will come up, from here click "more choices" and click the "Use a different account" box. From there you can enter in the username and password that was created while making the VM.
  After all of this is done. Your VM will load up and start and now we can start installing Osticket on our VM.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/a5f2d17a-b6a7-4759-b465-a750f87ca0b7)
  In your VM right click the windows icon and press the "run" tab. From there type in "control" and it will bring you to the screen shown in the picture above. 

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/9dd67f9b-c828-4022-b026-51083149410b)
  
  Click the word "program" it should bring you to this screen. Once on this screen click on the word "Turn windows features on or off"

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/9cd5ae98-99ae-4337-848a-32d75b5bfc79) 
  
  Now we will have this box pop up. Checkmark the box Internet Information Services and click the little plus sign box to expand it.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/2310046f-b384-4b5d-9fa9-4f37864bb23a)
  
  From here checkmark all the boxes shown in the picture above. What we are doing is installing all the prerequisites for IIS in your VM.
  
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/41132566-b7b9-4a72-897b-241af76f0042)

  Also checkmark all of these boxes and after doing that. Hit the "ok" button and it should start installing everything in your VM.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/5185a6d2-b39c-4980-b71e-6670ba543640)

  After everything is install. Open up a new tab and type in the search bar 127.0.0.1 from there a screen in the picture above should of popped up. If it popped up that means you have successfully installed all
  of what's needed for IIS in your VM.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/227aa382-a4a2-49ca-8a2c-40f9d366a05c)

  From here click on PHP Manager for IIS and download it in your VM. It's a pretty straight foward step.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/7c4b772f-ba89-4274-951c-63abd5985674)

  This is also the same step as before, but this time we are installing Rewrite Module in our VM.
  After both of those are done being installed. We are going to create a directory for PHP on the local hardrive. We will make a new folder in our C drive.
  
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/7b73f952-381d-455e-b104-13d9ac40209a)
  
  Now we are in our C drive. Make a new folder and name it PHP.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/56dec34f-6d0c-490a-a837-7d959439ee2d)

  So the next step is to click installation file and download a file named php-7.3.8-nts-WIN-32-VC15-x86.zip

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/47cce173-0e11-43aa-a55f-90f365c4820e)

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/b986597a-7a26-490e-a01f-d6f207b1a995)
  
  Now go back to our download folder and you'll see that the file is there along with the previous two files we have already downloaded.
  Once we are on that screen. We can right click the new file we just downloaded and extract all. It will ask for a new destination, from there we will unzip the files into our PHP folder we had created
  previously in our C drive.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/6bd2bb28-89a6-49f5-920a-0302b7784de2)
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/ab77d0d0-46fe-4007-898d-5f9ddc1486d2)

  Next we will download these two files in our VM.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/2447d577-c3e3-4703-9ddb-6850fbc4567c)
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/352ad521-64a6-4852-bde8-c191ee0da98a)
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/1b01cee8-b48f-4041-baa9-f241190b0d3d)
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/bfab4b4b-5f8e-4c99-9c7b-bb418344ceb5)
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/926f4027-677c-4a1f-84d6-918999f14968)


  Follow these steps one by one after we are done downloading MYSQL. We need to create our new password. In this case for our training VM
  make up a password and write it down if need be, after that is done hit the excute button and let it run. But don't make it a daily habit in real life.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/8d386e6c-c035-4d06-8982-00a170cac301)
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/d46ed7d2-8f3e-4516-bd11-9e30b59063c5)
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/f9a3b295-35ff-45e2-aa3c-a411e50c59fc)

  In this next step. Go to the windows icon, type in IIS and right click IIS and select "Run as admin"
  The last picture you will see that all the prerequisites that we had downloaded are now in here.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/2648d709-8892-4132-954d-5fbd09bae5f5)
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/c90cc929-3b08-4b77-a149-ecc97723f1cd)
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/90f57164-8116-479b-bb56-54c29c645308)

  The next thing we do is click on PHP Manager and it's asking us to register a new PHP version. So we'll click on register new PHP version
  browse to our C drive. Click the PHP folder and select PHP.cgi and click open. Then click "ok" and you're all set for that. It is recommended to restart IIS
  from it's home screen. The reason being is that we want everything to work and be ready for Osticket.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/ecf1efd2-2461-4834-a5a6-05ac9bd86317)
  
  Download Osticket
  
  Step 1
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/8343fa30-a453-436b-930a-3e6bace3d6b7)

  Step 2
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/99c124bd-5c9d-40e6-8a52-1574be47de1b)

  Step 3
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/2f1f3a34-e50b-4256-8f53-b0e23f0b0854)

  Step 4
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/95eb8a05-1251-4a65-abbe-62476b9bd378)

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/cc99ec11-28e2-49cd-8fa9-de6663c44bdc)


  There are multiple steps in this part. We open up two file folders. One file folder is already in the downloaded section.
  The other one is going to be in the C drive folder and from there we can click on the Inetpub->wwwroot->move upload folder from the
  Osticket download folder to wwwroot folder. Once that is all done, we can rename the "upload" folder to "osTicket".

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/59ca305b-9713-4e19-bd64-895ef83008e1)

  In this mini section. All we have to do is restart IIS.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/6182263a-8d49-42fd-9cfd-21620103191e)
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/3f1d36dc-47c7-41a3-9eed-a2b82be064d9)

  From here we can click sites->default web site->browse *:80(http)

  Once you press the button browse *:80(http) you should see a tab open that has the picture posted below
![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/578a6390-6d16-47d1-a3c2-bc5dad0c52f7)

  Now we have to enable some extensions. So we can go back to IIS>Default>osTicket, from there we double click PHP Manager then we click enable or disable extension. We have to enable: php_imap.dll, php_intl.dll, and php_opcache.dll. After all of that is enable we can go ahead and refresh the osTicket site in the browser. And you'll see that some of the X's that are highlighted in red are now green.

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/8fd3d694-85bf-4a8a-b45a-2f056ee80ae5)

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/980a6970-e938-4fd0-8712-9e0894a3309b)

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/9c1f0276-b525-440c-98a7-4a724db51734)

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/e5be847a-036a-4cb4-b7a0-2c3be206109d)

  In the image below. We need to change the name os-sampleconfig in the wwwroot folder to os-config. So I have already gone and done that, so that's why it's not shown in the image below. I hope it makes sense
  even though the word os-config is not highlighted.
  
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/d5ca5d8e-6efd-435b-89b8-baebc45f24d2)

  In this next step we are going assign permissions under the osticket-config.php. We are going to disable inheritance and remove all. Next we are going to add in new permissions for everyone and apply it for
  all

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/12b17b5a-1686-4415-89e8-ab9956cf1c29)

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/364a5890-031a-4873-abad-065e6a45162b)

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/20b639c0-83e8-4cb6-bfa2-d35f3cdf6d28)

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/045317b0-0bc0-41ea-bf89-d1c930d412c6)

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/b5e74677-1c5f-4f00-b82d-734b63f73ed1)

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/d4b944dd-8c98-4b8b-aa33-bb66da342a8d)

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/5e5796a2-b6e7-4ac5-8f6b-54695c13ce1c)

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/75d65761-d0a6-4afd-af6b-19738ed779f9)

  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/6a7ae8f1-7ae9-4a39-8131-139c53d07b4a)
  
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/f0599ffe-45de-4eee-a8cb-ea34448ced6b)

  Following the pictures posted above should give you a clear indicator on how to assing permissions for everyone.

  
  In this step, we are going to set-up os-Ticket in the browser. So we can just fill out everything that is listed in the browser.
  
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/7f6e6e43-7957-4584-a717-77cb4d60178f)


  The next step will be to download HeidiSQL. Once it's done downloading hit the finished button and HeidiSQL will launch.
  Once it's launch, we will create a new session. We will enter our username and password we got when we set up MySQL server. Once that is done we can connect to the session and create a database
  called "osTicket".
  
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/1b9d85be-12b8-4ebc-944e-e5c6cc5aa492)

  
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/0e4623e5-663e-49db-a95d-85f7873acbfa)


  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/0a52763f-df0c-4763-a746-0870a2237bf1)


  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/494eedb9-afdf-43dc-b27f-d5576b01ab14)

  Once we have created the database, we can go back to the osTicket browser and fill out the rest of the forms.
  Look over everything again and make sure it's all good to go. Then we can click the button "Install Now!" If everything is correct the image posted below should show up and now we can proceed to the next step.

  
  ![image](https://github.com/Sunnyyvaj/osticket-prereqs/assets/165757391/b2947beb-b7bc-40c4-a0eb-730e771ac9fe)

  So there are a few steps left to do, nothing major but minor clean up stuff. 
  We can go ahead and delete the setup folder in the osTicket folder under the wwwroot folder.
  After that we can also set the permissions to "read" only.
  It may sound confusing without pictures, I forgot to include the pictures. Again I am sorry.
  



  











  </p>
<p>

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

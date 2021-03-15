# pms.exe
## Setup database
  ### 1. Restore backup
  #### 1.1. Query
      RESTORE DATABASE Adventureworks FROM DISK = 'PathInYourDevice/db/pms.bak'
  #### 1.2 By SQL Server Management Studio assistant
    1. Connect to your SQL Server and right-click on the “Databases” directory and choose “Restore Database”
    2. Click the button beneath the “Source” section next to “Device”
    3. In the “Select backup device” press “Add”
    4. Select the backup file or files (.bak) you are going to restore, then click “OK”
    5. In the “Restore Database” window specify the database’s name you will restore and click “OK” to start
  ### 2. Run script
    1. On the SQL Management studio database side create new database.
    2. In Microsoft SQL Server Management Studio, on the menu, select File > Open > File. 
    3. In the Open File dialog box, browse for the script file ['PathInYourDevice/db/pms.sql'], and then click OK. 
    4. On the SQL Editor toolbar, select the appropriate database, and then click Execute to run the script. 


## Start app
  Double click on PMS.exe
  For first use only, user need to link pms app with database, there are two ways to do this:
  1. Set connection informations on right form;
  2. If you are not administrator of PMS app you can ask the adminstrator for database for the key of connection string and put it on the right textbox.
  To Genretae this key Run PMS app > Admin > Db connection

    ![database setup form][pms1]

[pms1]: https://github.com/maniabrahim/pms.exe/blob/master/readme/1.PNG "database setup form"

## Connection string for demo database
  Without installing database, you can you use the following key to try PMS app
  GmSmyPNKMB3mVNqArrvwLM8C2ax6EUSq2geh279KtjFGQyBc0+YqE0OeLFGuc2iBbTtbcu2zqfTVvMueTj9B+sQ6v1QacuAc5Pz/PorZt875e2S3fDJg+PJO3zA3dqHmHZKyHRdpYncrD2bxRzcN1KJ/Xc5cYMeo/3s+9FBcGfpYkgH/VsD2CQ4Q710OXu8xvV/2wrPNZgrhe6ATvsaJq7GRooLeTG6W+NRjDyZZENGHDMVyeBc0drE9I0TjHB4z

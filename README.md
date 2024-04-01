
# Synchronize and refresh Excel data to the database in real time



Earlier, we talked about [Scheduled Import of Excel into Database](https://dev.to/ryjfgjl/scheduled-import-of-excel-into-database-4pcd).  We only need to make a slight modification to achieve real-time refresh.
Add a new scheduled task, and keep the default setting for timing, which means running in real time

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ckvjm5nrce5sb8vx8tjy.png)



You can see the task running in the scheduled task interface.  When the Excel data is updated, click Save and you can immediately see the updated data in the database.

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/o3o433qpjyq1db6k41f5.png)


Because the refresh frequency is fast and needs to be continuously run, it consumes certain system resources. We can determine whether to execute the import by detecting whether the Excel file has been updated.  If the file has not been updated, the execution can be skipped.


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/pxfzj6ys8gcr3o3t7209.png)



## Introduction and Download of ExcelToDatabase
- [ExcelToDatabase - Automation tool for batch importing Excel files into database](https://github.com/ryjfgjl/ExcelToDatabase/blob/master/README.md)
 

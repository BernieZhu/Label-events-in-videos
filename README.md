# Label-events-in-videos

The collection process followed these approximate steps for each of these tasks:

1. Go to https://requester.mturk.com (https://requestersandbox.mturk.com for test)
2. Go to Create
3. Go to "New Project", and select Other (It will be edited anyway)
4. The task folders should include the settings you need. Please create a new name for your task. Pay should be adjusted such that payment is at least $8/h at reasonable pace.
5. Under "Design layout" select Source, and paste the interface in "main.html". Edit as needed. You can unselect source to view the interface, but you will need to upload a CSV file in the next steps to actually see some of these scripts do anything.
6. You are now finished with this one time process of creating the interface.
7. Go to Create again
8. Locate your interface, select "Publish Batch", and upload a CSV file with the information for your HIT. "example.csv" can be used for reference.
9. When you verify that everything looks good, you submitt the HIT. Each row of the CSV becomes a HIT where variables of the form ${url} in the layout are replaced by the corresponding columns in the csv file. Testing everything with a small batch first is recommended. 
10. Under the manage tab you can monitor the progress, download the results csv, and approve the HITs. Running the tasks through some verification procedure before approving is always adviceable, such as having each task completed by multiple workers and results compared, or a subset of tasks completed by each worker annotated again.
11. To check your interface, go to https://worker.mturk.com (https://workersandbox.mturk.com for test)

More files, scripts, and explanations are available by emailing me.

## Issues
button id="timestampButton" leads to directly submit the answers and jump to the next HIT. Before submitting to MTurk, please comment out this line of code.

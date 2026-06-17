This is my first cloud project and I will be building my application on AWS.
The main idea of the project is monitor the quality of calls in resturants as for example it counts each problem is counted such as "the food is cold." 
or "I received the wrong order." etc. 

So the first prototype will be work in these steps :
1.The recorded voice-call will be sent automatically to Amazon S3.
2.After the MP3 file is received and stored in S3 AWS Lamda will be notified by S3 events notifications it will create a folder for the customer.
3.AWS Transcribe will extract text from MP3 and store it in JSON file in the same folder.
4.AWS Comprehend will extract the important sentiment and key phrases from the text.
5.After all of that AWS bedrock will be used to create summerization of the analyzation from AWS Comprehend and text from AWS Transcribe.
6.AWS Quicksight will be the main dashboard for the stakehoalder as it will show for example : top frequent problems , avg. satisfaction for customers etc.

I am thinking that I will add DynamoDB or Aurora serverless to store customer data but still I do not know at this point.
I will be starting the project today 17-6-2026
note : in this phase at the project it will only contain the dashboard as front-end , in the future the application will have it's unique front-end  and login page .

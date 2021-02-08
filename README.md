# Face_Recognition_Data_Pipeline
A pipeline for scraping the YouTube data with Selenium and python script to create directories for each person automatically and to rename the Persons directory and the videos in it and to save the videos of that person in the respective folder. The videos are then converted to frames and then an output folder is created. The Images of Each person are stored in his respective folder created in the output folder. 
Steps :
A text file with keywords(Youtube Channel name) is created.
The selenium scrapes the urls of videos from those channels
Then with the Pafy( a library to download videos from youtube) we select and download the video with highest resolution
Then we create a folder for each personor keyword in the text file.
The videos from that particular keyword will be stored in the corresponding folder.
The structure would look something like, InputFolder---> Person_ID ---> Video_ID
Then we write another python script to create an output folder and a folder for each person in the input folder with the same name.
Then we convert all the videos in Input folders to frames and save them into Output folder. FRames belongimg to a particular person will be stored in folder corresponding to that person in Output folder.

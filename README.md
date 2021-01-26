# Production of a model
 
In this repo, only the architecture of the code will be done, in order to publish it through an API so that it is available from the web.
 
For this specific example, the publication will only be made for a local server, but the least thing is to send it to an azure server or to any other cloud service, so that it can be seen by other users.
 
Now, let's see the structure of the folders:
 
![24](https://user-images.githubusercontent.com/63415652/103446057-e3e53780-4c40-11eb-9cba-282a8d5a5aa2.PNG)
 
 
As we can see, the code is made up of several files and several folders, which are:
 
* ArchitectVEnv: It is our virtual environment, which contains all the dependencies necessary for the code to work.
 
* in: Here will be the input files, in this project it will be the happiness dataset.
 
* models: The best model found through cross validation will be saved here.
 
* out: CSV or excel files will be output here, but in this case we are not using it.
 
Now there are 4 more files left, which are:
 
* main: This is the main execution file.
 
* models: Where will our models be.
 
* Server: This can allow the configuration of our server.
 
* utils: Here are functions such as loading and file exploitation.
 
Now that we have our architecture and the code ready, we are going to run the server and go to the predict route:

![25](https://user-images.githubusercontent.com/63415652/103446183-628ea480-4c42-11eb-98e8-f14345e3265d.PNG)
 
And voila, we have a json that has a key called production and the value of the prediction that the model generated for us according to the data that we passed to our prediction.
 
And so with the json that it returned, we can treat it in a web, a mobile app, from js, android, etc. Regardless of the nature of what we are doing, we already have the predictions and we have a system that connects to our model, in an extensible, modular, easy-to-use way that we can turn into the solution we are looking for.

# popular-opinion
The API documentation we are using for this project is https://pullpush.io/
Using this API we can use query calls to search submissions and comments from reddit from archived reddit data

Group members:
One of the officers told us about web scrappers we could alternatively use as opposed to the pullpush.io 
These are Selenium and Beautiful Soup

Right now is just a general frame that I imagine we'd need to create in order to do this project with the pullpush API

We need to look into legal use of web scrapping and data from reddit cause if we get to spring showcase we should be 
doing everything legally :)

FILES:

main:
flow of how our project runs and calls from all the different modules' functions to assess an opinion

api_handler:
formats user input into HTTP calls
where we will be making HTTP calls to pullpush
overall interacts with pullpush

data_process:
parsing the JSON responses and restructuring them into a data structure we can analyze

analysis:
an algorithm that takes the data that is cleaned up from data_process and gives the topic a rating/sentiment

user_search:
facilitates all of the different functions and calls upon api_handler to make calls, data_process to format the data into
something manageable, and then analysis to create the sentiment around this subject, and finally takes the output of analysis 
into something that the user can read and get their answer

data_storage:
stores data between each step if necessary 

test_file:
run pytests



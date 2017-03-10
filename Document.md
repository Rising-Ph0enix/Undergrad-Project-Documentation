Service:

https://developer.android.com/guide/components/services.html

https://developer.android.com/training/run-background-service/create-service.html


https://www.tutorialspoint.com/android/android_services.htm

http://stackoverflow.com/questions/25647881/android-asynctask-example-and-explanation

https://androidresearch.wordpress.com/2012/03/17/understanding-asynctask-once-and-forever/


NOTE: HTTP POST is not required to be put in a separate async task - api 111 n/w optns on separate task

Start Documenting the entire process of your project

ASAP!!


1. Run task on separate thread

https://developer.android.com/guide/components/processes-and-threads.html#Threads

2. AsyncTask

https://developer.android.com/reference/android/os/AsyncTask.html

3. Keep the DB class as private helper class in the same file

https://www.quora.com/Can-we-keep-more-than-one-class-in-a-single-java-file

4. Integrate GPS with my app 

Is it possible to change the GPS - public class - to a private class - yes!

i) Study Service Lifecycle & Activity lifecycle - compare & contrast

ii) Study How Google has implemented its lifecycle & convert that for Service lifecycle.

iii) Make sure you include your permissions for you app - create a new activity which calls activitycompat.requestpermissions. :)

5. Modify GPS & ADD POST

Use Google's volley library - easy - TEST

6. Put Modified GPS in separate thread

See #2. Use Async Task

7. Design & Develop basic client side application

16J -> (onButtonClick) -> Send a HTTP request <routeNo> and GET data <latitude,longitude,crowd> and store in vars separately. 
15B ->

-> Go to the next Activity -> (Open Intent and pass the variable parameters..)

NEW ACTIVITY - 2 buttons
1. Track me!
2. Crowd 
2 onButton click listeners - that update the UI....

8. Extend server side API to handle the HTTP Post request...
(to receive data)

Client side - /client/HTTP POST<routeNo>

Server Side - response - res.send(latitude);
res.send(longitude);
res.send(crowd);

Clientside - onResponse (String response) - volley library
{
var crowd=res.crowd;
var lat=res.lat;
var lon=res.long;
Update the UI with your info...
}

9. Material design

10. TNSTC website


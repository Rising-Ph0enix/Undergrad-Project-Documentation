**NOTE:**

Learn about HTTP properly.

https://www.jmarshall.com/easy/http


**NOTE:**

Check the interfacing to see that they are compatible

http://www.androidhive.info/2014/09/android-json-parsing-using-volley/

**Server**

app.use(bodyParser.json())

res.json({Latitude : 32.234});

(little bit below the beginning)

https://scotch.io/tutorials/build-a-restful-api-using-node-and-express-4  

You may require this:

(ctrl+f - route spefcific)

https://www.npmjs.com/package/body-parser



(setting the header to application/json so the json object listener can know...)
http://stackoverflow.com/questions/5892569/responding-with-a-json-object-in-nodejs-converting-object-array-to-json-string


If you have to send a JSON object you could try this:
https://www.youtube.com/watch?v=KSdlX93m-3A

https://www.tutorialspoint.com/json/json_objects.htm


**NOTE:**

Protocol is to send it as a string but express allows you to send it as a json object - internally json(parse) is done by express.

http://stackoverflow.com/questions/22580998/nodejs-response-json-object-or-json-stringify 




**Client** 

**Barebone structure**

http://arnab.ch/blog/2013/08/asynchronous-http-requests-in-android-using-volley/

For parsing the JSON object at the client side - you can try this:

https://www.tutorialspoint.com/android/android_json_parser.htm

and

http://stackoverflow.com/questions/5566669/how-to-parse-a-json-object-in-android

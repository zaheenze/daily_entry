Just like the previous day, I was working on flutter the entire day. Today I was working on the second page of figma design. The page consisted of two containers with a background image which was another container that enclosed the entire screen. The first container was to plan a ride and the second container was to join a ride. The background image was downloaded from unsplashed and then copied to the assets folder that is in the travelapp folder. The image was brought using the Image.asset widget. Then two circles were made using shape widget. The code was:

shape: BoxShape.circle

The height and width was to be given within the Container widget with the shape widget which will give us the circle. Hence, the code is:

Container(height: 232, width: 232, shape:BoxShape.circle)

Once the ciecles were aligned in the center using the Center property in the column, the circle had to be colored in grey with an opacity of 50% after which the text “Plan A Ride '' and “Join A Ride” was added.  The text was added as a child within the circle. Bold characters were given to the texts with the style widget and TextStyle property within which fontWeight widget was used.

Apart from that, something that I learned new for the day was GestureDetector Class, Navigation.pop and Navigation.push widget. GestureDetector widget recognizes or detects gestures. Say the login button which when tapped takes us to the assigned page or takes us through the assigned process. Whereas navigation.push widget is used to navigate or move from a page to another and Navigation.pop is used to navigate back. Hence, the gesture detector widget was used in my login page for the login button which when tapped takes us to the next page after the credentials are verified or matched. The gesture detector code is as follows:

GestureDetector(onTap()

{print(“hi, how are you?”);

}

The code above works when tapped on the login button to print “hi, how are you?”.

There was a session today by the CTO of the company Mr. Abraham. He more or less took the continuation of the previous session taken by Koushik. “Data” was that topic and the same was continued. He started with what was data and we were asked to give our understanding on what was data. Basically any information that has been translated into a form that is efficient for movement or processing can be called Data. Hence the information acquired is then converted to binary form. Now binary could be literally any information converted into 0s and 1s. This binary is further converted into Boolean String. As such, the Boolean string is a function which returns a value of true or false value instead of a number, string or date. A question was asked how a picture was converted into the same. This was well explained by him. He took us to the good old days first where there were only mobile phones and not smartphones. Back in those days, a mobile phone with a two megapixel camera was a big deal. He wanted us to understand what the pixels role was. Nowadays we have cameras and mobile cameras that have a megapixel that extends to a hundred. Hence what the two megapixel about was the question. Mega stands for a million and pixels are small squares that are put together like pieces of a puzzle or mosaic to create a digital canvas. Image resolution is usually determined by the amount of pixels it packs together in a space. Higher pixel count results in better resolution. For easy classification, the pixels are also measured in megapixel format, which basically means one million pixels. Thus, a 2 megapixel camera literally means that it could capture 2million tiny information or pixels an inch. In short, the amount of pixels a device captures is directly proportional to the amount of information the device can process. This is how a HD TV, UHD TV, Youtube resolution etc are determined.

The point he wanted to make was that whatever it be, a string, a picture, anything is processed into a set of understandable code or format or dialect. The code can be somewhere similar to ASCII. Ascii is one of the most common character encoding formats for text data in computers and on the internet. There are unique values for 128 that are 2 to the power 7 alphabetic, numeric or special additional characters and control codes.

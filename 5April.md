Today as usual I was working on my designs on flutter. Even though the login page was quite simple, the flutter was not an easy task. This was my second day working on the same page. But comparatively, I do feel that I have improved on a great scale.

If listed, the things that needs to be coded to match my design are:

1. Grey coloring the email address bar

2. Grey coloring the password bar

3. Grey coloring the Login button

4. Grey coloring the New User button

5. Grey coloring the Guest User button

6. Giving border radius to all the bars and buttons

7. Giving proper border radius to the ZEhive logo

8. Bolding all texts

9. Making the New user and Guest user button to align in the center.

The above mentioned were for the day that is to be completed. Though it took time, I did complete all the above mentioned within the day.

Starting off with the coloring scheme. Grey color had to be filled within all the bars and buttons. The code used for coloring is:

 color: Colors.grey.withOpacity(0.5)

‘color’ is the class used for coloring schemes. This is generally used to fill a container. ‘Colors.grey.withOpacity(0.5)’ is the given property that is applied to the container. That is a grey color property. ‘withOpacity(0.5) is another property added to the coloring scheme. This will allow the user to fill the grey color with its opacity level. Hence 0.5 opacity is taken as 50% opacity. Overall, the code fills the container with grey color with an opacity level of 50%.

The next part of giving border radius. Border radius allows the user to curve the container on the edges. The radius level decides to what extent the border needs to be curved. With this in mind, the code for giving border radius is:

borderRadius:BorderRadius.all(Radius.circular(10))

As mentioned earlier, border radius is also a property given to the container. All represents all the sides of the container. If any of one side is needed to be curved, we can go for:

borderRadius:BorderRadius.onlyLeft(Radius.circular(10))

borderRadius:BorderRadius.onlyRight(Radius.circular(10))

Radius.circular is the extent to which the curve on the border is made.

Bolding the text or character was the next one. The email and password bars were made out of labelStyle class whereas the login, new user and guest user button were simple texts. Hence, bolding of character required two different methods. To bold the email id and password bar, the code used is:

labelStyle:TextStyle(fontWeight:FontWeight.bold)

The property applied to TextField bar is labelStyle. It is used when the label is on top of the input field. FontWeight is another property used within the textStyle property in order to bold the characters. Hence, that is given by .bold

To bold the new user, guest user and login button, the command used is:

style:TextStyle(fontWeight:FontWeight.bold)

The property applied here for the normal text that exists within the container is style. TextStyle is the base given with the property fontWeight. fontWeight allows the user to choose bold italic or underlined text.

Now the part of the day where I spend most of the time was to get a proper fit border radius for the ZEhive logo. Since the logo was an image.jpg, I had to find the code for getting border radius for an image. The code was found and was as follows:

borderRadius:BorderRadius.all(Radius.circular(22), image:decorationImage(image:AssetImage(‘assets/zehive.jpg’)

Image and decorationImage property was accompanied by the borderRadius property in case to add border radius to a photo or image. AssetImage property calls forth the image from the location of the image that is assets folder.

Now all these properties that are border radius, bolding the texts and coloring the container fall under the class of decoration. Decoration is a class used to decorate containers. Hence, before all the above properties are applied for the container or text, it must be within the class of decoration.

In the case of the logo, what we did was to fill a container with the image first and then make it fit properly. This was done with the help of the code:

decoration:BoxDecoration(

borderRadius:BorderRadius.all(Radius.circular(10)),

image:DecorationImage(

image:AssetImage(‘assets/zehive.jpg’), fit:FitBox.fill

))

)

Hence, decoration is the major class used here. BoxDecoration is the property given to the image. Border radius was given to the image. Finally fit property was used with FitBox.fill which will allow the image to fit within the container in the proper dimension. AssetImage was used here and not Image.asset since we had to fit the image inside the container. Image.asset is used where just the image is portrayed and not included inside a container. This was done in order to give the border radius for the logo. If the image is placed as such, we won't be able to give a border radius for the image directly. Hence, we fit the image inside a container and then gave the properties of border radius to the container which indirectly caused the border radius to the image too.

Apart from that there were no sessions for the day. There was a presentation by Arun on Computer networking and hardwares which went well. He went through various components of computers, topologies, various networking types etc.

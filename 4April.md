Monday, the starting of the week started off with flutter itself. I took a little extra time to finish the final piece of design on figma in order to start with the coding part on flutter. Hence, I sat for a while making it uniform with black, blue and grey theme. I added a few more designs to the interfaces to make it more attractive after which Kalyan asked me to start coding. He said that the designing part could be done later. Thus, he asked me to start with the homepage or login page on flutter. He said that at least the first page must be coded within the day.

Firstly, I had to create a new project on the computer which was named as “travelapp” inside which all the default dart file must be included. For that, after creating a folder or new directory, we give the command:

Flutter create travelapp

This code once run will install all the necessary files and folders in dart that are required to merge with Android Studio. Once the installation is done, we must get into the library within the travel app. The command was:

Cd travelapp

Cd lib

After getting inside the library, we create another folder or directory named “pages”. This folder will contain all the dart files of each pages in the application. Hence, we will create other folders like login_page, signup_page, home_page etc. Each of these folders will contain their respective dart file with the code for that respective page. For example login_page folder will contain login_page.dart file. This is created with the vim command:

Cd login_page

Vim login_page.dart

Hence, the pathway would look like:

USERS/travelapp/pages/login_page/login_page.dart

To start with the coding of login page, we have to link the login page dart file with that of the main.dart file. Hence in the main dart file, we literally call forth the other pages once we are done coding the respective page. For this, we import the login page pathway in the main.dart file.  The commands are as follows:

Import ‘package:flutter/material.dart’;

Import  ‘package:USERS/travelapp/lib/pages/login_page/login_page.dart’;

Void main() {

runApp(MyApp());

}

Class MyApp extends StatelessWidget {

@override

Widgetbuild(BuildContext context) {

Return MaterialApp(debugShowCheckedModeBanner:false,

Home: Login_Page(),

);

}}

Once this code is saved within the main.dart file, we can start coding for the login page in the login_page.dart.

The login page from figma had an image in the background. That image was used with the help of Unsplash plugin. So I started the code for login page by adding the background image. Firstly, the image was exported to the system from figma. Secondly it needed to be added. This required a set of procedures. The following procedure had to be followed in order to add the background image:

1. Open pubspec.yaml file

2. Insert I

3. Go to the 60th line.

4. 60th line: (two spaces)assets:

5. 61st line: (four spaces)-(one space)assets/pathway

6. pathway must be the pathway of the image after saving the image in the asset folder which had to be created in the library.

After doing the above procedure, the image pathway is tracked. Now the Image is to be added to the background in the login_page.dart file. For that, the following code is to be followed:

Import ‘package:flutter/material.dart’;

Class LoginPage extends StatelessWidget {

@override

Widget build(BuildContext context) {

Return Scaffold (

Body: Container(

Decoration: BoxDecoration(

Image: DocativeImage(

Image: AssetImage(“asset/homepage.jpg”),

Fit: BoxFit.fill

),)

),);

}

}

This code will portray the background image. Then looking at the homepage from figma, I gave all the text parts in the beginning. “ZEhive”, “Email address”, “Password”, “Login”, “New ZErider?” and “Guest ZErider?” were the texts that were present in the login page. I put them all in a column on center with the last two texts in a separate row that is aligned to the center column. I aligned them using:

mainAxisAlignment: MainAxisAlignment.spaceEvenly

Now I had to give the “enter email address” and “enter password” option in the page. This was given using the TextField command. The code for the email address was:

Container(

TextField(

Decoration:InputDecoration(

labelText: ‘Email address’,

),)

),

The code for the password had an added code to the previous one since it shouldn’t be seen while typing. Hence, the code was as follows:

Container(

TextField(

obscureText: true,

Decoration:InputDecoration(

labelText: ‘Password’,

),)

),

Then margin was added to the email id and password box. Along with that, the box had zero opacity as default which was not according to how I wanted. Thus had to make it transparent. The code was:

Container(

Margin: EdgeInsets.symmetric(horizontal:12), height: 30, color:Colors.transparent, child: TextField(

Decoration:InputDecoration(

labelText: ‘Email address’,

),)

),

Now there were no space between email id and password which was solved with the help of sizedbox command.

Container(

Margin: EdgeInsets.symmetric(horizontal:12), height: 30, color:Colors.transparent, child: TextField(

Decoration:InputDecoration(

labelText: ‘Email address’,

),)

),

SizedBox(height: 20);

Container(

Margin: EdgeInsets.symmetric(horizontal:12), height: 30, color:Colors.transparent, child: TextField(

Decoration:InputDecoration(

labelText: ‘Password’,

),)

),

 

In the second session, Koushik taught about Data. What was data, what are the different types of data and different operators used. Types of data could be generally classified into Numbers, Texts, Boolean, Audio and Video. Hence these can be widely classified into Text, mp3 and mp4 formats.

In usual scenarios, there are two types of operators being used. Arithmatic operators and Boolean operators. Arithematic operators are usually the calculation used ones like +, -, /, *, =, --, ++ etc. Whereas Boolean operators are used as or in case of true or false statements such as ==, >, <, >=, <=, !=, &&, !! etc.

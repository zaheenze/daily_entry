Today, the day could be literally divided into two as a whole. The first was spending a major part of the day on flutter and secondly, my figma presentation.  Talking about the first, I had great improvement in coding as well as understanding the logic that needed to be gotten into my head to code for flutter. I started with an interface of a grocery application from dribble.com The Screenshot of an interface page was taken and I tried to understand how and what all to use in flutter such as row, column, child, children, container, alignment etc. Then I went to write down the code in my notebook. I wrote down the code and asked Kalyan to go through it. He gave me a green signal after pointing out a few mistakes in closing the class brackets and children brackets. Without wasting a second, I opened flutter, terminal and android studio. Started to code what I have written down after making the necessary changes asked by Kalyan. Successfully the code ran in the very first go.

If coded in order, it was as follows:

Scaffold

Column

Text

Image

Text

Text

Text

Row

Text

Container

Text

Before an image could be added to the flutter, few changes need to be made. The steps are as follows:

1. Go to the app directory.

2. Open pubspec.yaml

3. Insert

4. Find the assets part which will be around the 60th line.

5. Change assets to two spaces assets:

6. The next line must have four spaces assets/

7. Save and quit

7. Run the command: flutter pub get

These steps will enable the image feature on flutter. After doing this, we must create a folder named assets in the app directory. The image to be added into flutter must be saved into that folder. When adding the image on flutter, the code must be:

Image.asset(‘assets/filename.jpg’),

Filename.jpg or whatever the name of the image.file format must be given in flutter. If and only if this process is done perfectly, we can add an image in flutter. We can adjust the size of the image by adding width and height for the image. The code is:

Image.asset(‘assets/filename.jpg, width: 390, height: 400),

I could almost imitate the screenshot which I referred to. After that I started experimenting myself through trial and error of codes for better understanding. I added three more containers at the bottom. Then I added various colors to the container. After that the bottom part which had text was put into a container with different colors. So in total a total of five containers in five different colors were given. Kalyan after seeing this asked me to give equal spacing between the containers. This was given with the code:

mainAxisAlignment:MainAxisAlignment.spaceEvenly

This command is to be added in between rows in order to maintain even spacing. After which I went on containers for all the text files with a definite height, width and color. A sample code looked like:

Container(width: 200, height: 200, color:Colors.red, Text(‘Hello!’)),

Another learning in flutter was SizedBox code. This is used for a definite space between two columns.

The first session was taken by Rexilia at 12PM on HTML. The session taught us how to make a circle, create texts in them. Apart from that, how to define a default color to text, how to define key words to do a certain task rather than writing the code every single time. #text and .text was also explained. Margin and padding was differentiated and explained to us. She also let us know where all both of them were used.

We had lunch after Rexilia’s session. I sat again on flutter to move ahead with my trial and errors. After a while, I started perfecting my figma work since I had my presentation at 5PM. I was working on new frames for New User and Guest User riders. By 5Pm, I was all ready to present. The presentation went well. I believe I conveyed all ideas right into them. There were plenty of questions. I answered all questions except one. That one question was what makes my application different from TravelBuddy. I really didn’t have any answer for that. Another question was what makes my application different from Rapido. The audience my application intends to market is totally different from rapido. Rapido is only for local travel. Moreover it isn’t for looking travel buddies but a two wheeler or four wheeler driver. They are not any buddy but just a driver.

The session was taken up by Askin. His topic for the day was Algorithms. The algorithm he stressed was breaking up the process into various steps to make it easier for that respective doing or move. He explained how algorithms can be useful in day to day life to make each task easier and better. Breaking down every task into its minute details will help us to frame those steps and apply everywhere. He also gave us a group task to find an algorithm within the office. That could be anything like switching off the light or air conditioner or something of that sort.

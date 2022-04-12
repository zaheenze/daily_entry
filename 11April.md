Today I was working on my third and fourth page on flutter. The errors which I had faced the previous day was cleared by Kalyan. The third page was the planning page on joining a ride. It had five options which were:

1. Date of Departure

2. Date of Arrival

3. Region

4. Country

5. Place/ Area

Hence, these were coded using ListView Separator. ListView Separator allows you to create n number of containers with the same measurement and with an equivalent spacing between them. The code used was:

ListView.Separated(

itemCount: 5,

SeparatorBuilder:(context,index) {

Return SizedBox(height: 10);

}

itemBuilder:(context,index) {

return Container(

Here, ListView.Separated is the class used. It enables creates a fixed-length, scrollable, linear array of list “items” separated by list item “separators”. Item count gives the total number of the repeated container. It must always be an integer. The itemBuilder is called whenever there are indices ≥ 0 and < itemCount. The separatorBuilder will be called with indices greater than or equal to zero and less than itemCount -1. After these, the text input was to be given inside various container. For that, right before the @override and after the class, we create and define the list. Hence, it will look like:

List<String>details=[‘aa’,’bb’,’cc’,’….’,];

Here, String defines the text to be given inside the containers. Aa, bb, cc etc are the texts of various respective containers. “Details” is the name given to the list that we have made. The list is made with the texts and then these needs to be returned back. Thus, the code is:

Return Container(

Child:Text(details[index])

There are chances that the ListView might take up the whole screen. This is because the shrink property of the ListView is false as default. This could be changed by making it true. The code is:

shrinkWrap:true,

Shrink wrapping the content of the scroll view is significantly more than expanding to the maximum allowed size because the content can expand and contract during scrolling, which means the size of the scroll view needs to be changed whenever the scroll position changes. The containers were aligned with the given sizedbox height ie. 10. Now it had to be aligned in the center where we used the property of mainAxisAlignment:MainAxisAlignment.center inside Column which aligned the containers in the center. The containers were filled with grey color with an opacity of 50% with the color property ie. Color:Colors.grey.withOpacity(0.5)

 Then the texts were made bold with style property ie. Style: TextStyle(fontWeight:FontWeight.bold)

Stroke of width 2 was given with border property and then the border radius was changed to 10 with the help of borderRadius property.

To resize the containers width, margin property was used. Since the opposite side ie. Left and right was to be resized equally, we used the symmetric property horizontally. The code is:

Margin:EdgeInsets.symmetric(horizontal: 25)

In case, if top and bottom is to be resized, instead of horizontal we use vertical.

Apart from this the new learning for the day was MediaQuery. The MediaQuery property is used to provide a size that resizes according to various phones. Hence, instead of giving height and width, if MediaQuery is given, a uniformity will be given in the size. Hence, it will resize automatically according to the phone screen. The code is:

height: MediaQuery.of(context).size.height

width: MediaQuery.of(context).size.width

The Monday meeting was attended where the Hopeww team, Reducated team and Term team discussed their progress and their plan for the week. The plans that had been accomplished from the previous week was also shared. The minutes of the meeting was taken down and recorded by me.

In the afternoon, we had a session on html. We were taught about how a login page is coded. Label was taught to us. How the username and password text appears on the webpages. When input type was given with the help of placeholder, we will be able to enter the text in case of username and password. Placeholder lets us give a text within the box which goes off once we click inside the box. Various types were also taught like checkbox, date and radio. Then the dropdown menu was introduced within the label. The option property was used to give various options within the dropdown.

The next session was taken by Askin. He had two topics in mind to share with us. The first one was based on the computing language itself and the second was a cultural talk on friendship. In the foremost, he went through various keywords like filter, find, push, pop, slice, splice, unshift, shift, reduce etc. He then explained about key value where key value= key+value properties. Hence, a collection of properties in keyvalue is said to be called Object. This said, while coding the keyvalues will have () brackets and the objects will have {} brackets.
The second topic about friendship was something everyone could relate to. A discussion rose when he asked about what friendship means to each and every person. He asked what significant difference were there between friendship and being friendly. Friendship was ones choice to bond with whom he or she wants. But when it comes to being friendly, it is a choice. Being friendly is a trait or character that needs to be inculcated in everyone. It is more or like letting the other person know that we ready to lend a hand in case if that person wants any. In short, it is more of letting others know that we are approachable. The point he wanted to make clear was none should not stick around with the same circle of friends but must be ready to make new friends by getting to know others out of the circle as well as letting others know you.

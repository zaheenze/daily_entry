Today I finished the third page and was working on the fourth page of my figma design on flutter. There were no sessions for the day. In the third page, two more containers were added at the bottom horizontally. One was for the search 4 wheeler and the other was for search 2 wheeler.

The containers were made in a row. Hence, children property was used here. The containers were filled with grey color with opacity of 50%. Then the texts were given. Both had search icons along with the text. Therefore children property had to be used within each container again to give the icon. So each container in the row had children with a text and an icon that is search icon. The search icon was taken from google icons. The flutter code for the icon was:

Icon(

  Icons.search_outlined,

),

The text for the first container was “Search 4-wheeler” and the second container was “Search 2-wheeler” where both where followed with the icon. Then border color with a width of 2 was given. The code was:

Border:Border.all(width:2, color:Colors.black)

Then the border radius of 10 were given to both containers. The code was as follows:

borderRadius:BorderRadius.circular(10)

Since more than one decoration was given to the container, all the above including the filled in color of grey had to be placed inside the decoration widget with the property of box decoration. Hence, the code with all together will look like:

decoration:BoxDecoration(

color:Colors.grey.withOpacity(0.5),

Border:Border.all(width:2, color:Colors.black),

borderRadius:BorderRadius.circular(10)

)

The texts inside the container were made bold using the style widget with font weight property. Hence, this was to be put inside the Text widget itself since it was applicable only to the text. The code looked like:

Text(‘Search 2-wheeler’,

style(fontWeight:FontWeight.bold)

)

Now both the containers were close to each other. An equivalent space had to be given. For that we used the property of mainAxisAlignment with space around. This had to be used at the beginning of the row itself.

The third page was completed and the fourth page which was already started began. The fourth page had profiles that were available for rides with 4 wheelers. The major task that I faced coding this page was the continuous use of child and children with row and column. I had designed it in such a way that there were containers above and below within which texts were there. Started with the background image which was exported from unsplashed. DecorationImage widget was used with ImageAsset property to import the background image from the assets folder. Then the heading container which had the text “4 wheeler ZErides x 3”. There were a total of 3 profiles to be made. It was given in the middle with Column widget and center property. The border color with width 2 and border radius of 10 were given. The text was made bold. Next was starting of the profile. A container was made for a profile with grey color filled with an opacity of 50%. The heading container and the profile container were children within the column of body. A height of 10 was given between the heading container and the profile container using Sized Box widget.

A row was created inside the profile container first. The row had children that is the profile picture in the first place and few texts in the second place. The profile picture was made in a circle within which the photo was enclosed. Hence, the circle was made using the shape widget with circle property. Then the image was inserted using DecorationImage widget and ImageAsset property. The circle was given black border and a grey fill with opacity 50%. Then a column was made after the profile picture which had the basic information about the driver. Three different stanza were there. They were:

1. Name and Age

2. Vehicle brand, model and make

3. Date and day of departure.

The texts were given in their order within the column.

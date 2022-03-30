The whole day I was working and learning about various widgets in Flutter. Few of them were Text, Row, Column and Stack. Text widget lets you create string of texts. In general, Text Widget allows you to display or give text were intended. Text widget code in flutter is as follows:

Import ‘package.flutter/material.dart’;

Void main()

{ runApp(NewApp());

}

Class NewApp extend to StatelessWidget

{@override

Widget build(BuildContext context)

{return MaterialApp(debugShowCheckedModeBanner: false,

 home: Scaffold (Text(‘Hi! How are you?’),),

);

}

}

The text that is given here is “Hi! How are you?”. These set of code will allow you to portray the above text on screen. As default, the text appears at the top left corner of the screen. If the text needs to be brought into the center of the screen, the command for doing the following is:

Import ‘package.flutter/material.dart’;

Void main()

{ runApp(NewApp());

}

Class NewApp extend to StatelessWidget

{@override

Widget build(BuildContext context)

{return MaterialApp(debugShowCheckedModeBanner: false,

 home: Scaffold (body: Center (Text(‘Hi! How are you?’),),),

);

}

}

These set of command will show the text at the center of the screen.

Similarly row and column also follows a set commands. Flutter completely works on the right alignment of rows and column. Flutter can be easily understood if where to place that is in which row and column is understood. Row is the command for the horizontal lane and Column is for the vertical lane. To portray a single text, the row and column is not necessary. But if there is a set of texts, either the row or column or both needs to be mentioned in the code.

The most important part of flutter which I needed to work on was understanding child and children. Child basically means a sub and if it has more than one sub, it is called children. Then the alignment part was taught by Kalynan. MainAxisAlignment widget was used for alignment in center, start or end position. The command was:

mainAxisAlignment: MainAxisAlignment.center

mainAxisAlignment: MainAxisAlignment.start

mainAxisAlignment: MainAxisAlignment.end

 

By 11AM, there was a session downstairs by Koushik. The first part of the session was about Truth Table for propositional statements. Say that there are two statements p and q-

P: The house is painted red

Q: The house is at the corner of the street.

If we are using the AND logic, p^q would be framed as “The house is painted red and the house is at the corner of the house.” The truth table would look like this-

P l Q l p^q

T  T  T

T  F  F

F  T  F

F  F  F

If we are using the OR logic, the sentence could be “The house is painted red or the house is at the corner of the street”. The truth table will be-

P  l  Q l  p OR q

T  l  T  l  T

T  l  F  l  T

F  l  T  l  T

F  l  F  l  F

The second part of the session was about Logical implication. In short, it is about a condition given in the first sentence and second sentence becomes true if the first one is satisfied. For example:

“If you study well, you will get good marks.”

P: You study well

Q: You get good marks.

The truth table if made would look like:

P  l Q  l p->q

T  l  T  l  T

T  l  F  l  F

F  l  T  l  T

F  l  F  l  T

The third part was about Logical biconditional statements. It happens to be a set of sentences where the first sentence provides a condition and the second sentence is true if and only if the first one is met. For example: “You will get good marks if and only if you study well”

P: You study well

Q: You will get good marks.

The truth table will look like-

P  l  Q l p<->q

T  l  T  l  T

T  l  F  l  F

F  l  T  l  F

F  l  F  l  T

 

After lunch, we had another session by Rexilia on Html. In the same, we were taught about how to create text inside a rectangle. How to border the rectangle and align the text, change font and color of the text and border as well. Moreover <div> was the main thing taught.

Back to flutter, then I started learning about Container Widget. Container widget is basically a container that can hold something. It could be anything like a text or even another widget. Say if you wanted a text inside a box that is where Container widget comes into play.

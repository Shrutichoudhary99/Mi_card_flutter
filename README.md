import 'package:flutter/material.dart';

void main() {
  runApp(
    MyApp()
  );
}
class MyApp extends StatelessWidget {
  //const MyApp({Key key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return  MaterialApp(
      home: Scaffold(
        backgroundColor: Colors.teal,
        body: SafeArea(
          child: Column(
            mainAxisAlignment: MainAxisAlignment.center,
           children: [
             CircleAvatar(
              radius: 50.0,
              backgroundImage: AssetImage('android/images/Matnure.jpeg'),
             ),
             Text('Think Organic, Think Matnure',
               style: TextStyle(
               fontFamily: 'Caveat-VariableFont_wght',
               fontSize: 25.0,
               color: Colors.white),

              ),
             SizedBox(
                 height: 30.0,
                 width: 200.0,
                 child: Divider(
                  color: Colors.teal.shade100,
             )
        ),
             Card(
                 color: Colors.white,
                 margin: EdgeInsets.symmetric(vertical: 10.0, horizontal: 30.0),
                 child: ListTile(
                   leading: Icon(
                     Icons.phone,
                     color: Colors.teal,
                   ),
                   title:
                   Text('+91 7404404477'),
             ),


             ),
             Card(
               //padding: EdgeInsets.all(10.0),
               margin: EdgeInsets.symmetric(vertical: 10.0, horizontal: 30.0),
               child: ListTile(
                 leading: Icon(
                   Icons.email,
                   color: Colors.teal,
                 ),
                 title: Text('matnure@gmail.com') ,
               ),
             ),
           ],

          ),
         ),

      ),
    );
  }
}


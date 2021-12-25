
 import 'package:flutter/cupertino.dart';
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';
import 'package:flutter/material.dart';
void main(List<String> args) {
  runApp(
   MaterialApp(
     title: 'MyFirstApp',
     home: MyApp(),
   )
  );
}
class MyApp extends StatefulWidget{
  @override
  State<StatefulWidget> createState() {
  return Myappstate();
  }
}
class Myappstate extends State<MyApp>{

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.blueGrey,
      appBar: AppBar(
        backgroundColor: Colors.red,
        title: Text("myApp"),
        leading: IconButton(
          onPressed: () {},
          icon: Icon(Icons.arrow_back),
        ),
      ),

      body: Center(
        child: Column(mainAxisAlignment: MainAxisAlignment.center,
        children: <Widget>[
         const Text("Maryam Salah"),
         Image.network(
           'https://image.freepik.com/free-vector/gradient-new-year-social-media-cover-template_52683-78659.jpg',height: 300,)
        ],
      ),
      ),
    );
  }
}

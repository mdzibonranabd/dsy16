# dsy16
09/10/2021
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: MyStackWidget(),
    );
  }
}

class MyStackWidget extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(title: Text("Stite Widget ")),
        body: Center(
          child: Stack(
            fit: StackFit.passthrough,
            overflow: Overflow.visible,
            children: [
              Container(
                height: 300,
                width: 400,
                color: Colors.deepOrange,
                child: Center(
                  child: Text(
                    'Top Widget _AmberAccent',
                    style: TextStyle(color: Colors.amberAccent, fontSize: 20),
                  ),
                ),
              ),
              Positioned(
                  top:30,
                  right: 29,
                  child: Container(
                    height: 100,
                      width: 150,
                    color: Colors.blue,
                    child: Center(
                      child: Text(
                        'AM ',
                        style: TextStyle(color: Colors.red,fontSize: 50),
                      ),
                    ),
                  ),
              ),
              Positioned(
                top:30,
                left: 29,
                child: Container(
                  height: 100,
                  width: 150,
                  color: Colors.blue,
                  child: Center(
                    child: Text(
                      'I',
                      style: TextStyle(color: Colors.red,fontSize: 50),
                    ),
                  ),
                ),
              ),
              Positioned(
                bottom:30,
                right: 29,
                child: Container(
                  height: 100,
                  width: 150,
                  color: Colors.blue,
                  child: Center(
                    child: Text(
                      'RANA ',
                      style: TextStyle(color: Colors.red,fontSize: 50),
                    ),
                  ),
                ),
              ),

              Positioned(
                bottom:30,
                left: 29,
                child: Container(
                  height: 100,
                  width: 150,
                  color: Colors.white,
                  child: Center(
                    child: Text(
                      'JIBON ',
                      style: TextStyle(color: Colors.red,fontSize: 50),
                    ),
                  ),
                ),
              ),
            ],
          ),
        ),
      ),
    );
  }
}

Write a code of implement layout
structures  using colum widget  in  flutter?

import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('Column Widget Layout'),
        ),
        body: Padding(
          padding: const EdgeInsets.all(16.0),
          child: Column(
            crossAxisAlignment: CrossAxisAlignment.start,
            mainAxisAlignment: MainAxisAlignment.spaceEvenly,
            children: [
              Container(
                height: 100,
                width: double.infinity,
                color: Colors.blue,
                child: Center(
                  child: Text(
                    'Header',
                    style: TextStyle(color: Colors.white, fontSize: 20),
                  ),
                ),
              ),
              Container(
                height: 100,
                width: double.infinity,
                color: Colors.green,
                child: Center(
                  child: Text(
                    'Content Area',
                    style: TextStyle(color: Colors.white, fontSize: 20),
                  ),
                ),
              ),
              Container(
                height: 100,
                width: double.infinity,
                color: Colors.red,
                child: Center(
                  child: Text(
                    'Footer',
                    style: TextStyle(color: Colors.white, fontSize: 20),
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


Write a code of Implement flutter
image widget in Flutter ?

import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('Flutter Image Widget'),
        ),
        body: SingleChildScrollView(
          child: Column(
            crossAxisAlignment: CrossAxisAlignment.center,
            children: [
              // Display an image from the network
              Padding(
                padding: const EdgeInsets.all(8.0),
                child: Image.network(
                  'https://flutter.dev/assets/homepage/carousel/slide_1-layer_1-6071fb16a5d2d9c3e82864e45f63738f73b31a2933b52e0ac232c5f2dfd74a87.png',
                  height: 200,
                  width: double.infinity,
                  fit: BoxFit.cover,
                ),
              ),

              // Display an image from assets
              Padding(
                padding: const EdgeInsets.all(8.0),
                child: Image.asset(
                  'assets/images/sample.png', // Ensure the image is added to pubspec.yaml
                  height: 200,
                  width: double.infinity,
                  fit: BoxFit.cover,
                ),
              ),

              // Display a placeholder image with circular shape
              Padding(
                padding: const EdgeInsets.all(8.0),
                child: ClipOval(
                  child: Image.network(
                    'https://via.placeholder.com/150',
                    height: 150,
                    width: 150,
                    fit: BoxFit.cover,
                  ),
                ),
              ),

              // Display an image from memory (example with placeholder)
              Padding(
                padding: const EdgeInsets.all(8.0),
                child: Container(
                  color: Colors.grey[300],
                  child: Center(
                    child: Text('Memory Image Placeholder'),
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

# This is h1 header
## This is h2 header
### This is h3 header
#### This is h4 header
##### This is h5 header
###### This is h6 header


## Add Image
![application languages](https://user-images.githubusercontent.com/91416868/213454776-3e147f9c-ef71-42e7-bbe2-249fd40046dd.jpg)


## Add Code
### Flutter drawer

```
import 'package:flutter/material.dart';

void main() => runApp(const MyApp());

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  static const appTitle = 'Drawer Demo';

  @override
  Widget build(BuildContext context) {
    return const MaterialApp(
      title: appTitle,
      home: MyHomePage(title: appTitle),
    );
  }
}

class MyHomePage extends StatelessWidget {
  const MyHomePage({super.key, required this.title});

  final String title;

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(title: Text(title)),
      body: const Center(
        child: Text('My Page!'),
      ),
      drawer: Drawer(
        // Add a ListView to the drawer. This ensures the user can scroll
        // through the options in the drawer if there isn't enough vertical
        // space to fit everything.
        child: ListView(
          // Important: Remove any padding from the ListView.
          padding: EdgeInsets.zero,
          children: [
            const DrawerHeader(
              decoration: BoxDecoration(
                color: Colors.blue,
              ),
              child: Text('Drawer Header'),
            ),
            ListTile(
              title: const Text('Item 1'),
              onTap: () {
                // Update the state of the app
                // ...
                // Then close the drawer
                Navigator.pop(context);
              },
            ),
            ListTile(
              title: const Text('Item 2'),
              onTap: () {
                // Update the state of the app
                // ...
                // Then close the drawer
                Navigator.pop(context);
              },
            ),
          ],
        ),
      ),
    );
  }
}
```

## Make a list
### Day 1 as an intern

- [x] Completed **Introduction-to-github** 
- [x] Completed **Communicate-using-markdown**
- [ ] Next task is **Hello-Github-actions**


## Add task list
### Create new Flutter project

- [ ] Invoke View > Command Palette.
- [ ] Type ???flutter???, and select the Flutter: New Project.
- [ ] Select Application.
- [ ] Create or select the parent directory for the new project folder.
- [ ] Enter a project name, such as my_app, and press Enter.
- [ ] Wait for project creation to complete and the main.dart file to appear.

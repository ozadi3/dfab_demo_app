# draggable_floating_button

We all like the Floating Action Button Widget, but how can it be better?

Well, we made a Draggable Floating Action Button!

You can use it to make the user interact in crazy and unexpected ways with your application.

# How Can I Get This Widget?

1. Add ```draggable_floating_button``` to your ```pubspec.yaml``` file
2. When the notification bar pops up in Android Studio prompting you to get Packages, do so

![Get Packages](https://github.com/ozadi3/dfab_demo_app/blob/master/draggable_floating_button/getPackageFlutter.png?raw=true)

3. Add an import statement in your Dart code like so, ```import 'package:draggable_floating_button/draggable_floating_button.dart';```
4. You are ready to create draggable floating actions buttons


# Usage

```   
      DraggableFloatingActionButton(
          offset: new Offset(200, 200),
          backgroundColor: Theme.of(context).accentColor,
          child: new Icon(
               Icons.your_icon,
               color: lightDfabColor,
              ),
          onPressed: () => foo(),
          appContext: context,
          appBar: appBar,
          data: 'your_data',
      );
 ```

The Draggable Floating Action Button (or **DFAB**), can be created just like the Floating Action Button, but it has a few features in addition:

- You need to pass in an Offset object, to letting the button know where to position itself

- You need to pass in the context and appBar of your application in order for the button to calculate correctly which where it has been dragged to across the application.

- The data field works in a similar fashion it works in a [Draggable widget](https://docs.flutter.io/flutter/widgets/Draggable/data.html)


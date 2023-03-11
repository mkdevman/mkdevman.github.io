---
title: "3D Model View in Flutter"
layout: post
---

3D models are ones that have three dimensions: length, breadth, and depth.When used for various purposes, these models provide a fantastic user experience.Also, including this kind of observation in your software will make it very helpful for users, aiding in its growth and ability to draw in a sizable user base. 


Here, we'll look into Flutter's Model Viewer.
We'll integrate a model viewer demo programme and use the model viewer package in your flutter apps to display 3D models in the glTF and GLB formats. 


A Flutter widget for delivering dynamic 3D models in the glTF and GLB designs.The widget adds a WebView with Google's model-viewer> web component.The 3D model presents a 3D picture, and the user ought to turn towards any direction for the watcher. 


# Implementation

```
ModelViewer(
  backgroundColor: Colors.teal[50],
  src: 'assets/table_soccer.glb',
  alt: "A 3D model of an table soccer",
  autoPlay: true,
  autoRotate: true,
  cameraControls: true,
),

```

``` dart

import 'package:flutter/material.dart';
import 'package:model_viewer/model_viewer.dart';

class DemoView extends StatefulWidget {
  @override
  _DemoViewState createState() => _DemoViewState();
}

class _DemoViewState extends State<DemoView> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text("Flutter Model Viewer Demo"),
        automaticallyImplyLeading: false,
        backgroundColor: Colors.black,
      ),
      body: ModelViewer(
        backgroundColor: Colors.teal[50],
        src: 'assets/table_soccer.glb',
        alt: "A 3D model of an table soccer",
        autoPlay: true,
        autoRotate: true,
        cameraControls: true,
      ),
    );
  }
}


```

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/

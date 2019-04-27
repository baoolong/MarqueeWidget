# marquee
[![pub package](https://img.shields.io/pub/v/marquee_flutter.svg)](https://pub.dartlang.org/packages/marquee_flutter)

一个用ListView做的跑马灯，可以垂直方向滚动，也可以水平方向滚动。由于ListView回撑满空间，所以在水平滚动时，必须设置高度，垂直滚动时，必须设置宽度

A Marquee widght with ListView,Can scroll vertically or horizontally.The ListView will fill up the space, the height must be set when scrolling horizontally, and the width must be set when scrolling vertically.

HomePage：[https://github.com/baoolong/MarqueeWidget](https://github.com/baoolong/MarqueeWidget)

MoreWidght：[https://github.com/OpenFlutter/PullToRefresh](https://github.com/OpenFlutter/PullToRefresh)

<img width="38%" height="38%" src="https://raw.githubusercontent.com/baoolong/PullToRefresh/master/demonstrationgif/20180814_142220.gif"/>

## Usage

Add this to your package's pubspec.yaml file:

	dependencies:
	  marquee_flutter: ^0.1.4
	  
Add it to your dart file:

    import 'package:marquee_flutter/marquee_flutter.dart';

## Example

    import 'package:flutter/material.dart';
    import 'package:marquee_flutter/marquee_flutter.dart';
    
    
    class MarqueeWidgetDemo extends StatelessWidget{
      @override
      Widget build(BuildContext context) {
        return new Scaffold(
            appBar: new AppBar(
              title: new Text("跑马灯"),
            ),
            body:new Container(
              color: Colors.blueGrey,
              height: 30,
              child: new MarqueeWidget(
                text: "ListView即滚动列表控件，能将子控件组成可滚动的列表。当你需要排列的子控件超出容器大小",
                textStyle: new TextStyle(fontSize: 16.0),
                scrollAxis: Axis.horizontal,
              ),
            )
        );
      }
    }

## Notice

由于ListView回撑满空间，所以在水平滚动时，必须设置高度，垂直滚动时，必须设置宽度

The ListView will fill up the space, the height must be set when scrolling horizontally, and the width must be set when scrolling vertically.

## LICENSE
    MIT License

	Copyright (c) 2018 baoolong
	
	Permission is hereby granted, free of charge, to any person obtaining a copy
	of this software and associated documentation files (the "Software"), to deal
	in the Software without restriction, including without limitation the rights
	to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
	copies of the Software, and to permit persons to whom the Software is
	furnished to do so, subject to the following conditions:
	
	The above copyright notice and this permission notice shall be included in all
	copies or substantial portions of the Software.
	
	THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
	IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
	FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
	AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
	LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
	OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
	SOFTWARE.

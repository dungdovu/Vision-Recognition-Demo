
## Requirements
* Android 4.0+ support

* ARMv7 and x86 based devices

* Get the Caffe model and push it to Phone SDCard. For object detection, network(*.prototxt) should use ROILayer, you can refer to [Fast-RCNN](https://github.com/rbgirshick/fast-rcnn). For scene recognition(object recognition), it can use any caffe network and weight with memory input layer.

* Build with Gradle. You can use Android studio to build


## Demo

![](demo/1.png)

![](demo/2.png)


## Usage 

* Download and push the neccessary file to your phone. There should be model and weight in /sdcard/fastrcnn and /sdcard/vision_scene.

` $ ./setup.sh `

* Build and run the application using  gradlew or you can open AndroidStudio to import this project

` $ ./gradlew assembleDebug`

` $ adb install -r ./app/build/outputs/apk`


``` 


## License

	
	Licensed under the Apache License, Version 2.0 (the "License");
	you may not use this file except in compliance with the License.
	You may obtain a copy of the License at
	
	     http://www.apache.org/licenses/LICENSE-2.0
	
	Unless required by applicable law or agreed to in writing, software
	distributed under the License is distributed on an "AS IS" BASIS,
	WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
	See the License for the specific language governing permissions and
	limitations under the License.

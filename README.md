# PicMagic_Gui V1
<div style="text-align: justify;">
The PicMagic GUI is an ImageProcessing Gui is designed to provide users with a user-friendly interface for performing various image processing tasks. It allows users to load images in different formats (such as JPEG, JPG, PNG, BMP) and provides them with tools to manipulate and enhance these images.
</div>
# Notes
1) The project was implemented using Qt Framework and C++ programming language
2) The filters implemented in the GUI are: [GrayScale, Black & White, Invert image, Merge two images, Flip image, Rotate image, Resize image, Crop image, Darken & Lighten, Frame in image,Detect image Edges, Blur image, Purple filter, Infrared filter, Old_tv filter, Sunlight filter, Oil painting filter, Image Skewing Filter, Night Vision Filter, Noise Filter]
3) Please read the steps correctly and complete them until the end

# Steps to setup and run Gui
1) install Qt Framework: you can enter this link to know how install Qt [ https://youtu.be/wR_jXBUW11g?si=imG2NI6KZ3FYLBbO ] Until minute 9:30 but when choose version. you must choose version Q 6.7.0

2) After install Qt Framework: Click on create new Project and It is called the same name as the folder in the project that you will find in the repo link Attached above [PicMagic_GUI],Then you will go to the location of the project in file explorer you created and replace the entire folder with the folder from the project located in the repo.

3) Verifying files in Qt: Now you can access Qt Creator and verify the presence of the following files: [main.cpp, ImageProcessor.cpp] in Source Files and [AutoInfoBox.qml, Main.qml, ImageProcessing.pro] in appPicMagic_Gui and [ImageProcessor.h, stb_image_write.h, stb_image.h, Image_Class.h] in Header Files and [assets folder] in Resources
   
4) Run Application: The last step is to go to [ File explorer => Project location => Build => Desktop_Qt_6_7_0_MinGW_64_bit-Debug ] and copy the path, then go to Qt Creator and open Main.qml and go to line 29 which contains property string temporaryFile: You will put between the Double Quotes " "The path you copied and at the end is /temporary_file.jpgNow You can press on Ctrl + s , after that press on Ctrl + r , if app doesn't Run, Then read Error list at the Bottom

# Problems expected to be encountered
1) You have not taken some of the steps mentioned. You must do them and read them carefully

2) Make sure the following code is present in CMakeLists.txt in Qt Creator:
     ```
      qt_add_qml_module(appFirst_GUI
      URI First_GUI
      VERSION 1.0
      QML_FILES
          QML_FILES AutoInfoBox.qml Main.qml
          SOURCES Main.cpp ImageProcessing.pro ImageProcessor.cpp
          SOURCES ImageProcessor.h Image_Class.h stb_image.h stb_image_write.h

      RESOURCES
          assets/images/parots.bmp
          assets/images/House.bmp
          assets/images/gamma_adjusted_image.jpg
          assets/images/luffy.jpg
          build/Desktop_Qt_6_7_0_MinGW_64_bit-Debug/temporary_file.jpg
          assets/images/image.png
          assets/images/image1.png
          assets/images/log.jpg
     )
     ```
3) Do not change anything or file not mentioned here
# Contributors
Ibrahim Mohamed Saad - [QNQ124](https://github.com/QNQ124)

Ahmed Hussein Mohamed Ahmed - [HaZrDoOo0](https://github.com/HaZrDoOo0)

Ezz eldin Omar Abd El-latif - [ezzeldin2005](https://github.com/ezzeldin2005)

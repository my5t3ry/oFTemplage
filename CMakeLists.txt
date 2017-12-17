
cmake_minimum_required( VERSION 3.3 )
project( openframeworks )

set( APP_NAME   ofApp )

set( OF_DIRECTORY_BY_USER "/Users/sascha.bast/codeBase/c/openFramework/of_v0.9.8_osx_release/" )

set( ${APP_NAME}_SOURCE_FILES
        src/main.cpp
        src/ofApp.cpp )
set( OFX_ADDONS_ACTIVE
        #        ofxXmlSettings
        #        ofxOsc
                ofxGui
                ofxCurlNoise
        #        ofxNetwork
        #        ofxVectorGraphics
        #        ofxThreadedImageLoader
        #        ofxAssimpModelLoader
        #        ofxKinect
        #        ofxOpenCv
        #        ofxSvg
        #        ofxEmscripten (untested)
                )

include( ${OF_DIRECTORY_BY_USER}/addons/ofxCMake/modules/main.cmake )


set(CMAKE_SKIP_RPATH)
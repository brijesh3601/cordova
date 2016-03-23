
Installation Steps after checkout
--------------------------------------------------------
1) npm install -g cordova
1) npm install -g ionic	
2) cordova plugin add cordova-plugin-camera
ionic emulate android -lc

npm install -g bower (this is required to run ionic add ngCordova in right path under 'www'.)

bower install ngCordova ( 'ionic add ngCordova' will not work as it will not create folder under 'www' so browser will throw 404 ng-cordova.js error. Also npm install ngCordova will install plugin & it will also have ng-cordova.js file but path is different so browser will complain)


Main File
--------------------------------------------------------
/www/js/app.js


Run On Browser from command Prompt
--------------------------------------------------------
ionic serve -f chrome

Run on Emulator
--------------------------------------------------------
ionic emulate android -lc"


Reference
--------------------------------------------------------
http://ngcordova.com/docs/plugins/camera/


Installing new Cordova (blank layout) Project Steps
--------------------------------------------------------

1) install Node.js
2) Install Ionic and cordova : npm install -g cordova ionic
3) create a simple project: ionic start camera-plugin blank
4) cd mySimpleApp
5) ionic platform add android
6) Build the project: ionic build android


Emulator Debugging
--------------------------------------------------------

1) Check "Use Host" ( "Unfortunately, launcher has stopped" . On logcat you will see avoids error => No suitable EGL configs found.)
2) set "VM Heap" to 512
3) to view logs open separate nodejs cmd prompt & type 'adb logcat'and then start the emulator.
4) running emulator "ionic emulate android -lc" 
5) AVD setting snap location =>  www\img 



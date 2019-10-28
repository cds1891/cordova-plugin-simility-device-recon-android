# Simility Device Recon SDK Cordova plugin for Android
This plugin allow to execute Simility Device Recon SDK Signal on Andoroid native side from a javascript based application.

## How to install
Go to your mobile folder and run

Cordova:
```
cordova plugin add cordova-plugin-simility-device-recon-android
```

Then run the app for android and check if everything looks fine.

## Call it
Then in javascript:
```
cordova.exec(success => { },                        //success callback
             error => { },                          //error callback
             "DeviceRecon",                         //class name
             "SIGNAL",                              //action name 
            [                                       //args array
                {
                    customer_id: 'brand_uid',       //replace with unique identifier assigned by Simility.
                    session_id: 'session.variable', //replace with sessionID variable
                    user_id: 'user.variable'        //replace with userID variable
                }
            ]);                                     
```

# Plinko

PROJECT NAME: OSIZ-PLINKO

PROJECT URL : https://cryptowalletapi.io/

 
OVERVIEW: 

              First you have to  purchase your apikey through this link https://cryptowalletapi.io/games/

then you can download a build file.


REGISTER:

                   If you are a new user you have to register. You have to fill the all required

 fields.otherwise you have to login.

                               Register Link:  https://cryptowalletapi.io/

                                Login Link    :  https://cryptowalletapi.io/login/

WORKINGFLOW:

Once your payment is completed. It shows a Game Api Keys option show in your page.

In this page your APIKEY generated successfully.

![image](https://user-images.githubusercontent.com/52325658/205283443-ffe637ff-ec5f-49a1-b25f-f8e062b09e6f.png)

In this coinDetails you have to set all the details for token name, token logo, token balance,and also token Id.

![image](https://user-images.githubusercontent.com/52325658/205283489-a0226d13-8192-4e7e-a67b-f7d75235cec6.png)

NOTE: “Here you have to change your apikey(Which apikey you buy)”

This findkey()  you have send the two params to the this.gameInstance.sendMessage.


  PARAMS:

    1.  "GameManager",
    2.  "apiupdatekey"


In JSON.stringify you have to pass the which apikey you buy (eg):apikey: “YOUR APIKEY”, 

if the apikey is wrong you can’t play the game.then call the sendBalance() function.
         
         ![image](https://user-images.githubusercontent.com/52325658/205283542-08dbf9d2-5de8-43ea-96fd-c5bd577caa2f.png)

This sendBalance()  you have send the two params to the this.gameInstance.sendMessage.

                                               1. "GameManager"             
                                         2.  "BalanceUpdate"


 In JSON.stringify you have to pass the coinDetails:this.conDetails.
 
 ![image](https://user-images.githubusercontent.com/52325658/205283588-4e6909dd-1417-4821-aaf7-bcd795f8a7ac.png)

  unity will send the actiontype=="isGameOver"  with the help of actiontype to check the calculation for both win and loss the game.
                         
      calculation: 
                          
                  let coinBalance = (this.coinDetails[index].balance)
                  let balance = (unityObj.balance)
                  this.coinDetails[index].balance = balance

![image](https://user-images.githubusercontent.com/52325658/205283644-eb34c825-84b4-4b7a-b290-9223e5f8c968.png)

Unity will sent the request unityObj.apikey == ‘request’ you have to call the this.findkey() function in it.

![image](https://user-images.githubusercontent.com/52325658/205283684-9acdc17b-b316-4481-b34d-25bf47642cf4.png)

checkDeviceType() is used to check a mobile view or web view, if the window inner width is less

than 600 then it’s a mobile view. Otherwise it’s a web view.

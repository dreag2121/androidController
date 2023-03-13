# androidController
currently making a Wacom controllor working with krita on Android 


I am really hoping to finally finsh this year long project, lol. I have a work around that is very brute force. 

This project uses Automate, keymapper and is to use a Wacom express key with Krita on android.

I am going to try to use the JSON formate to setup the database.

The current method used had this codeing for each button on the contoller.

"ButtonCodek96L1":96,"Layerk96L1":1,"96L1":"N/A","ButtonNamek96L1":"A Button key","kritaNamek96L1":"Wacom layer1","kritaShortcutk96L1":"N/A","ModifiersCodek96L1":0,

I use sheets/excel to expidite code building, which may or maynot be smart. This is the formula I use. 

=arrayformula(char(34)
&"ButtonCode"&"k"&data!G2:G49&"L"&data!H2:H49&char(34)&":"&data!G2:G49&","
&CHAR(34)&data!$H$1&"k"&data!G2:G49&"L"&data!H2:H49&char(34)&":"&data!H2:H49&","
&char(34)&data!G2:G49&"L"&data!H2:H49&char(34)&":"&data!B2:B49&","
&char(34)&data!$F$1&"k"&data!G2:G49&"L"&data!H2:H49&char(34)&":"&Char(34)&data!F2:F49&char(34)&","
&char(34)&data!I$1&"k"&data!G2:G49&"L"&data!H2:H49&char(34)&":"&CHAR(34)&data!I2:I49&CHAR(34)&","
&char(34)&data!J$1&"k"&data!G2:G49&"L"&data!H2:H49&char(34)&":"&char(34)&data!J2:J49&char(34)&","
&char(34)&data!D$1&"k"&data!G2:G49&"L"&data!H2:H49&char(34)&":"&if(data!D2:D49="","0",data!D2:D49)&",")

There is more, but basically its not good. 
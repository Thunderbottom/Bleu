BLEU
======================

Bluetooth instant messaging app for Android.

No Internet Connection required. Works on Peer to Peer Wireless connection.


How it works:
  - To send messages and images, we transmit them in formatted byte arrays in the following format:
      <blockquote>
      [ Message Type, Sender Name Length, ...Body Length**..., Sender ID, Sender Name, Body ]
      </blockquote>
      
    ** The Body Length is separated into tens digits (from least to most significant digit) just in case the body length exceeds the size of a byte.



Notes:
  - If having connection problems, make sure the host creates a room before a client tries to join. 
  - Make sure Higher API Level (Higher Android Version) Creates the Room.
  


#  Simple scenario

The first example [<b>(ndn-simple.cpp)</b>](https://github.com/syaifulahdan/ndndlearn/blob/master/Simple-scenario-Coding/ndn-simple.cpp)  shows very basics of ndnSIM. In the simulated topology there are 3 nodes, connected with point-to-point links, one NDN consumer, and one NDN producer:

Consumer is simulated using  The first example [<b>(ConsumerCbr)</b>](http://ndnsim.net/2.0/doxygen/classns3_1_1ndn_1_1ConsumerCbr.html)reference application and generates Interests towards the producer with frequency of 10 Interests per second (see [<b>ndnSIM applications</b>](http://ndnsim.net/2.0/applications.html)).

Producer is simulated using [<b>(Producer)</b>](http://ndnsim.net/2.0/doxygen/classns3_1_1ndn_1_1Producer.html) class, which is used to satisfy all incoming Interests with virtual payload data (1024 bytes).FIB on every node is populated using default routes (see [<b>ndnSIM helpers</b>](http://ndnsim.net/2.0/helpers.html)) and the content store structure of the original ndnSIM is used. The following code represents all that is necessary to run such a simple scenario

![alt tag](http://ndnsim.net/2.0/_images/aafig-d966166dcbc734645cc600acbd97e5aff63a118c.svg)

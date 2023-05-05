Download Link: https://assignmentchef.com/product/solved-ece-315-assignment-3-media-access-control
<br>
<ol>

 <li>The <em>Media Access Control</em> (MAC) layer in communication interfaces implements the <em>data link protocol</em>, using the terminology of the 7-layer ISO-OSI reference model for computer networks. After consulting reputable resources, use your own words to briefly explain the major functions that are provided by the MAC layer. Briefly contrast those functions with those that are provided by the <em>physical layer transceiver</em> (PHY).</li>

 <li>The <em>Fast Ethernet Controller</em> (FEC) block in the MCF5234 microcontroller provides hardware functions that implement many of the mechanisms required by the MAC layer for an Ethernet interface. For example, the FEC provides a <em>First-In First-Out </em>(FIFO) buffer and a <em>Direct Memory Access</em> (DMA) controller. Briefly explain the purpose of the FIFO and the DMA controller in the FEC. The FIFO has a fixed capacity that must be partitioned between the transmit and receive directions. How would a system designer decide how much FIFO capacity to allocate for each direction? How would that decision be implemented using a value loaded into an FEC register?</li>

 <li>Consider the receive buffers that are used in the Ethernet interface of the MCF5234 microcontroller. If the L flag in a <em>receive buffer descriptor</em> (RxBD) is written by the FEC hardware to 0, then this means that the corresponding Rx buffer is not the last in the received frame; it also means that the data length in the RxBD will be the same value that was written into the <em>Ethernet Maximum Receiver Buffer Size Register</em> (EMRBR). If, however, the L flag in the RxBD is written by the FEC to 1, then this means that the corresponding Rx buffer is the last one in the received frame; it also means that the data length in the RxDB will be equal to the total length of the received frame. What would be the advantage of loading a value in the EMRBR that is at least as big as the length of the longest expected Ethernet frame? What would be a possible disadvantage of loading such a value in the EMRMR instead of a value that is quite a bit smaller than the length of the longest Ethernet frame?</li>

 <li>On lecture slide 10-10 a formula is given for the angle of rotation corresponding to one full step of a stepper motor. If N_sdenotes the number of stator teeth and N_r denotes the number of rotor teeth, the step angle is given by (360 deg/N_s) – (360 deg/Nr). Provide a justification for this formula.</li>

 <li>The stepper motor control algorithm that is described in lecture slides 10-30 to 10-35 assumes that there is one fixed</li>

</ol>

(maximum) slew rate, which will correspond to a particular stepper motor (SM) rotor rotation rate. If the SM drives a train, it is possible that different stretches of track will have different maximum speeds. In that case, the slew rate would have change to conform to the local speed limit. Briefly outline how the SM control algorithm should be modified so that the SLEW period could be made a variable that changes depending on the local speed limit. How, if required, would the code need to be modified in each of the four control algorithm states?

<ol start="6">

 <li>The <em>Internetworking Protocol</em> (IP) is concerned primarily with providing a simple and convenient way of getting a variety of different packet switched networks to work together as a single network. Briefly discuss how this practical priority explains why IP provides only an unreliable and connectionless service using its own node addressing scheme, even if at least some of the underlying networks might already provide reliable communication; also, some of the underlying networks might already provide a very large number of unique addresses for every node (e.g., the six-byte Ethernet physical addresses).</li>

 <li>In your own words, and with reference to the 11-state TCP finite state machine, explain what happens to the TCP enitity in aserver when when the TCP state advances from the CLOSED state to the ESTABLISHED state. Be sure to explain what causes the state-to-state transitions, and specify all of the states that are entered by the server. Then explain what happens when the client, with whom the server is exchanging data messages, decides to terminate the connection. As before, explain the state-to-state transitions and the states through which the TCP entity passes.</li>

 <li>When a TCP connection is established, the window size and maximum segment size parameters must be agreed upon by thetwo end nodes for both directions of the connection. First, briefly explain what factors should be taken into account when these two values are selected for both directions. Then explain how the values are communicated between the two end nodes of the connection.</li>

</ol>
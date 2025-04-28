# cs3357-assignment-2-solved
**TO GET THIS SOLUTION VISIT:** [CS3357 Assignment 2 Solved](https://www.ankitcodinghub.com/product/cs3357-asn2-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;119933&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS3357 Assignment 2 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Purpose of the Assignment The general purpose of this assignment is to explore network programming by building a simplified client-server chat application. This assignment is designed to give you experience in:

Individual Effort Your assignment is expected to be an individual effort. Feel free to discuss ideas with others in the class; however, your assignment submission must be your own work. If it is determined that you are guilty of cheating on the assignment, you could receive a grade of zero with a notice of this offence submitted to the Dean of your home faculty for inclusion in your academic record.

Assignment Task You are required to implement in Python a simple client-server chat program. We are going to start with just basic messaging in this assignment, and then build upon this in Assignment #3 with the ability to follow users or topics, send files, and more! For now, we will be layering this on top of TCP sockets for reliability, but we will be circling back to this in Assignment #4 and replacing this with UDP sockets and a custom-built reliability layer.

At a high level, your chat application will function like this:

You start by launching your chat server. It needs to be first as chat clients will need to connect to it to be able to message one another. When it starts, it picks a random port to listen for clients on, and then reports this port number so that your clients know where to find it. When you start a chat client, you provide it the address of the server and a user name for use in the chat system. On startup, the client will establish a connection with the chat server and register itself with the server. This way, the server knows the client exists to send messages to it later on. Multiple clients can be started in this fashion and so the server must support communicating with multiple clients at the same time. To send a message, a user will type it at a prompt provided by their chat client. Each message is composed of a single line of text. When the user hits enter/return on their keyboard, their client will send this message to the chat server, prefixed with “@username: “, where username is a user name provided during registration. When the chat server receives a message from a chat client, the server will broadcast the received message out to every chat client connected and registered at that time, except for the one that originally sent the message. In this way, every other chat client will receive this message. When a chat client receives a message from the chat server, it will display this message for its user. When a chat client ultimately wants to shut down, it notifies the chat server so the chat server can remove it from its list of connected clients. Likewise, when the chat server shuts down, it notifies all connected clients, so they can disconnect and shut themselves down. (If there is no chat server, there is no point for the chat clients to stick around.) For example, suppose we have started a chat server and it is listening for clients on port 54307. Users Alice and Bob then start chat clients to connect to this chat server, and exchange messages with one another, taking turns typing and reading messages that come in from the other party. Alice has to leave and so disconnects from the chat server. The chat server is then shut down, disconnecting Bob in the process. This sequence of events is shown in the screen shots below.

Chat Server:

Alice’s Chat Client:

Bob’s Chat Client:

Some Particulars Here are some specific requirements and other important notes for this assignment:

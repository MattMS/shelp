# ping

Check if your computer can reach another computer on the network.

	ping www.example.com

This will continue sending packets until you press `Ctrl+C`.

The ping statistics will show you how many packets were sent and how
many responses were received.


## Limit sent packets to 4

	ping -c 4 www.example.com


## Notes

Sends an
[ICMP](http://en.wikipedia.org/wiki/Internet_Control_Message_Protocol)
echo request.


## Links

[Ping on Wikipedia](http://en.wikipedia.org/wiki/Ping_%28networking_utility%29)

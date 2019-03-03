## Send traffic to the load balancer
Send 5,000 requests from a single client - ~64 RPS
ab -n 5000 -c 1 http://phx.mattgartner.org/

Send 60,000 requests via 100 clients - ~6350 RPS
ab -n 60000 -c 100 http://phx.mattgartner.org/

## Send traffic to the load balancer

# Iowa 
Send 100k requests from a single client
ab -n 100000 -c 1 http://phx.mattgartner.org/

# Germany
Send 300k requests from 10 clients
ab -n 300000 -c 10 http://phx.mattgartner.org/

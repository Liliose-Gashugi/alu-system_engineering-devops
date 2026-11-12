# Load balancer

Scripts to double the number of web servers and place them behind a load balancer.

- `0-custom_http_response_header`: configures a new Ubuntu machine with Nginx and a custom `X-Served-By` header holding the server's hostname.
- `1-install_load_balancer`: installs HAProxy and balances traffic between web-01 and web-02 with roundrobin.

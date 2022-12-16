# Commands

- mkdir /var/lib/consul
- mkdir etc/consul.d
- consul agent -server -bootstrap-expect=3 -node=consulserver03 -bind=172.20.0.3 -data-dir=/var/lib/consul -config-dir=etc/consul.d
- consul agent -bind=172.20.0.5 -data-dir=/var/lib/consul -config-dir=/etc/consul.d -retry-join=172.20.0.3 -retry-join=172.20.0.2
- consul agent -config-dir=/etc/consul.d
- consul keygen
- consul members
- consul join 172.20.0.1

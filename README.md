# application-delivery-controller
Is a Abstraction Layer for Application delivery that allows you to fast deploy Production Grad MicroServices and Serverless Functions.

It Links DNS and Gateway Services with Apps that can be combined in a serial flow.

## The Concept
A Application often consist of more then one Service and this Service can run on Multiple nodes.
Also There are common requirments like SSL Authentication and other features like Monitoring or AB Tests Stats and so on that are needed by a varity of services. A Service Mesh is only the First Step it needs often to also offer dns that is missing in most Service Mesh Solutions that exists

maybe you know the service cloudflare they offer one of the best application delivery controllers in the world they are amazing but often you don't want a 3th party to have as much controll or you want to use the same tech for your local services. This is where @direktspeed/application-delivery-controller comes in it supports plugable DNS Providers and offers pre Configured Managed Able DNS/ROUTING services.

It allows you to scale your Public Facing Applications and also allows adding new futures without any downtime.

It is designed to run on more then one node in parallel.


Design Solutions.

Auth, Caching, PreProcessing, Security Audit, FailOver, RelayServer MPROXY Protocol, grpc endpoint, LoadBalancing Solutions.

## How?
HaProxy + DataPlane API + DNSMasq + Bind + Custom App Registry

## Use
register a Endpoint (DOMAIN/IP)
configure the endpoint to point to the right App (CDN,MESH,CACHE)



Register a Application and configure its behavior also specify a next Application or Error

Website 


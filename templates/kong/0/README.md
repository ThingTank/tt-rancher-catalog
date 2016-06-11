# Kong API Gateway

### Info
Kong API Gateway 0.8.3 with Rancher support. Using littlebaydigital/kong and PostgreSQL.

This service uses Rancher Meta Data service to work out the correct container IP address to add to the Kong cluster. And also 
exposes necessary environment variables for easy connectivity with external Kong database.

### Config:
For Kong database host field, you can either:

- select an existing database service in `database link` and leave the `host` as the default value.
- leave `database link` empty and replace `host` with an external database such as RDS.

### Usage:
After the cluster spins up, you should be able to access:

- kong on port `8001`
- kong-dashboard on port `8080`
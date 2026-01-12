The simulation has following 2 sections:

## 1. Recursive DNS
- Select a task to begin with.
- Aim is to find the IP Address of a hostname by recursively querying the DNS Servers.
- Begin from the **Requesting Host** and following proper hierarchy of DNS Servers, find the IP Address of the required server.
- Once the IP Address is found, return it back to the **Requesting Host** along the path in which IP Address was found.
- Keep an eye on the *Communication Log* to know when IP Address is found.

## 2. Iterative DNS
- Select a task to begin with.
- Aim is to find the IP Address of a hostname by iteratively querying the DNS Servers.
- Begin from the **Requesting Host** and following proper hierarchy of DNS Servers, find the IP Address of the required server.
- Once the IP Address is found, directly query for the IP Address to reach the hostname server.
- While creating a query: 
    - Default `hostname` is given.
    - Set appropriate value to `Type`.
    - Enter the `IP Address` to query for.
    - `Submit` to send the query.
- Keep an eye on the *DNS Reply Messages* to know when IP Address is found.

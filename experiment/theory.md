## **Introduction**  
- The Domain Name System (DNS) is responsible for translating **hostnames** into **IP addresses**.  
- It operates as:  
  1. A **distributed database** implemented across a hierarchy of DNS servers.  
  2. An **application-layer protocol** enabling hosts to query this database.  

## **Distributed, Hierarchical Database**  
- DNS is **distributed** globally across multiple servers to handle scalability.  
- These servers are structured in a **hierarchical fashion**, ensuring efficient resolution of domain names.

## **Types of DNS Servers**  
DNS servers are categorized into three hierarchical classes:

1. **Root DNS Servers**
   - The top-level servers that direct queries to appropriate TLD servers.
   - There are **13 root server clusters** worldwide.

2. **Top-Level Domain (TLD) DNS Servers**
   - Responsible for handling domain extensions like `.com`, `.org`, `.net`, etc.
   - These servers forward queries to authoritative DNS servers.

3. **Authoritative DNS Servers**  
   - Maintain records for specific domains (e.g., `example.com`).  
   - Provide final IP address resolutions for queries.  

## **Recursive vs. Iterative DNS Queries**  
- **Recursive DNS:**  
  - The server takes full responsibility for resolving the query.  
  - It queries other DNS servers on behalf of the client until an answer is found.  

- **Iterative DNS:**  
  - The server provides the best available answer but may refer the client to other DNS servers.  
  - The client must follow up on the next query.  

## **DNS Resource Records (RRs)**  
- DNS servers store **Resource Records (RRs)**, which provide hostname-to-IP mappings.  
- A **resource record** consists of four fields:  
  - **Name** – The domain name (e.g., `www.example.com`).  
  - **Value** – The corresponding IP address or another DNS name depending on the type. 
  - **Type** – The type of DNS record.  
  - **TTL (Time-To-Live)** – The time the record remains valid before refresh.  

## **Common DNS Record Types**  
1. **A (Address Record):** Maps the hostname to it's IP address.  
2. **NS (Name Server Record):** Specifies an authoritative name server for the domain.  
3. **CNAME (Canonical Name Record):** Maps an alias name to a canonical domain name. 

### Reference Books
1. Kurose, J. F., & Ross, K. W. *Computer Networking: A Top-Down Approach*. Pearson.
2. Tanenbaum, A. S., & Wetherall, D. J. *Computer Networks*. Pearson.
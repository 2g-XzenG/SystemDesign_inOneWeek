##  lambda architecture (for big streaming data)

- the batch layer of Lambda architecture manages historical data with the fault-tolerant distributed storage which ensures a low possibility of errors even if the system crashes.
- it is a good balance of speed and reliability.
<img width="400" alt="Screen Shot 2022-04-20 at 11 03 01 AM" src="https://user-images.githubusercontent.com/11614469/164261470-f8864ab9-0c08-4ab0-9982-1877b19c8840.png">


## pull vs push

- pull: a client requests work from a server 
    - pros: stateless
    - cons: not real-time; resource comsuming (e.g., bandwidth)    

- push: a server push work to a client 
    - pros: real-time; less resource comsuming
    - cons: stateful server, not easy to scale (horizontally);  

#### ex1: news feed notification 
- hybrid of pull and push
    - for majority: push
    - for celebrity: pull

 
## write global read local vs write local read global
- write global read lcoal (tradictional): writes are applied to one database and asynchronously replicated to databases across all regions.
- write local read global: storage handled writes locally, then less frequently collect from all data centers to produce the final result.

#### ex1: [facebook live commenting](https://engineering.fb.com/2011/02/07/core-data/live-commenting-behind-the-scenes/)
- write locally + when viewing, fetch the comment out.


## db sharding vs partitioning
Sharding and partitioning are both about breaking up a large data set into smaller subsets. 
- sharding implies the data is spread across multiple computers 
- partitioning is about grouping subsets of data within a single database instance.



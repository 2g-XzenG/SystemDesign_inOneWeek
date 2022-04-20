##  lambda architecture (for big streaming data)

- The batch layer of Lambda architecture manages historical data with the fault-tolerant distributed storage which ensures a low possibility of errors even if the system crashes.
- It is a good balance of speed and reliability.
<img width="400" alt="Screen Shot 2022-04-20 at 11 03 01 AM" src="https://user-images.githubusercontent.com/11614469/164261470-f8864ab9-0c08-4ab0-9982-1877b19c8840.png">


## pull vs push

- Pull: a client requests work from a server 
    - pros: stateless
    - cons: not real-time; resource comsuming (e.g., bandwidth)    

- Push: a server push work to a client 
    - pros: real-time; less resource comsuming
    - cons: stateful server, not easy to scale (horizontally);  

## write local read global vs write global read local

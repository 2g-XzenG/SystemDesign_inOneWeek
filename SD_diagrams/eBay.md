# Design Online Auction/Bidding System (Ebay Auction)

### key points:
  - message queue (kafka): 
      - item_ingest_topic: items that needs to be added into the system
      - item_update_topic: items that have had successfull/un-successful bids in the system

### storage
  - item storage (documentDB): since the items are diverse and do not have a common structure
  - auction storage (redis+sql): redis is used for every item bid with expiration for fast read/write.



<img width="717" alt="Screen Shot 2022-04-19 at 3 31 17 PM" src="https://user-images.githubusercontent.com/11614469/164081259-e645c643-56f2-409b-9906-9e6a160ff30e.png">

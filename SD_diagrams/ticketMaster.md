#  Hotel/Theater Ticket Booking System

### key points

- center service: add to decouple the search/booking/payment service
- kafka cluster:
    - event_digest_topic   
    - event_update_topic

storage
- event storage 
    - documentDB: if the items are diverse and do not have a common structure
    - SQL: otherwise
- booking storage (redis+sql): redis is used for every item bid with expiration for fast read/write.

<img width="729" alt="Screen Shot 2022-04-19 at 9 11 10 PM" src="https://user-images.githubusercontent.com/11614469/164127031-2b58a807-6dfd-4c19-bca4-67a26dbc1ea7.png">

# Top K Songs (hourly & daily update design)

### key points
  - single server small problem -> hashtable + heap: count freq + heap linear scan
  - convert real-time stream problem (unbounded data flow) to bounded: count-min-sketch

### storage
  - HDFS for batch-job updates
  - redis? for real-time updates



<img width="640" alt="Screen Shot 2022-04-19 at 4 09 38 PM" src="https://user-images.githubusercontent.com/11614469/164087983-49bd79db-1feb-40ab-8a05-e8a3bf7de2c5.png">

<img width="591" alt="Screen Shot 2022-04-19 at 4 09 35 PM" src="https://user-images.githubusercontent.com/11614469/164087969-500ad917-51da-46a3-87ab-dd90f4153ff7.png">

<img width="679" alt="Screen Shot 2022-04-19 at 4 42 03 PM" src="https://user-images.githubusercontent.com/11614469/164092120-1ec96c9e-2350-42cb-be23-6e3ee19d5add.png">

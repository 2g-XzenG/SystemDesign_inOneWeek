## Byte Number Sizes
#### The number of zeros after thousands increments by 3.

- Thousands = KB (3 zeros)
- Millions = MB(6 zeros)
- Billions = GB (9 zeros)
- Trillions = TB (12 zeros)
- Quadrilions = PB (15 zeros)

#### Example
- x Million users * y KB = xy GB


## Object Sizes
#### Data
- char: 1B (8 bits)
- char (Unicode): 2B (16 bits)
- Short: 2B (16 bits)
- Int: 4B (32 bits)
- Long: 8B (64 bits)

#### Objects
- File: 100 KB
- Web Page: 100 KB (not including images)
- Picture: 200 KB
- Short Posted Video: 2MB
- Steaming Video: 50MB per minute
- Long/Lat: 8B

#### Lengths
- Maximum URL Size: ~2000 (depends on browser)
- ASCII charset: 128
- Unicode charset: 143, 859


## Per Period Numbers

<img width="400" alt="Screen Shot 2022-04-20 at 4 18 36 PM" src="https://user-images.githubusercontent.com/11614469/164315669-9bc39389-c9fc-4e1c-b426-fad011d90fe3.png">

## Cost of Operations
- Read sequentially from HDD: 30 MB/s
- Read sequentially from SSD: 1 GB/s
- Read sequentially from memory: 4 GB/s


## Systems

#### SQL Databases
- Storage: 60TB
- Requests: 25K per second

#### Cache (redis)
- Storage: 300 GB
- Requests: 100k per second

#### Web Servers
- Requests: 10k per second

#### Queues/Streams (kafka, kinesis)
- Requests: 1k per second
- Throughput: 10 MB/s (Write) / 20 MB/s (Read)

#### Scrapers (colly)
Requests: 1000 per second



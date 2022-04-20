# News Feed/Insagram Feed System

### key points
- fanout on-write
    - news feed is generated in real-time.
    - if user have too many friends -> hot key problem or inactive users -> waste resource
- fanout on-read
    - slow but save resource and mitigate hot key problem   

### storage
- fanout relationship use graph database, such as Neo4j

<img width="735" alt="Screen Shot 2022-04-19 at 10 22 09 PM" src="https://user-images.githubusercontent.com/11614469/164134164-47a295f8-ab9d-4ff0-89c0-bed72d83215e.png">

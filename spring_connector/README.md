
Description Tech Task D3 Cloud: Full-Stack Developer Atlassian Applications
# API Connector #
## Backend ##
Please implement a connector to the Randomuser API service with the following
specification:
- [ ] Develop java standalone application (Connector) (Spring or Spring boot)
- [ ] Connector periodically (JobTask) get data from https://randomuser.me/api and save
into internal database
- [ ] Required Data from https://randomuser.me/api - gender, name, location, email
- [ ] Documentation of API - https://randomuser.me/documentation
- [ ] Implement simple GET controller to get users (Responce - JSON (“countries”:
[{“name”: <country>, users: [{“name”: <userName>, “gender”: <gender>, “email”:
<email>}}]))
- [ ] In case of an unsuccessful synchronization attempt, the Connector should return
data from the last successful synchronization
Connector is configured with simple spring.properties
- [ ] url - API end point
- [ ] userSize - max of users count to get from API
- [ ] period - period of synchronization with API in second
For storage, please use a relational database. The best solution would be any Embedded
DB
There are no special performance or architecture requirements for the Connector.
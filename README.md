# ContactManagement
Contact Management uses WEB API and EntityFramework.
For Dependency Injection I have used Unity Framework.
DAL layer is in separate project , DAL context is mocked for unit testing.
All API responses are HttpResponseMessage which contains status code and data.
For Unit testing MSTest and NSubstitute is used.


To Run/Deploy application:
Extract Zip , Edit connection string and build solution.
Run the Solution.And Use REST calls to perform operations.
GET: Method-Get url - Http:\\localhost:port\Contact.
GET with Id: Method-Get url - Http:\\localhost:port\Contact?id=1.
Post : Method-Post url - Http:\\localhost:port\Contact
  In requset Body: {
        "Id": 1,
        "FirstName": "Mayuresh1",
        "LastName": "Penkar1",
        "EmailId": "m@gmail.com",
        "PhoneNumber": "63636631",
        "IsActive": false
    }.
Put: Method-Delete url Http:\\localhost:port\Contact?id=1.

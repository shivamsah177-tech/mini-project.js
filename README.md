mini project - Count Page Visits Using Express Middleware
1. Create visits.json. Its starting content must be: { "totalVisits": 0,
"routes": {} }
2. Create GET /home, GET /about and GET /contact. Each returns { "success": true,
"Welcome to the <page> page" }.
3. Write one custom middleware that runs for every request and updates the counts in visits.json.
"message":
4. For every visit, increase totalVisits by 1 and the count of that route by 1. A new route starts at 1.
5. Create GET /visits that reads visits.json and returns the statistics.
6. GET /visits itself must not be counted.

   After visiting /home 5 times, /about 7 times and /contact 3 times:
GET http://localhost:5000/visits

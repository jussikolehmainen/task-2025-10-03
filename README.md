# Assignment for Full Stack Engineer at Yellow Method

## Intro
- You have 1 hour to complete as much as possible.  
- Fork the https://github.com/vercel/next.js/tree/canary/examples/blog-starter repo, clone it locally, and work on your fork.
- Use AI assistant of your choice when instructed to do so.

## Tasks

### 1. Explore the code
- Explore and explain the most important parts of the code.
- How are posts loaded into frontend? What other ways would there be? What are the differences?
- Start the app and make sure it works.
- Remove existing blog posts and generate 20 new ones with AI about a topic you are interested in.

### 2. Implement search feature (use AI assistant)
- Add a search bar to the top of the front page that can be used to find blog posts.
- Explain what changes the AI assistant made.

### 3. Improve search algorithm (manual coding)
- Move search algorithm to `lib/search.ts` and implement it with the following requirements:
  - Return only posts where the title or content matches the query.
  - Matching must be case-insensitive.
  - Rank results so posts with the query in the title appear before those with matches only in the content.
- Bonus: use fuzzy matching and allow for spelling mistakes.

### 4. Track visitor counts (use AI assistant)
- Add an API route that increments a view count every time a blog post is opened.
- Add /analytics page that displays total number of visits.

### 5. Improve analytics algorithm (manual coding)
- Show a list of five most viewed blog posts together with view counts.
- Show total views by date for the past week.
- When the app starts, generate random views data to test these.

### 6. Discussion (verbal)
- Deployment
  - How would you deploy this app on AWS as MVP?
  - Which services would you use and why?
- Authentication and Authorization
  - How would you implement simple authentication and authorization?
  - How would you enforce roles (admin vs normal users)?
- Persistence
  - How would you persist view counts instead of keeping them in memory?
  - Which database or storage would you choose, and why?
  - Can you run into race conditions with your chosen approach?
- Scaling
  - How would you scale the search if there were millions of posts and users?
  - How would you make sure latency is low for users all over the world?
- Security
  - What common web security risks would you consider (XSS, CSRF, SQL injection, etc.)?
  - How would you protect against bots inflating view counts?
- Monitoring and observability
  - What metrics or logs would you add to track errors and performance?
  - How would you set up alerts for failures?
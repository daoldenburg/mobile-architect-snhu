# mobile-architect-snhu
Coursework for my Mobile Architecture &amp; Programming course at SNHU

Q: Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?
A: The requirements for this inventory app were:
  (1) a database to store user login information and inventory items, 
  (2) app should display inventory items in a grid layout, 
  (3) user should be able to perform all "CRUD" operations (create, read, update, delete) on stored inventory items, and 
  (4) user should be able to login or create an account at a login screen.
  
  I identified two primary categories of potential users: 
    (1) small business owners/employees who seek a simple and free inventory management tool, and 
    (2) people who are moving or storing a large number of personal belongings, and want a free and convenient tool to track them.
  
Q: What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?
A: The app required a login screen, a "main inventory" screen, an "item detail" screen, and a database. The goal of the UI design was to create a very minimal yet intuitive interface, that makes it clear to the user what options are available and how to use them. Note that the current UI design is not finalized. Despite its unfinished state, the UI achieves its core goal of putting functionality first, with simple intuitive menus that operate as expected.

Q: How did you approach the process of coding your app? What techniques or strategies did you use? How could those be applied in the future?
A: I chose to approach the coding/development process by combining, customizing, and building upon design patterns that I had used before or knew were functional. For example, the Room Persistence Library enabled powerful and flexible database access via DAO (data access objects). The singleton pattern was effective in enforcing database uniqueness and accessibility across the app. In the future I hope to use this technique of a singleton Room-backed SQLite database in many applications, for example as a means of storing data in mobile games.

Q: How did you test to ensure your code was functional? Why is this process important and what did it reveal?
A: I tested continuously and iteratively throughout the design process. Though my process was not rigidly structured, each testing iteration generally consisted of two phases: a phase of functional testing for the established application requirements, and a phase of trying whatever I could to break the app or cause an error, an approach Alejandro Maderna described as "destructive creativity" (Maderna, 2016).

Q: Considering the full app design and development process, from initial planning to finalization, where did you have to innovate to overcome a challenge?
A: I initially planned to implement "in-line" editing for inventory items, but encountered difficulties with dynamically assigning an onClickListener to Buttons within RecyclerView items. I was faced with the decision of cutting the feature, or risking failure to meet my deadline. I made the choice that maximized the odds of delivering a functional application on schedule, and cut the feature from the release. I followed up on this decision by redesigning the UI -- so that it no longer depends upon or implies the removed feature, and also to double-down on the minimalist approach that the removal of in-line controls encouraged. Ultimately I think the resulting UI is more successful than the original.

Q: In what specific component from your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?
A: I am particularly happy with the implementation of hash cryptography for user passwords. Application and data security is incredibly important, so although the project assignment did not explicitly require it, I took the extra step to implement the industry-standard SHA-256 hash algorithm for user passwords. I believe my implementation to be secure and effective.

----------
References
----------

Maderna, A. (2016, April 29). Psychology of Testing. Retrieved October 25, 2020, from https://web.archive.org/web/20160506115640/https://www.kanoah.com/blog/psychology-of-testing/

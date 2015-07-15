## Misc Job Market Notes

Busy week for me. I can probably come by a/A again next Mon or Tuesto to talk shop again if it'll be helpful. 

## General advice: 

+ Focus on either front-end or back-end, not both. Take a few weeks (depending on how much time you are able go without a job), and go hard at the field that you're targeting first. If things don't go well, you can always switch focus. Why don't go full-stack?

    * Companies *do not want to train you*. They want devs who will be productive as early as possible - quick learners are a plus insofar as you can get ramped up to being prouctive sooner, but they will almost always prefer people with existing skills.  Any training they have to provide is a fixed-cost that they might be willing to tolerate depending on their estimate of your potential upside and how quickly they need to move. Large companies have more resources and are more patient. Small, high-quality startups are the most impatient. Small sketchy startups might take a chance on you, but you are also taking a chance on them. 

    * Whether you're straight front-end or back-end, you're going to be drinking from a fire-hose from day one as you rush to learn a new language, a new framework, a new database, your company's gitflow, its continuous-integration system, and a large codebase, none of which you have written. The move from a/A to a job is a move from playing entirely in your own sandbox, spending most of your time writing code, to cooperating on a project with other people, spending (initially) most of your time reading code and understanding an architecture that you haven't built. If you are full-stack to start, you have a represent an even greater training cost for your employer. 

    * Splitting focus b/w front-end and back-end makes you a less competitive candidate for the many positions that are single-focus. Even if you are pretty good at both, you will be competing with people who are excellent at one. 

    * That said, entry-level full stack positions are definitely around. If your heart's set on full-stack, you can make it work. Your initial position also isn't going to limit what you can work on forever. A number of my friends who started front-end have since moved on to implementing some server endpoints as well. Once you have a job your position can be somewhat fluid.  
    
+ You should aim to have done ~5 on-sites and have ~2 offers by the time you have your on-sites for companies you care about. Interviewing is a learnable skill - but you have to put in the time discovering your weaknesses and building confidence through actually doing it live, whiteboarding isn't enough. Don't feel pressured to accept the offers you get from the mediocre companies you interview at initially. The better people at a/A have placed really well. If you have enough enough money to finance a longer job-search, you'll be able to hold out for a very strong starting position. 

## Back-end advice
Usefulness of different concepts in algorithms and data structures follows a power law. 20% of the concepts account for 80% of the value. It's probably even more skewed than that: data structures tend to be much more useful than algorithms (much of the transition from novice to intermediate programmer consists of learning the myriad ways in which hashmaps can make your life much easier)

Which to focus on? 
  + Arrays you should already get. There really isn't too much to know here. It's a useful exercise to figure out how dynamically resizing arrays are implemented, and why insertion into a dynamic array is still ammortized O(1) even though you have to do a costly O(n) operation from time to time (also useful to understand what 'ammortized')

  + Hashmaps. Extremely important. Know both the hash-table (array) implementation and the treemap (I prefer treemap, but ymmv). Order of efficiency in many algorithms typically goes: brute force > simple solution using hashmaps > sophisticated solution using dynamic programming. Much of the time a hashmap solution is enough to make the interviwer happy. I haven't had to explicitly use dynamic programming once in my 8 months on a fairly technical back-end heavy project.  

  + Trees. Extremely important. The omni-data structure. Using trees as a primitive, you can basically implement any conceivable data structure. Know your DFS and BFS (do them once, and know them well enough to remind yourself of how they work if they happen to get sprung on you in an interview. Pretty easy to remember. Identical implementation but one uses a stack, the other a queue. Another example of data structures reigning supreme). Implement all the collection algorithms on these (`each`, `reduce`, `select`, `map`, etc...). Trees are awesome. 
  
  + Graphs. Situational. Learn a simple representation in your language of choice, then BFS, DFS, and least-cost path and call it a day. 





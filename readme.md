## Misc Job Market Notes

These are pretty rough. I'll continue to update this. Probably going to split this up into separate more focused parts.

Busy week for me. I can probably come by a/A again next Mon or Tues to to talk shop again if it'll be helpful.

## General advice:

+ Focus on either front-end or back-end, not both. Take a few weeks (depending on how much time you are able go without a job), and go hard at the field that you're targeting first. If things don't go well, you can always switch focus. Why don't go full-stack?

    * Companies *do not want to train you*. They want devs who will be productive as early as possible - quick learners are a plus insofar as you can get ramped up to being prouctive sooner, but they will almost always prefer people with existing skills.  Any training they have to provide is a fixed-cost that they might be willing to tolerate depending on their estimate of your potential upside and how quickly they need to move. Large companies have more resources and are more patient. Small, high-quality startups are the most impatient. Small sketchy startups might take a chance on you, but you are also taking a chance on them.

    * Whether you're straight front-end or back-end, you're going to be drinking from a fire-hose from day one as you rush to learn a new language, a new framework, a new database, your company's gitflow, its continuous-integration system, and a large codebase, none of which you have written. The move from a/A to a job is a move from playing entirely in your own sandbox, spending most of your time writing code, to cooperating on a project with other people, spending (initially) most of your time reading code and understanding an architecture that you haven't built. If you are full-stack to start, there is even more that you don't know, and you represent an even greater training cost for your employer.

    * Splitting focus b/w front-end and back-end makes you a less competitive candidate for the many positions that are single-focus. Even if you are pretty good at both, you will be competing with people who are excellent at one.

    * That said, entry-level full stack positions are definitely around. If your heart's set on full-stack, you can make it work. Your initial position also isn't going to limit what you can work on forever. A number of my friends who started front-end have since moved on to implementing some server endpoints as well. Once you have a job your position can be somewhat fluid.  

+ You should aim to have done ~5 on-sites and have ~2 offers by the time you have your on-sites for companies you care about. Interviewing is a learnable skill - but you have to put in the time discovering your weaknesses and building confidence through actually doing it live, whiteboarding isn't enough.

+ If you are considering both front-end and back-end, go for back-end first. Should you later decide to switch focus to front-end, the skills you've practiced for back-end will still be helpful in front-end interviews. Front-end skills are much less applicable in back-end interviews.

Most importantly:
#### Don't feel pressured to accept the offers you get from the mediocre companies you interview at initially. The better people at a/A have placed really well. If you have enough enough money to finance a longer job-search, you'll be able to hold out for a very strong starting position.

## Front-end advice
Front-end interviews are much more structured and have a much tighter connection with your actual on the job responsibilities. At your new company, you are going to be trying to make polished user-interfaces, probably using some single-page app javascript MVC framework. If you have a portfolio of polished web apps, this is an accurate costly signal of your ability to do the same when on the job.

What to focus on?

Build your portfolio - more for practice than for show and tell. Get a single extremely good example web app to sell your skills to employers. Bring your laptop to interviews, ideally with your own reliable internet connection tethered through your phone (or however). Many of your interviewers probably won't have taken a look at your app prior to meeting you. Having it on hand to demonstrate what you've built can make a really good impression.

Learn another major framework. React is an interesting option and a fairly different paradigm from Backbone. Angular is much more prevalent, but pretty opinionated and heavy-weight (30k plus of source code vs the ~1600(?) of Backbone).

Learn a Key-Value store. Redis seems popular with front-end folks.

Understand all the performance optimization wizardry. I'm not front-end so I don't really know anything about this. I've heard good things about:

http://chimera.labs.oreilly.com/books/1230000000545/

Ilya Grigorik is a badass. He is basically the [human manifestation of high-performance](http://lh6.ggpht.com/f_0W8h__3G99CWTjnMjD8BUKm7yp2-wJyApLtTwFoFtlal2ULf_JgHIsOQq2NiYfKOdMlXlMHDKNo5XVZLs=s0).

## Back-end advice
It's hard to interview for back-end positions for new hires. The best predictor of back-end competency is having worked on a high-quality team building a distributed system. Obviously new hires won't have experience with this as there's a minimum scale of project size before it's reasonable or useful to apply the sort of tools that a large project needs.

##### Interviewing is a game. Both (conventional) employers and applicants know what the metric is. The content of the interviews is in large part arbitrary: it could be a competition of your knowledge of the linguistic properties of Esperanto. Whiteboarding data structures and algorithms is a learnable skill. The point of the competition is to provide a costly signal of how capable you are of acquiring arbitrary technical skills when required to. Many times on the job, you will have to learn some codebase or difficult bit of software arcana that is not terribly interesting to you, but is required to get another task done.

You can learn to do well at the interview game. If you want to target a medium-to-large company (and especially for the top tech companies), you have to put in the time. If [Google rejected the creator of Homebrew for not being able to reverse a binary tree](https://twitter.com/mxcl/status/608682016205344768?lang=en), they will happily reject a bootcamp grad for the same.

The upside is that not all of the preparation is a sunk cost. Data structures are beautiful and extremely useful. Dynamic programming, while also beautiful, is not used all that much.

Usefulness of different concepts in algorithms and data structures follows a power law. 20% of the concepts account for 80% of the value. It's probably even more skewed than that: data structures tend to be much more useful than algorithms (much of the transition from novice to intermediate programmer consists of learning the myriad ways in which hashmaps can make your life much easier)

Which to focus on?
  + Arrays you should already get. There really isn't too much to know here. It's a useful exercise to figure out how dynamically resizing arrays are implemented, and why insertion into a dynamic array is still ammortized O(1) even though you have to do a costly O(n) operation from time to time (also useful to understand what 'ammortized')

  + Hashmaps. Extremely important. Know both the hash-table (array) implementation and the treemap (I prefer treemap, but ymmv). Order of efficiency in many algorithms typically goes: brute force > simple solution using hashmaps > sophisticated solution using dynamic programming. Much of the time a hashmap solution is enough to make the interviwer happy. I haven't had to explicitly use dynamic programming once in my 8 months on a fairly technical back-end heavy project.  

  + Trees. Extremely important. The omni-data structure. Using trees as a primitive, you can basically implement any conceivable data structure. Know your DFS and BFS (do them once, and know them well enough to remind yourself of how they work if they happen to get sprung on you in an interview. Pretty easy to remember. Identical implementation but one uses a stack, the other a queue. Another example of data structures reigning supreme). Implement all the collection algorithms on these (`each`, `reduce`, `select`, `map`, etc...). Trees are awesome.

  + Graphs. Situational. Learn a simple representation in your language of choice, then BFS, DFS, and least-cost path and call it a day.

## Resources

##### Persistence
Understand the difference between relational databases and some of the more popular non-relational dbs. There are many, many no-sql db options. I'd recommend just focusing on a key-value store as they tend to have an excellent fit for situations in which relational dbs don't work well. There are many KV stores. I'd recommend looking at CouchDB. Extremely simple to get set-up, and an incredible interface. You communicate with a CouchDB instance purely by sending HTTP requests, so by default it abstracts away where the location of where the db lives: it could be on localhost, it could be on a cluster - it doesn't matter.
NoSql distilled by Martin Fowler is a really good primer on some of the different dbs. I haven't watched this talk by him, but probably legit stuff: http://www.youtube.com/watch?v=ASiU89Gl0F0

#### Distributed systems
Related to above.

The problem in brief: your single relational database can't scala, so you move to a distributed KV store with nodes A, B, and C. A client makes an update to some key-value pair in A. Milliseconds afterwards, another client makes reads the same key-value pair from B. Given that the write was made at another node, how does A update B and C as to the change of state? What version of the pair will the client read from B? What are some of the tradeoffs we face, and what are some use-cases in which we'd make different decisions? (this is what the CAP theorem deals with: "Consistency, Availability, Partition-tolerance: pick two")

To get started, the Jepsen series of talks by Aphyr stress-testing various databases are excellent:
http://www.youtube.com/watch?v=QdkS6ZjeR7Q

I'll poll my team for some more resources here.

# Fancy algorithms (aka dynamic programming)
To recap above, for many algorithm problems the order of hierarchy of "sophisticatd" or performant solutions is loosely:
  + Naive: brute force
  + Pretty good: use hashmaps
  + Fancy, best possible performance: dynamic programming

More to come on dynamic programming. Probably in a separate section, this is getting fairly long.

## THE ROBBER PROBLEM (aka the simplest possible dynamic programming problem)
I went over this quickly when I first came by to talk to you guys like 2 (3?) months ago.

The problem: You have an array of houses. Each house holds some amount of loot. If you rob a house, you can't rob its neighbors (i.e. robbing house at index `i` means you can't rob house `i - 1` or `i + 1`)

The problem is to choose a collection of houses to rob such that you maximize the overall loot.

We'll start off with brute force and come back to the clean solution later:

```
# in ruby:
houses = (1..10).to_a.shuffle

def maxLoot(houses)
  subsets(houses)
    .filter { |neighborhood| no_adjacent_houses?(neighborhood) }
    .map { |neighborhood| total_loot(neighborhood) }
    .max
end
```
Implementations aren't there, but that's the structure of the problem.

For bonus, here's a possible scala version:
```
type House = Int
type Neighborhood = List[House]

val houses: Neighborhood = shuffle(1 to 10).toList

def maxLoot(houses: Neighborhood): Int = {
  houses
    .subsets
    .filter(noAdjacentHouses)
    .map(totalLoot)
    .max
}

// with some type signatures of TBD methods:
def noAdjacentHouses(houses: Neighborhood): Boolean = {...}

def totalLoot(houses: Neighborhood): Int = {...}
```
Types are the best.

# Learning Log DLXV82
(p.s. looks better in dark mode, always does)
# Part 1 *DurHack 2022*

### *Project: [Spoil Wordle](https://github.com/sbarnham/spoilWordle)*

When starting this practical I felt lost, I'm sure a problem many faced. It was only after DurHack that I knew what I wanted to achieve. 

I am breaking this project into parts in attempt to emphasize the importance hackathons have in gaining the experience of actual developing environments. Having interned at a start up I saw the ordered chaos that developing can be and being at a hackathon made me feel as if I was starting my own. 

>In my opinion a hackathon should be a mandatory aspect of this project and where better to start then DurHack. 

### <span style="color:red"> *My Guide to Hackathons ([DurHack](https://durhack.com/)):*</span>

1. Read [Challenges]((https://hack.mlh.io/prizes)) Before Hand

    For first time hackers, there is a list of challenges that will be released before every hackathon. This is a must read before competing.
![DurHackTeam](public/PrizeList.PNG)

1. Build Your Team Beforehand 
    * Saves Time
    * Allows you to build with diversity of skill in mind. Something you will be limited doing, building your team at events.
> You will spend a lot of time together. Get people work well and get along with.
1. Rely on Sponsor Representatives
    * use Hackathons/Sponsors resources and engage with the Representatives. They are there to help! I found the lectures the most informative and helpful.
1. The Demo
    * Let the best speaker present don't default to the group leader.
        * Explain why you made the project, the value it adds. 
        * Practice demoing to your group and choose the teammate that demos the best.

### <span style="color:Red"> *Hackathon Tips (DurHack):*</span>
* Rest before, these are long events don't burnout.
* Go in open minded, **your plans will change**.
* Choose a personal objective. 
    
>It's okay if it changes. I found this very useful especially when trying to learn something when there are so many options.

* Make a list of what your project must do and focus on core functionality before adding extra.

### <span style="color:Red"> Motivation for our Hack:</span>

All businesses require [communication channels email, text messages, phone calls](https://www.health.org.uk/sites/default/files/Communications-channels.pdf). As annoying as it is to call Amazon and select the 50 different options given to you before you can finally speak to someone, there is a reason businesses do this. It is incredibly efficient. These communications are not specific to customers, within a business it is also imperative for an efficient work environment. It is important to know how these communications can be done autonomously as it is **unavoidable**. This was my personal goal for DurHack.

<hr>

### <span style="color:Red"> Background knowledge: </span> 

Before starting with API's such as [Twilio](https://www.twilio.com/) or [alternatives](https://rigorousthemes.com/blog/best-twilio-alternatives/). You should attempt to work with more basic API's. I recommend [Gmail](https://developers.google.com/gmail/api/) as a good starting place before you attempt to jump into more complex combinations of communications. This is where I started and it is a route I recommend. Start by sending basic emails and categorizing emails received by their content/subject. [Tutorial using nodemailer](https://www.youtube.com/watch?v=vgk7Yio-GQw) or [JavaScript Quickstart](https://developers.google.com/gmail/api/quickstart/js#python-3.x). 

<hr>

### <span style="color:Red"> Spoil Wordle: </span>

API's can differ drastically, some even having their own local languages. Twilio has [TwiML](https://www.twilio.com/docs/glossary/what-is-twilio-markup-language-twiml). Using this we were able to incorporate much greater functionality into our project [Spoil Wordle](https://github.com/sbarnham/spoilWordle). A website that allows you to enter phone numbers then play [Wordle](https://www.nytimes.com/games/wordle/index.html) (a word guessing game) with the solution being sent to entered numbers via SMS's and call's. 

Using Twilio we were able to host Mp3's ([example](https://altaudio-9871.twil.io/3.mp3)) splicing them to generate unique and *human sounding* phone calls to each of the entered numbers. We created a response tree in TwiML reading and replying to messages sent to the phone numbers we controlled though Twilio. This would allow customers to access information they require, contact relevant company members able to help as well as other uses.

<Checking phone numbers>

Top 3 & Funniest Hack   | Spoil Wordle Team
-------------  | -------------
![DurHackWinners](public/DurHackWinners.jpg) | ![DurHackGitHubAccs](public/DurHackGithubAccs.jpeg) 

![DurHackTeam](public/DurHackTeam.jpg)

# Interlude: *code quality*

One of the big issues I faced in the first practical of programming black was [code quality](https://www.perforce.com/blog/sca/what-code-quality-overview-how-improve-code-quality). I did not realize how important this issue was until DurHack.

Often I would reach a point where a piece of code achieving what I wanted, but when others had to work with that code they would get lost. Much of my code could have be called ***spaghetti code***, due to this approach. I would think about how to solve the problem and often not putting enough thought into [issues like](https://www.youtube.com/watch?v=k238XpMMn38).

1. Later development
    * Changing functionality
    * Adding extra functionality
    * Upgrading efficiency

> This would mean even small changes of code or it's objective would take disproportionately long with simple tasks becoming complex.
2. Working with others
    * Understanding others code
    * Others understanding my code
    * Collaborating efficiently
2. Code testing
    * Finding Bugs
    * Fixing Bugs without having to re-write
        * Having bugs disguise other bugs
    * Code reliability
> This proved the most infuriating of the issues and I believe it is was my weakest link. This proved a meaningful motivator in improving my codes quality.

Once you have sat with a issue for a time you gain greater insight into it. For others developing with you fully understanding of every single line is arduous and wastes time. Especially in situation where time is a main factor such as hackathons.

<hr>

## <span style="color:red"> Fixing the Issue: </span>

* The most effective strategy is to be hard on yourself. Step back and try and read your code as if you've just seen it for the first time.

* [**Use informative comments in your code,**](https://stackoverflow.blog/2021/12/23/best-practices-for-writing-code-comments/) make sure the comments describe not only the line but sometimes also surrounding lines.

* If there is a operation which is being used repeatedly throughout the code make a function for it. This helps in 2 ways.
    1. Decreases the total lines of code making it quicker to read and understand.
    1. Helps identify where issues in the code lie.

<hr> 

## <span style="color:red"> Still need help?: </span>

* [How To Write Better Code](https://www.youtube.com/watch?v=g2nMKzhkvxw)
* [Spaghetti Code](https://www.geeksforgeeks.org/spaghetti-code/)

The good news is that this issue can be fixed. Though this is not something that you will ever truly be done with as your code quality will continue to improve always. There is a large initial boosts that can be gained following these basic principles. You will thank yourself for learning the skill of developing with good code quality.

# Part 2: Data Storage
### *Project: [ScheduleYouLater](https://github.com/Fa41m/ScheduleYouLater)*

### <span style="color:Red"> Motivation for our Hack: </span>
Information technology is just that **Information**. Learning how to store, organize display information is a must for all developers. It is also something I wish was focused on more. I particularly wanted to look into databases one of the most efficient way to store and organize large quantities of data. 

And how better to develop these skills than with a calendar project where information must be sorted, added/edited and displayed efficiently and in a very specific format (according to the date the entry is in reference to)

<hr>

### <span style="color:Red"> Background knowledge: </span>

Databases are the most efficient way of storing records and information. When dealing with databases it is important that you learn [SQL](https://en.wikipedia.org/wiki/SQL), the industry standard. SQL is a structured database query language that deals with managing data within a relational database management system. A system where multiple databases are linked together by a primary key. These are the best resources I found when learning SQL and the ones I used.

### introductions to SQL:

* [Storing IoT Data in a database](https://techcommunity.microsoft.com/t5/educator-developer-blog/storing-iot-data-in-a-database/ba-p/1183534)
* [w3schools SQL tutorial](https://www.w3schools.com/sql/default.asp)
* [SQL for Beginners Tutorial](https://www.youtube.com/watch?v=h0nxCDiD-zg)
* [TOP-70 MOST IMPORTANT SQL QUERIES IN 2022](https://bytescout.com/blog/20-important-sql-queries.html)

### Website using databases:
* [SQL Database with Only HTML5 and JavaScript](https://www.youtube.com/watch?v=QExydkuuE30)

The final draft of this project ended up using JSON files instead of databases as we found a very succinct and clean way of storing the data. This was because we felt the amount of data we stored was not large enough to warrant the use of databases. Though we made a working beta using databases.

### introductions to JSON:

* [Working With JSON Data in Python](https://realpython.com/python-json/#a-real-world-example-sort-of)
* [Introducing JSON](https://www.json.org/json-en.html)
* [Coding A Calendar App In Plain JavaScript](https://www.youtube.com/watch?v=m9OSBJaQTlM) 

### Cookies

Cookies are something else that must be considered when web developing. General client side storage used to be done using cookies. This is no longer done as it is inefficient. Cookies can be very useful when web developing.

### Introductions to Cookies:

* [Using HTTP cookies](https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies)

# <span style="color:Red"> Conclusion </span>
There are multiple small projects I undertook during this project eg. a bot auto signing up to college formals. This more broad approach meant I had two skills I was developing, as someone not having done A levels this was the route I decided to take. Focusing data storage and communications led me to gain more than If I had only focused one.
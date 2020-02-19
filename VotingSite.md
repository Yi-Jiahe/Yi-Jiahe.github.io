# CN Yang Executive Committee Voting Site

In my second year of university, I was commissioned to develop an online voting system for the CN Yang Scholars Progamme, which would allow them to move away from physical ballots to an electronic voting system. The system was developed to cut down on the paper used for the physical ballots, as well as reduce the logistics invovled. The electronic voting system would also allow year 3 and 4 scholars on their overseas exchange and final year projects to have a say.

For this project I made use of python and the flask package to generate the site and handle the HTTP requests. SQLalchemy was used for the database.

To limit each voter to one vote, a 5 letter case-sensitive one-time password was emailed to each voter, which was then deleted when it was used or replaced. I implemented a running key cipher in the python code to encode the used passwords, as well as a running key cipher in a vba script, used by a moderating party to ensure all the votes were valid, while ensuring annoynimity. In this way, all votes were accountable to a voter, but no one party would have both the voter's one time password and their vote.

On the voting day, the source code was uploaded to github and hosted as a heroku app running a postgres server.


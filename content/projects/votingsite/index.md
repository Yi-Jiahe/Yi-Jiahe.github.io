# CN Yang Executive Committee Voting Site

In my second year of university, I was commissioned to develop an online voting system for the CN Yang Scholars Club, which would allow them to move away from physical ballots to an electronic voting system. The system was developed to cut down on the paper used for the physical ballots, as well as reduce the logistics involved. The electronic voting system would also allow year 3 and 4 scholars on their overseas exchange and final year projects to have a say.

For this project I made use of python and the flask package to generate the site and handle the HTTP requests. SQLalchemy was used for the database.

To limit each voter to one vote, a 5 letter case-sensitive one-time password was emailed to each voter, which was then deleted when it was used or replaced. I implemented a running key cipher in the python code to encode the used passwords, as well as a running key cipher in a VBA script, used by a moderating party to ensure all the votes were valid, while ensuring anonymity. In this way, all votes were accountable to a voter, but no one party would have both the voter's one time password and their vote.

On the voting day, the source code was uploaded to GitHub and hosted as a Heroku app running a Postgres server.

## Testimonials

> The electronic voting system has improved the efficiency of our voting process significantly. It not only allowed us to tabulate the results within minutes, but also allowed voters who were overseas to participate in the elections via the easy to access portal. The encryption also ensures we are able to meet the same demands of accountability and anonymity as the traditional system. Most importantly for us, we wanted to reduce the amount of paper waste produced from printing over 200 traditional voting pamphlets. The system has already been handed down to the next batch of scholars in the committee and works amazingly.
- Sowmya Srinivasan Iyer, Vice-President 11EC
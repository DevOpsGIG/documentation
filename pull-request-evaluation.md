# Principles for Evaluating Pull Requests

### Everything should be well-tested with automation

The code doesn't have to be 100% covered by unit tests. But most of the 'happy path' do.

Pull requests with large amounts of new; untested functionality *shall not pass*.

### PRs that are just submitted without any prior communication will likely be summarily closed

First of all, stick on the planning for the current iteration.
Probably there's already a lot of delicious tasks waiting for you in the project's Kanban. Always follow the plan.

If you notice that some functionality should receive a fix; be re-engineered or if you found the opportunity to implement a beautiful piece of code as new feature. Open an issue and bring the discussion for the daily meeting.

Communicating intentions and stating problems in a proper manner is the best way to design a better solution for the task, but also, to avoid wasting development time implementing unnecessary stuff, and duplicated work.

### Maintainabilty > completeness

Do not add something that increases maintenance burden unless it is a very compelling functionality or an obvious bugfix. No one can maintain a system that it's not fully understood.

Keeping things lighter and cutting off edge cases rather than adding [technical debt](http://martinfowler.com/bliki/TechnicalDebt.html) is the way to go.

### Don't commit random stuff

The PR for your fix or feature implementation should only contain code related to that particular and well-defined issue.

Do not try to fix or change random things that are not directly related to your task. Another developer working on a different problem could stumble on the same stuff and, bang! Duplicated unplanned work.

Remember, open an issue and talk with the team.

### Make it small

A small and focused Pull Request is what you want. This is the mantra!

You have spent days obscured by the clouds of the problem that you were trying to solve.

Now, that you can see the sunlight, and the food and the wine can taste again, you want to merge your implementation and look ahead for your next dopamine shot.

Now, from the reviewer perspective:

Some people like to review code as the first thing in the morning when they get to the office. Others, do that immediately everytime the PR alert pops in the channel. The point here is that no one would like to find an extensive list of Pull Requests to review, each one with a huge amount of code that they didn't write, and they don't understand. Because since you've fit so much code in the same change, neither yourself can objectively describe what is in there.

Keep your implementations concise, and cater for the people which will review your work.

### Be logical with your commits

Well, be logical with your commits.

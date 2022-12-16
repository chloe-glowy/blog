On my [dev.to](https://dev.to/chloeglowy) account, I'm going to write about a project I'm working on, called Dandelion. 

The purpose of this post is to give an overview of what Dandelion is, so I can reference it in other posts. The source code for this post is on GitHub [here](https://github.com/chloe-glowy/blog/blob/main/dandelion/what-is-dandelion.md). The source code for Dandelion is on GitHub [here]([todo](https://github.com/chloe-glowy/dandelion)).

Dandelion is: **A mobile web application for collaboratively helping people who need things.**

Specifically, it was originally developed for a group of people (volunteers) who visit people who are living outside (residents) and offer help. Residents ask for things like batteries, tents, boots, propane stoves, etc.

When a resident tells a volunteer that they need something, the volunteer can record the request on Dandelion. Currently, in the code, we refer to this recorded request as an **AidRequest**.

The app hasn't been used by actual volunteers since about October 2022, and I'm not actively promoting it for real-life use.

I'm using the app as a pet software project to which I can apply new concepts that I learn.

I wrote the original code very hastily, so there are a lot of improvements I can make now.

Here's a non-exhaustive list of things I'm considering learning by applying them to Dandelion:

1. [Clean Architecture](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)
2. Different authentication methods, e.g., sign in with Google, email a magic link
3. Multi-Factor Authentication
4. Protection from DDOS
5. Protection from XSS
6. Serving static assets through a CDN
7. Using spritesheets
8. Adapting the app to be open to the public, rather than allowlist-only

Here's a mostly-exhaustive list of all the features that Dandelion currently has, as of 12/15/22:

1. A volunteer can access the app on the web. 
   1. I'm technically using React Native, so Android and iOS are kind of supported, but I haven't been regularly building or releasing to these platforms, and do not plan on doing so. In fact, I want to move to web-only.
2. Account management:
   1. A volunteer can create an account using an email address and password, if their email address is on the allowlist
   4. A volunteer can log out and sign in again with their password
   5. If a volunteer forgets their password, they can get an email with a password reset link
   6. A volunteer can change their Display Name, which is what other volunteers see associated with their activity in the app
3. Aid Request List:
   1. A volunteer can see a list of all the Aid Requests that are currently open and that they have permission to see. Permission is based on whether the Aid Request is associated with a Sharing Group that the user is a member of.
   8. A volunteer can toggle between seeing Open and Closed Aid Requests.
   9. A volunteer can filter to view only the Aid Requests that they are working on (or that they worked on, if they are looking at closed requests)
   10. A volunteer can search for Aid Requests. The text they enter is compared against prefixes for all the text fields in each Aid Request, as well as the Display Names of each other Volunteer that is associated with the Aid Request.
   11. Each item in the list displays what is needed, who it is for, and the most recent activity on the request
   12. Requests are sorted by how recent the most recent activity was, newest to oldest
   13. A volunteer can tap the Three Dots icon on any Aid Request to see the Quick Actions drawer
   14. A volunteer can tap on any Aid Request to navigate to the Aid Request Detail page for it
4. Quick Actions
   1. todo
5. Aid Request Detail page
   1. todo
6. Creating Aid Request(s)
   1. todo

Here are some more features I'd like to implement:



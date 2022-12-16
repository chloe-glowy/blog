I'm going to write a series of posts about a project I'm working on called Dandelion. 

The purpose of this post is to give an overview of what Dandelion is so I can reference it as context in other posts.

Dandelion is: 

## A mobile web application for collaboratively helping people who need things.

Specifically, it was originally developed for a group of people (volunteers) who visit people who are living outside (residents) and offer help. Residents ask for things like batteries, tents, boots, propane stoves, etc.

When a resident tells a volunteer that they need something, the volunteer can record the request on Dandelion. Currently, in the code, we refer to this recorded request as an **AidRequest**. Volunteer can mark themselves as working on an aid request, mark it as complete, comment on it, tag other volunteers, and more. In a future post, I'll describe the features in more detail.

The app hasn't been used by actual volunteers since about October 2022, and I'm not actively promoting it for real-life use as of 12/15/22. In the future, when the app supports more features, this may change.

For now, I'm using the app as a pet software project to which I can apply new concepts that I learn.

Here's a non-exhaustive list of things I'm considering learning by applying them to Dandelion:

1. [Clean Architecture](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)
2. Different authentication methods, e.g., sign in with Google, email a magic link
3. Multi-Factor Authentication
4. Protection from DDOS
5. Protection from XSS
6. Serving static assets through a CDN
7. Using spritesheets
8. Adapting the app to be open to the public, rather than allowlist-only
9. Unit testing under Clean Architecture, using a test API
10. React testing
11. Using different kinds of databases (it currently only supports MongoDB)

I don't know if anyone is going to read this, but if you do, feel free to comment other things I could try learning with this project :)

In my next post, I'll describe the existing features of Dandelion and some features I want to add to it next. After that, I'll dive into my current project, which is refactoring the backend to use Clean Architecture. 

All my posts will be on [GitHub](https://github.com/chloe-glowy/blog/tree/main/dandelion) and my [DEV page](https://dev.to/chloeglowy). The source code for this post is on GitHub [here](https://github.com/chloe-glowy/blog/blob/main/dandelion/what-is-dandelion.md). 

The source code for Dandelion is on GitHub [here](https://github.com/chloe-glowy/dandelion).

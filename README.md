# Front export

**:hand: Heads up! This code uses the Front API V1, which is deprecated. @niklasravnsborg took this project further and created a Front API V2 compatible version: https://github.com/niklasravnsborg/front-export :tada:**

**This repository is no longer maintained.**


Little export script for exporting all conversations in a Front inbox, using the Front API V1.

When using the awesome [Front App](https://frontapp.com/), you want to export all conversations in an inbox. For example, for backup purposes.

Three environment variables are needed:

- FRONT_APP_ID: your App ID (see [Front API docs on authentication](http://docs.frontapp.com/docs/public-api#authentication))
- FRONT_API_SECRET: your API key (see [Front API docs on authentication](http://docs.frontapp.com/docs/public-api#authentication))
- FRONT_INBOX_ID: the ID of the inbox you want to export (see [Front API docs on listing all inboxes](http://docs.frontapp.com/docs/list-all-inboxes))

With these environment variables in place, run the script:

```$ npm start```

This will create a directory with a `conversations.json` file containing all conversations from the inbox. Per message a directory is created containing all attachments for the message.

### Disclaimer

Use at your own risk, no guarantees, don't try this at home, etc. etc.

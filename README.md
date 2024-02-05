# Node.js Assignment

## Instructions

**Important** Before you begin with the assignment, it is important to know that you will be required to work on Golang and Node.js projects both, starting with Golang projects.  You will be required to scale-up yourself in Golang if selected for the position.  If you aren't interested to learn and work with Golang programming language in addition to Node.js, then it is better you skip the assignment and update our hiring team.

```
1. Create a PRIVATE Github repository.  Add "idteam-at-onecom" as collaborator.
2. Read and understand the questions carefully before attempting them.
3. Record your assumptions about anything in a file for interviewers to consider.
4. This is a CONFIDENTIAL material of one.com and should not be shared with anyone else.
```

---

## Assignment

Build an `Event collector` HTTP micro service in Node.js.  Following are the requirements:

- HTTP service should run on port 7007
- Create a database using MySQL or PostgreSQL or CockroachDB to store the events.  Let us also see how well you define the database schema.
- Make a docker image of the service

Following are the endpoints:

1. `POST /event` - Store the list of events in the database
```
{
  "events": [
    {
      "type": "click",
      "item": "subscribe",
      "timestamp": "2024-02-02T10:15:26Z"
    },
    {
      "type": "close",
      "item": "inbox",
      "timestamp": "2024-02-02T10:15:26Z"
    }
  ]
}
```


2. `GET /event` - Returns list of all the events stored in the database

```
{
  "events": [
    {
      "type": "click",
      "item": "subscribe",
      "timestamp": "2024-02-02T10:15:26Z"
    },
    {
      "type": "close",
      "item": "inbox",
      "timestamp": "2024-02-02T10:15:26Z"
    }
  ]
}
```

---

## FAQs

**Q: Where do I have to solve the assignment?**

**A**: Implement it on your local system or use any virtual server on cloud/VPS, etc.  We will need this system again in panel interview, so do not destroy your work.

**Q: Do I have to use a particular operating system?**

**A**: It is up to you to choose operating system of your choice.

**Q: Do you have preference for a OS?**

**A**: We will prefer any Linux distribution of Ubuntu family.

**Q: Can I make this repository public?**

**A**: No, you should not do that.

**Q: Can I purge stuff on my system once changes are pushed to repo?**

**A**: No, you should not do that. If you are selected for panel interview, then panel may ask you to show it in real time.

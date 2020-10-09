# ARD Example
A single document approach to ARD's inspired by [this template from Michael Nygard](https://cognitect.com/blog/2011/11/15/documenting-architecture-decisions)

Tries to shrink the format yet further.

### Template

---

### ID - Title 
**Status**
  
**Context** 

What are the factors which fed into this decision (not just technical). Acknowledge contention but language should be neutral.

**Decision** 

What is change that has been made.

**Consequences** 

Impact of the decision, likely to be both positive and negative.

---

Status might be: Accepted, Proposed, Superseded

### ARDs

---

### ARD-1 - Decisions will not be spread over multiple files
**Proposed**

**Context**

Creating lots of files could make it hard for someone to quickly view all decisions.

Creating lots of files could make it hard for someone to quickly view change history.

We are only concerned with decisions made in small libraries and microservices.

We do not expect the number of decisions to be large.

We do not expect their to be a large workflow around decisions.

**Decision** 

All ARD's will be contained within a single file, separated by horizontal rules for clarity.

**Consequences** 

A reader will not need to run though multiple files to see all decisions that were made.

No index of an ARD will need to be maintained.

It will not be possible to link ARDs together.

This file will grow large if there are many complex decisions.

---

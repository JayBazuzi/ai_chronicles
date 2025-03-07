# The AI Chronicles

A spaceship crashes on a planet. You emerge in the wreckage of a civilization, populated by robots. How will you survive and thrive?

The AI Chronicles is an experiment in using OpenAI/ChatGPT to create a role-playing game. It's built in React and TypeScript on the front end with Spring Boot and Java on the back end.

We're building it live! Join us on Twitch every week at https://jitterted.stream. For more information, see https://www.jamesshore.com/s/ai-chronicles. Your hosts: [James Shore](https://www.jamesshore.com) and [Ted M. Young](https://ted.dev/about).


# Technical Approach

We are building The AI Chronicles using Extreme Programming practices, including pair programming, continuous integration, test-driven development, and more. For information, see [*The Art of Agile Development, 2nd ed.*](https://www.jamesshore.com/v2/books/aoad2) by James Shore.

* Architecture:
  * Monolith with separate React front-end and Spring Boot back-end
  * Monorepo with unified build (still in progress)
  * [A-Frame Architecture](https://www.jamesshore.com/v2/projects/nullables/testing-without-mocks#a-frame-arch)
  * Testing using [Nullables](https://www.jamesshore.com/v2/projects/nullables)


# The Plan

(Plan based on chapter 8, "Planning," of *The Art of Agile Development*.)


## Vision

A compelling role-playing game in which the player negotiates with a complex robot civilization. They have to balance the goals of multiple robot factions with their own goals and need for survival.


## Mission

Build a proof-of-concept that demonstrates three major gameplay systems: conversation, environmental hazards, and conflict.

Non-goals:

* We are not yet supporting robot factions or conversations with more than one robot.
* We are not yet supporting persistence or multiple players.


## Minimum Valuable Increments

* ➡️ A conversation with a robot resulting in success or failure, where "success" is the robot agreeing to take us to shelter.
* (Future: Additional MVI's involving environmental hazards and conflict.)


## User Stories

* ➡️ Placeholder communication with OpenAI
* Placeholder web page
* Conversation with OpenAI via front-end
* (Future: tbd)


## Engineering Tasks

* ➡️ OpenAI Wrapper that talks to real Open AI
* Nullable OpenAI Wrapper
* Reuse HttpClient wrapper that communicates via HTTP(S)
* Manual test of communication
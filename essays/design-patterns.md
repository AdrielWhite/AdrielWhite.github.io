---
layout: essay
type: essay
title: "Design Patterns: Don't Reinvent the Wheel"
# All dates must be YYYY-MM-DD format!
date: 2024-04-26
published: true
labels:
  - Software Engineering
  - Design Patterns
  - Java
  - Algorithms
---


In the world of software development, a common challenge is the constant need to reinvent solutions to common problems. As a student in an algorithms class, I often tackle familiar coding problems. While we analyze algorithms and their efficiencies, the pursuit of groundbreaking solutions remains elusive. This is because many of today's problems have been extensively studied and optimized over the years. Discovering a more efficient algorithm could lead to solving a complex problem, like the traveling salesman or Boolean satisfiability problems, and earning a million-dollar reward. Even small improvements in these solutions could revolutionize entire industries.

Design patterns are the unsung heroes of software engineering. They provide guidance for solving common issues efficiently. So, what are design patterns? They are not just abstract concepts, they are distilled wisdom from generations of programmers, encapsulated into reusable templates that transcend time and technology.

Consider creational patterns, for instance. These patterns provide a blueprint for creating objects in a flexible and decoupled manner. In my Java programming experience, I often used creational patterns. For example, when designing with prototypes, I used data structures to store information about abstract fruit objects and their specific subclasses, making object creation streamlined and scalable.

Similarly, structural patterns offer guidelines for composing classes and objects into larger structures. In a recent software project, "Project Portal," my team and I used a structural pattern to create collections of projects and sponsors, dynamically attaching sponsors to projects. This approach allowed for a modular and extensible design, seamlessly integrating sponsors into the project collection.

While I haven't extensively used behavioral design patterns, I recognize their potential in addressing complex behavioral scenarios in software systems. These patterns focus on assembling objects to solve common problems, like piecing together a puzzle.

Consider another instance where design patterns were instrumental, such as the implementation of the publish-subscribe pattern in the "Project Portal." We implemented the publish-subscribe pattern using MongoDB to deliver data efficiently from the server to the client. This pattern protected sensitive data, ensuring that only relevant information was shared with users based on their subscriptions. However, our implementation had a flaw: we filtered the data after subscription, allowing users to access all projects and then filtering them by project statuses. This oversight highlighted the importance of adhering to best practices in design pattern implementation, emphasizing the need for thorough planning.

In conclusion, design patterns are not just solutions; they are lessons learned and distilled into reusable templates that guide us in software development. They offer a way to avoid repeating the same mistakes and pitfalls that have been encountered and addressed by programmers before us. As George Santayana wisely said, "Those who cannot remember the past are condemned to repeat it.”

Use of Chat GPT:
* I wrote a detailed outline and gave it to Chat GPT to generate a draft
* I also gave it the prompt and a couple of my essays for reference of voice
* After that I repeatedly prompted it trying to make the language more simple and accurately reflect the messages I was trying to convey
* Then I made it end with the George Santayan quote
* I again tried to prompt it to sound like my voice by giving it a reference essay, but it got kind of confused
* The main point of this was to see how it would do and I think it's decent but not great

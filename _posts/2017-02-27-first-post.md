---
layout:     post
title:      Getting a CS internship sucks
date:       2017-02-27 14:30:01
summary:    How my failed quest to get a CS internship showed me the harsh reality of the software industry and how you need to fit the right model.
categories: hard CS student
---
Getting a CS internship sucks
=================================
***

## Background

In an increasingly full job market for interns the process to get employed as a Computer Science
student is nearly impossible. As a little background I am a Sophomore Computer Science
student as Boston University pursuing an internship with a technology company for the
Summer of 2017. I have always been fascinated with computers and have only fallen
more deeply in love with them since coming to school in 2015. I have worked on mostly
small projects, have a good understanding of Computer Science fundamentals.

One of the biggest issues in the job search thus far has been proving my worth
to these companies and convincing them that a Sophomore intern is worth their time.
Not only is it considerably more difficult to get your foot in the door as a Sophomore,
but it is harder to convince the company that regardless of the amount of formal
schooling you are an effective employee.

## Getting Interviews

When I first started applying for internship positions at various companies, I
naïvely assumed that if I applied to enough places I could get interviews and
persuade companies at that step. Getting an interview with a company is difficult
and for the larger companies they systematically weed you out of their process. The
style is considered acceptable because it is better for them to weed out the false-positives
(bad employees that look good) and risk the loss of false-negatives (good employees that
  look bad). Unfortunately for most of us, that means if you have a mediocre GPA
and small projects it can be impossible to argue your worth to an interviewer that
only sees that you cannot code an efficient implementation of Prim's algorithm in
a completely unrealistic on-the-spot environment.

### Prim's Algorithm Implementation
```ruby
# find the minimum spanning tree
def prim(graph G)
  adjacency_matrix = create_adjacency_matrix
  first_edge = select_first_edge(adjacency_matrix)
  @nodes_spanned_so_far, @edges = [first_edge[:start], first_edge[:end]], [first_edge]

  while !nodes_left_to_cover.empty?
    cheapest_edge = find_cheapest_edge(adjacency_matrix, @nodes_spanned_so_far, number_of_nodes)
    @edges << cheapest_edge
    @nodes_spanned_so_far << cheapest_edge[:start]  
  end

  puts "edges: #{@edges}, total spanning tree cost #{@edges.inject(0) {|acc, edge| acc + edge[:weight]}}"
end
```

Even still, I managed to get interviews with companies &mdash; although not very many,
about 15% &mdash; but when I got there I failed. I'm not sure exactly where I failed
in the process, but somewhere during the interview I failed to perform some menial
task that the interviewer had given me. Unfortunately, most of the interviews were
simple technical tasks in the one of the most awkward situations you could ask a
largely introverted group of people to perform in. I mostly got interviews with
companies thanks to [a wonderful piece written by Felix Feng](https://medium.freecodecamp.com/5-key-learnings-from-the-post-bootcamp-job-search-9a07468d2331#.kcgstarkj)
which describes the best methods for actually getting the interview.

## In the Interview

This was probably the scariest part of the entire process. Once I finally got into
the actual interview itself it was some of the weirdest experiences I have ever had.
Generally there are a couple stages/types of interviews when applying for programming
or software internships. Obviously I have not made it through the entire process
so I may be missing out on certain steps or functions, but the first stages are
generally the same throughout.

> ![HackerRank Coding Challenge Invitation](/blog/images/mozilla-hackerrank.png)

1. Coding Challenge/Phone Screen
2. Possible self-recorded video interview
3. Technical Interview
4. More technical interviews
5. Offer or on work-campus interviews

The first interview is usually a phone screen which is either a phone call or video
call where the interviewer is simply trying to get an idea of you as a person. The
second interview is typically only done by large companies who do not have the time
to individually phone interview candidates. Third is where the interviews start
to really show how different a job application is for CS/Engineering students
than any other field of profession. The technical interview is an on-the-spot
interview where you are typically asked to write a small program that traverses a
binary tree or implement a hash table. They are not complicated, but most students
do not posses the proper knowledge of how to prepare for these interviews and by
the time they find out, it is far too late.

> They are not complicated, but most students
  do not possess the proper knowledge of how to prepare for these interviews and by
  the time they find out, it is far too late.

During the interviews I felt as if I was doing well enough to solve the problems
they presented me. I was told to write a function that would implement and update
a balanced binary tree. However, the feedback was minimal and I felt that I was expected
to know everything. I ran into the same issue that most CS students come across,
especially at a school not in the top CS schools. When we started applying, it
was too late and we did not know that we should have been preparing for at least a
month before the interview. Instead of testing/judging candidates on their ability
and hunger to learn new things, and passion for CS they judge their candidates on
their ability to program on the spot.

## Results &amp; Reflection

All in all I learned a lot this year and am grateful for the help that my family
and friends have provided me. Unfortunately, complaining about industry standards is not
going to help me or you get a job. Because of this fact, there are many things
that I would recommend to CS students and prospective interns in the software industry:

> ![Interview Rejection Email](/blog/images/basecamp-reject.png)

- Start practicing your CS fundamentals months ahead of time
- Email a real person at the company (ala Felix Feng's piece)
- Learn what they want you to learn (Algo's, Data structures, etc)
- Read [Cracking the Coding Interview](https://www.amazon.com/Cracking-Coding-Interview-Programming-Questions/dp/0984782850/ref=pd_sbs_14_t_0?_encoding=UTF8&psc=1&refRID=9VYEGF6MTP5FGEXEZTRF) by Gayle Laakmann McDowell
- Do side projects! Whatever you make, if it is interesting to you will get you into more interviews and will teach you more than any book can.
- Follow through on your side projects, there's no point of starting them if you don't plan to finish them.

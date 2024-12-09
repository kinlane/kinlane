---
published: true
layout: post
title: 'Radical Book Buzz with Library Freedom Project and Library Futures at the Francis Kite Club'
date: 2024-12-09T12:00:00.000Z
tags:
  - Publishing
  - Authors
  - Books
  - Radical
  - Libaries
image: https://kinlane-productions2.s3.us-east-1.amazonaws.com/book-event-nyc/radical-book-buzz.jpg
---
Audrey and I headed down to the East Village last night for the [Radical Book Buzz](https://www.eventbrite.com/e/radical-book-buzz-with-library-freedom-project-and-library-futures-tickets-1073114086119) with Library Freedom Project and Library Futures at [The Francis Kite Club](https://www.franciskiteclub.com/). The intimate event showcased the good work of the Library Freedom Project and Library Futures organizations, but also showcased ten publishers who support radical authors across a variety of genres.

{% assign publishers = site.data.publishers %}
<table align="center" style="width: 70%">
{% for publisher in publishers %}
    {% if publisher.BookName == "No Straight Road Takes You There" or publisher.BookName == "Talking About Abolition" or publisher.BookName == "Motherdom" or publisher.BookName == "B. Traven, Portrait of a Famous Unknown" or publisher.BookName == "If I Must Die" or publisher.BookName == "Mafalda" or publisher.BookName == "Sympathy For Wild Girls" or publisher.BookName == "Gabriële" or publisher.BookName == "King of the North" or publisher.BookName == "Ghassan Kanafani, Selected Political Writings" %}
    <tr>
        <td width="175" align="center">
            <a href="{{ publisher.BookUrl }}"><img src="{{ publisher.BookImage }}" width="150" style="border: 3px solid #000;"></a>
        </td>
        <td>
            <a href="{{ publisher.BookUrl }}">{{ publisher.BookName }}</a> by {{ publisher.BookAuthor }} from <a href="{{ publisher.BookUrl }}">{{ publisherUrl }}</a> - {{ publisher.BookDescription }}
        </td>
    </tr>
    {% endif %}
{% endfor %}
</table>

I will be working through these titles, but also continuing to explore what is coming from these publishers. [I published this list as YAML](https://github.com/kinlane/kinlane/blob/main/_data/publishers.yml) so that I can power future stories, but also feed my reminders to regularly tune into what these publishers offer and reduce my attention given to Amazon.

I am thankful for the work of these two organizations for making the event happen and bring together the publishers, but also everyone that made it out last night for such an important aspect of storytelling.

{% assign organizations = site.data.organizations %}
<table align="center" style="width: 70%">
{% for organization in organizations %}
    {% if organization.name == "Library Freedom Project" or organization.name == "Library Futures" %}
    <tr>
        <td width="175" align="center">
            <a href="{{ organization.url }}"><img src="{{ organization.image }}" width="150" style="border: 3px solid #000;"></a>
        </td>
        <td>
            <a href="{{ organization.url }}">{{ organization.name }}</a> - {{ organization.description }}
        </td>
    </tr>
    {% endif %}
{% endfor %}
</table>

I walked away with more of an awareness of how the translation of radical books between languages, but also how the republishing of books that have gone out of print impacts our storytelling. I was also reminded of how this fucked up timeline we find ourselves in is driven by Amazon, Overdrive, Elsevier, and Penguin Random House, HarperCollins, Macmillan, Simon and Shuster, and the other top book publishers.

As I make my way through these books I will publish more here about what I am reading, and when I find any new books from these publishers I will share as well. It feels like these outlets are our lifeline to the storytelling that is going to save us, sustain us, and bring us together in these troubling times. I don't know about you, but I am looking to spend my time in the next few years reading and trying to attend as many events like this as I can to help me stay in tune with what truly matters.

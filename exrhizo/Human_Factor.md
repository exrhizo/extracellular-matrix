# The Human Factor

![[00_Static/TheHumanFactor/logo.png]]
[app.thehumanfactor.ai](https://app.TheHumanFactor.ai)

### Truly interactive online learning for interpersonal skills

The mission of The Human Factor is improving emotional regulation by making interpersonal skills measurable.

The product is inspired by the [Facilitative Interpersonal Skills Assessment](http://clinica.ispa.pt/ficheiros/areas_utilizador/user11/facilitative_interpersonal_skill_manual_and_rating_scale.pdf). Shown to be the most predictive indicator of psychotherapist effectiveness.

The team decided to discontinue work, not because we don't believe in the mission or product, but because life took us in different directions.

Please reach out if you are interested in working with video role plays.

## Philosophical Background

Most assessments are working with System 2, the logical conscious process of
the mind. However, interpersonal interactions engage both aspects of mind.
The emotional reactionary instinctual orientations are the background
from which our speaking comes. This is why _State of Being_ is important and
techniques are of secondary importance to presence.

By tightening the feedback loop, video role plays get closer to
the experiencing mind, and allow us to measure the capacity individuals have to
bring awareness to the distress of others and to exercise leadership in
relationship. This is the essence of spiritual adulthood, to respond to suffering while honoring the goodness of life.

Before it is possible to work with others, we must first develop the capacity
internally. There can't be an alliance with the other if there isn't already
an internal alliance with experiencing self. Shadow work shows us that people
project their internal conflict onto others and judge them the same ways that
they judge themselves. Because of this, Video Role Play also has the possibility of illuminating where individuals are caught in internal conflict and confusion.


## Founding Team

- [Brian Basham](https://www.coachbasham.com)
- [Leo Urbina](https://leourbina.com)
- Alex Warren (Myself)

## The Product

The app is a platform for doing video role plays. You watch a video of a challenging interpersonal situation (e.g. someone companies you have been judging them) and then your response is immediately recorded. It's as though you are in a micro dialog with the person. The unfinished part of the product is reviewing and scoring the responses.

We explored multiple industries and variations for the target market, situations where it is valuable to assess people's interpersonal capacity, e.g. sales.

To develop this product, I interviewed performers, to elicit challenging situations and tested the situations on end users to iterate both the UI and the content.


## Who worked on what?

Alex was the Front End lead for this project, and would design and develop accross the stack. Leo did dev ops and back-end. The entire team made strategic and tactical decisions. This is Alex's product portfolio, so it focuses on that.


## Product Design

There are three main types of users:

 - Assessment end users
 - Content creation actors / actresses
 - Administrators

In these screenshots, the design doesn't yet reflect the different user journeys that they would experience. At this point our main goal was to iterate on the content and get it clear to users what a challenge is.

### Login / Profile

 ![[00_Static/TheHumanFactor/login_web.jpg]]

I developed a full stack authentication for, for users to log on with token and refresh tokens and for requests to cause a token refresh.

## Create Challenge (Web & Mobile)

![[00_Static/TheHumanFactor/record_web.jpg]]
![[00_Static/TheHumanFactor/record_mobile.jpg]]


I worked with actors and actresses to develop content for our assessments. It was done over video chat and we iterated to find emotional situations that connected to the performers experience so that the challenge would have realism.


## Browsing Challenges / Responses

![[00_Static/TheHumanFactor/responses_web.jpg]]

## Respond to Challenge

An end user recorded thier response parallel to the challenge video that was played. We developed a backend using Google Cloud Storage and Postgres to store and serve these recordings.

![[00_Static/TheHumanFactor/take_challenge_web_0.jpg]]
![[00_Static/TheHumanFactor/take_challenge_web_1.jpg]]
![[00_Static/TheHumanFactor/take_challenge_web_2.jpg]]

### Respond to Challenge on Mobile

The app has a responsive design and challenges can be taken on mobile phones.


![[00_Static/TheHumanFactor/take_challenge_mobile_2.jpg]]


## Admin

The Administration panel allows editing of which challenges are visible, as well as descriptions and titles.

![[00_Static/TheHumanFactor/admin_web_detail.jpg]]
![[00_Static/TheHumanFactor/admin_web_list.jpg]]

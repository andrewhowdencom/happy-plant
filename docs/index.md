# Happy Plant?: Open source plant analytics

### An idea posted into the void in the hope that someone picks it up

An idea that I have been playing with now for about 6 months is to build and ship little hardware devices that keep track of devices. This neither a unique, nor particularly innovative idea — a simple Google search of “Raspberry Pi plant” shows this has been done by hobbyists innumerable times:

![[https://www.google.co.uk/search?q=raspiberry+pi+plant&oq=raspiberry+pi+plant](https://www.google.co.uk/search?q=raspiberry+pi+plant&oq=raspiberry+pi+plant)](https://cdn-images-1.medium.com/max/2260/1*2i4qlHK7cPaDu52FrQGPvA.png)*[https://www.google.co.uk/search?q=raspiberry+pi+plant&oq=raspiberry+pi+plant](https://www.google.co.uk/search?q=raspiberry+pi+plant&oq=raspiberry+pi+plant)*

However, none of these solutions appear to have been brought to the “consumer” market. Indeed, the consumer market is a tough nut to crack, and the cross-section of those who are into tech but also plants would seem to be a niche market indeed.

However, it is my suspicion that for various reasons a correctly positioned and delivered analytics tool would be well received by various parts of those inclined to leafery. Unfortunately the things I would like to do far exceed the time I have to push forward with such ideas, so to start the conversation around this topic I’m writing this up in a post.

Please feel free to steal this idea and take it to market. If it makes you a millionaire I would appreciate you paying off my university debt.

## A warning

I sit at a cross section of a few different interests which is why I am investigating this. However, this post denotes where I am beginning to investigate this topic in earnest, rather than making a collection of half formed ideas written on the telephone.

Accordingly, much of the information that you find here might be wildly incorrect, and the challenges dramatically underestimated.

Or, put simply, I know fuck all about this stuff.

## Why Now

My understanding of how a product’s success in the market is determined is based on a few different things:

* The quality of that product

* The audience to whom that product is released

* The cost of the product relative to its potential gains

There have been for the last couple of years unique tradeoffs in the combination of these things that mean the market might be well positioned to receive such an agricultural device.

### Audience

There have been several notable developments of recent years that make the audience more receptive to a solution that both exposes and uses data to help manage agricultural product.

Firstly, and as an overarching motivation climate change seems to be changing the nature of agriculture. In my home country of Australia [increasing drought conditions mean farmers must innovate, growing their relative productivity year after year simply to maintain the same yields.](http://theconversation.com/australian-farmers-are-adapting-to-climate-change-76939) In Africa [wheat production is expected to decline by 10–20%, while population growth increases.](https://www.un.org/africarenewal/magazine/special-edition-agriculture-2014/despite-climate-change-africa-can-feed-africa) However, by counterpoint, [the Netherlands have dramatically increased their agricultural yield by applying new, tech driven approaches to farming.](https://www.nationalgeographic.com/magazine/2017/09/holland-agriculture-sustainable-farming/) Global warming provides perhaps humanities largest challenge and, while it may change our nature and relationship with the earth, keeping humanity supplied with as much food as possible is perhaps the most sustainable business model imaginable.

Secondly, the market is already showing interest in adopting technology to help improve agricultural yields. In addition to the aforementioned Netherlands example there are cases where [farmers are using machine learning to filter out remove bad plants](https://cloud.google.com/blog/products/gcp/how-a-japanese-cucumber-farmer-is-using-deep-learning-and-tensorflow) or [collaborating to share rain data.](https://www.maschinenring.de/leistungen/information-beratung/wetterstationen) The market is embracing technological solutions to its projects, but the current buy in is extremely high.

Thirdly, technology is fundamentally shifting the constraints around our lives. The internet initially allowing us to connect and transfer information at essentially zero cost, cell phones allowing us to both access and supply that information at a moments notice and new hardware sensors taking advantage of this cheap wireless network to relay information back to a central based station to command combined with new ways to analyse and make useful this data mean that our lives are becoming dramatically more efficient than they once did. It stands to reason that instrumenting our agriculture in the same way would allow similar gains in efficiency, in exactly the same way Google Maps supplying traffic information allows us to navigate the flows of traffic.

Accordingly, the audience is uniquely prepared and willing to take the risk on a product that makes available the same insights that have been applied from other verticals to agriculture.

### Cost

It is additionally my conjecture that it is rarely those who invent a solution that will both roll it out to a mass market and reap the gains that such a rolling out entails.

Consider the cast of Android, a sub-par quality operating system released at a similar time to iOS. However, when Android was released it was released freely to the world, and has [thus become the dominant phone operating system.](http://gs.statcounter.com/os-market-share/mobile/europe)

Alternatively consider the case of Facebook (or even MySpace), [which aggressively pursued reducing consumer cost to do all sorts of bizarre but somewhat social actions ](https://www.forbes.com/sites/adamhartung/2011/01/14/why-facebook-beat-myspace/#6fa2020a147e)— all within the Facebook ecosystem.

In all cases, those who bring the cost of a product down to such a low level that it is trivial to implement quickly monopolise the market, finding new ways to add revenue to their business on top of their monopoly position.

The goal of the Happy Plant project would be to take a similar market strategy — release the core product for free, and entirely open source. This would allow experimenting with the product freely, as well as allowing a community to form and hack on the product itself. Such a community would then dictate the future of the product, and any business entity set up behind Happy Plant would need to use its knowledge and influence over the project to set up a continued revenue stream such as shared, centralised analytics.

### Quality of product

Though, in my mind, it has far less impact than the other two on the general success of a product it is still a critical component. However, here we’re quite lucky in that there is an abundance of superbly high quality technical solutions available for commodity pricing.

The principle thrust of this idea is that the management of agricultural networks is similar to the management of computer networks. Indeed, it may be reasonable to model the agricultural industry on the computing one — consider a crop consisting of many different plants, each complementary to its neighbours, rather than large homogenous crops.

Within the realm of networked computer management there is an abundance of tools that are designed to collect, store, analyze and display time series data. Tools such as:

* Prometheus

* InfluxDB

* Grafana

These tools have even agreed on interoperable protocols allowing a mix and match style approach of software to solve specific problems.

It should be readily possible to use these, or similar tools to develop solutions quickly and cheaply that allow high quality data to be collected, analysed, stored and made useful.

## Vision

The analysis of the market fit side, in order to define the goal of this project. Broadly, the goal is:
> Trivially available, ubiquitous analytics for agriculture.

## Unique Selling Point

Given the above any number of solutions would be possible. However, for a solution to be successful it must be the most ${SOMETHING} more than any alternatives.

There are several properties that might distinguish this model of plant helper aside from others that either exist on the market or will enter it shortly.

### Cheap

The goal of this exercise is not maximal profit, but rather developing and deploying trivial agricultural economics. To do this, the invest on the part of farmers must be as cheap as possible.

The simplest cheap solution is a free solution. The goal of this project should be to assemble a device from commodity hardware, such as a “Raspiberry pi experiments kit”, insert an SD card of the appropriate “type” and boot the device.

In this case, the required pricing is for the Raspberry pi kit.

### Simple

What distinguishes the hobbyist market from the commercial one is the ability of hobbyists to invest time. Time can be spent a number of ways:

1. Learning how to build the device

1. Learning how to program the rpi

1. Making the mistakes

1. Developing interfaces for the rpi

1. Maintaining the stack

This time is absolutely unreasonable for either the consumer or agricultural market. The device should be as simple as possible.

Here, there is a tradeoff. The core of the device must be free, which means it’s on the implementer to build the rpi and attach sensors. However, once the rpi is built we can use the “etcher” tool or similar to flash an SD card with the “Happy plant OS”, and the tool should be up and running.

Alternatively, it is reasonable to sell fully assembled kits pre-installed with the happy planter OS — however, these kits must be assembled exactly as the users will assemble their own kits.

### Standards Driven

Part of the difficulties in implementing a “smart home”, or other smart type networks is that each given device is not interoperable. Devices from one manufacturer do not work with another and a consumer must select a given manufacturer, trusting them to continue manufacture of these devices.

By contrast, the happy plant would consist of a set of independent components, each adhering to either specifications that exist or published specifications that must be complete before implementation is started.

In this way we are able to have parts of the stack replaceable by custom solutions implemented by larger bodies while still reusing the same core hardware and operating system. We further invite other tools to be built on top of the happy plant that take action on the plants state, such as a system that waters the plant when moisture sensors indicate that this should be completed.

This property would give the happy plant a life beyond mistakes in each component of the system, giving it a resilience otherwise hard to meet in the market.

### Federable

One of the unique problems associated with the “Internet of Things” (IoT) is the necessity to have the device functional with a minimum of information. Various devices approach this in different ways:

* Google Home works together with other Google Homes

* Panasonic lights completely ignore each other, using a central hub

One of the cooler, unique properties of the Prometheus time series data monitoring too is called “Federation”. This allows one Prometheus server to collect data from another Prometheus server:

                         +-----------+
                         |           |
          +--------------+           +-------------+
          |              |  PROM     |             |
          |              |           |             |
          |              +-----+-----+             |
          |                    |                   |
          |                    |                   |
          v                    v                   v
    +-----------+        +-----------+     +-------------+
    |           |        |           |     |             |
    |    PROM   |        |           |     |    PROM     |
    |           |        |  PROM     |     |             |
    |           |        |           |     |             |
    +-----------+        +-----------+     +-------------+

What is particularly clever about this is that each Prometheus server is individually useful, but even more useful when combined with several other Prometheus servers.

This means there are two options for running Prometheus:

* By itself

* With other Prometheus’s

The same property should exist for the happy plant. Each individual unit should be useful. However, should more units be added they should become more useful.

This would perhaps be fairly easy to implement by simply allowing them to discover each other (via smth like gossip) for “cross service” federation, or by allowing a third party base station for “hierarchical” federation.

### Hackable

Lastly, being open source, the happy plant should be hackable. There’s no way we’ll hit upon the right abstractions first up. However, being built in the open perhaps there are some lessons that others may find both more utility and success.

## Architecture

Broadly, there are several high level components that need to exist for this to be a full entity. They are separate components as it is reasonable that hardware could be created more cheaply for sensor networks rather than packaging it all in the heavyweight rpi.
> **Note**: This is a conceptual overview, and considerably different to the original plan I had in my head. This is more like “Hmm if i was designing this and I had infinite time, I’d do…”. Current plan is to package all components up into a single box (rpi) and ship them.

### Sensor

This is a target with network access that reads some property of the agricultural material and expresses the content in [the “Prometheus” or “Open Metrics” format.](https://github.com/prometheus/docs/blob/master/content/docs/instrumenting/exposition_formats.md)

### Data Store

This is some component that reads the content from the target that exposes the metrics in the Prometheus format and stores it with the time that this value was present.

### UI

This is some component that queries the content from the data store and displays it for humans

### Control Loop

This is some component that reads the data from the data store and applies some change designed to modify the data in a desirable way.

## Minimum viable product

### This Post

Given that this is designed to be a vehicle to describe a desired, open source product the minimum viable product is probably this post or the links associated.

Based on who reads this and whether I have time I will either pursue this, or not.

### Raspberry Pi

Broadly, the goal would be to create a raspberry pi build that made this fairly trivial.

The architecture components aforementioned should be exposed by this pi.

It’d probably consist of the following components:

* Project Atomic / CoreOS, or another self-upgrading container based OS

* CRI-O or another container runtime

* Maaaybe Kubernetes. It’s a lot of overhead, but it also handles a bunch of tricky tasks like application upgrades. Toyota is including it in cars, maybe it’ll work.

* Prometheus to collect and store the data

* A custom UI to display the data

* Some sort of app to help set up the device

* A web app to control the device, hosted on the device itself.

* A “feedback look” app (maybe just AlertManager) that alerted when the plant was in an unexpected condition.

* A case from Shapeways

All this would need to be regularly rebuilt, presumably via a CI/CD service (Travis CI et. al) and then stored as an image. The image can then be linked on GitHub, burned with Etcher.io and then run on the Raspberry pi.

Once on the pi, it should be self updating.

## Potential future features

### Plant detection

It would be reasonable to use a companion application to take a photo of a given plant, and have that analysed by some sort of machine learning based plant identification service.

The device can then be configured to alert based on the specific requirements of that plant, perhaps even given sunlight and altitude information.

### Automated plant management

A natural progression of “Happy Plant” would be “Active plant”; tools that modified the state of a plant or a set of plant based on data supplied by the sensor.

A simple example would be watering the plant, but it could extend further to:

* Opening windows in a greenhouse based on air properties

* Drawing shade over a greenhouse based on temperature

* Turning off or on lamps based on power consumption rates and plant health

Google supplies a bunch of good information about preventing noisy alerts which is also useful in the context of scheduling too many or too sharp actions based on these alerts.

### Centralised analysis

Cheap, commodity data invites analysis. By collecting large pools of plant data such as moisture, electrical conductivity and a host of other arbitrary sensors it may be possible to draw new patterns about the state of a given plant, as well as that tendency of plants in general.

## Revenue Model

Should this project gain any interest it would need a benefactor that devotes their time to bringing it to life. That benefactor will likely not work for free (or even cheap), and the project thus needs to deliver so much value to its consumers they decide to impart their cash to it.

Given that the core product is free, it must be possible to make revenue on other, more “premium” services. This could include:

### Payment to direct development

One of the more interesting open source models for small projects such as cURL or OSQuery is to pay to implement features that are good for a project, but not immediately on the road map. This benefits both the user who is paying to have that feature implemented but also the project, as the feature is contributed back.

### Donation / Patreon

It might be reasonable that an income is based on continuing benefactors of the project. Perhaps agricultural workers might be convinced to donate a subscription fee to continue the development of the project.

### Installation / Support

While the goal of the project is to be as simple as possible, it stands to reason there will be custom deployments of this or similar tech.

Such deployments make for good consultation opportunities, as well as highlights areas in which users are not self-sufficient.

### Centralised management

Being the developer of the tool allows the insertion of advertising material for a centralised management service of these devices.

Such a service is not necessary, but perhaps useful for users who do not want the overhead of setting up the and managing many of these devices themselves. The advantage of this would be:

* Health checking the device itself

* Centralised analytics

* Access to shared data

### Selling of units

Additionally and as mentioned, regardless of whether the software is free some assembly will be required to ship the units. For the consumer market, these units can be created and solid as pre-built packages in premium casings and with pre-configured sensor sets.

## Market

The delivery of the happy plant would go through several stages:

### Hobbyist

There is already an active hobbyist community around all these technologies. Finding fit in this community and providing a centralised project for all to contribute to and benefit from would be a mutually beneficial activity, as well as give the project its initial community.

### Academia

Academia are in a similar position as hobbyists, but require larger deployments and further understanding and analysis of devices. They make good “second tier” markets, allowing semi-commercialisation of the project as well as potentially connections with industry

### Commercial

The commercial market is the ultimate goal of such a project. While hobbyist markets are potentially interesting and would demonstrate some project success, a product needs to be deployed in an industrial way in order to truly improve the efficiency as it is intended.

### Consumer

Lastly, as a mechanism to both make consumer market as simple as possible and to continue to drive innovation and simplicity the goal of this project is to make the consumer market.

This forces the device to remain cheap, simple and easy to use.

## Further Links

* [https://mtlynch.io/greenpithumb/](https://mtlynch.io/greenpithumb/)

* [https://www.sciencedirect.com/science/article/pii/S0007681317301325](https://www.sciencedirect.com/science/article/pii/S0007681317301325)
`

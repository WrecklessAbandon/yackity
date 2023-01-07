# yackity
A communication system that is protocol agnostic.

# Primary Objective
The primary purpose of this project is to allow users to relay messages to each other across any platform, without needing to constantly update the routing addresses.

This means hacking existing & supported multiplatform protocols to be used to relay modern communications. The hacking involved is minimal and mostly relies on the presentation layer - changing the netiquette and the way the information is interpreted rather than changing the protocol to behave differently.

It's imperative that people are able to communicate with each other using modern interfaces across different networks and platforms. The goal of this project is to allow users to use a modern interface with modern features to communicate while at the same time have their communications reliably routed across multiple different platforms.

It would be more efficient for a modern protocol that has everything required for modern communication to be routed across multiple platforms. An example of a protocol that is supported across multiple platforms is SMTP (email). This protocol is supported across Google, Microsoft, Apple, Facebook, ISPs and many others - which means it would be possible to send messages across these platforms and have them correctly routed to their destination.

If I send a message from myemail@gmail.com to myemail@apple.com, I can rest assured that my message will be correctly routed to its destination. However, if I were to use an open protocol such as the XMPP, I would need the platform to support it in order for my messages to be correctly relayed. For XMPP to work, 2 clients would need a service to exist in the middle in order to facilitate their communication. As it currently exists, platforms such as Apple, Microsoft, ISPs or others don't generally provide an XMPP service that can route XMPP messages.

It's possible to rely on the lowest common denominator, such as IP address as a relay, but this comes with its own set of platform dependent problems that require constant monitoring and updating - such as updating the destination IP addresses.

Some hacking may be more intense - such as sending 5 emails to transmit a binary file. From the user's perspective, they've simply initiated a file transfer but from the platform perspective there have been 5 emails sent. The hacking of these protocols will also introduce sub-optimal behaviour, but it's better for something to mostly work than for multiplatform relaying to be impossible.

# Secondary Objective
The way in which communications also needs to be modernized, much of this is controlled through our expectation to communicate. The concept of email is modeled after mail; the message is expected to be asynchronously delivered and maybe requires an asynchronous reply. Common Netiquette in email also dictates a type of formality, in the traditional sense of writing a letter. None of this is necessary but it's encouraged since the medium is the message and the medium is presented to us as if it were a stack of letters.
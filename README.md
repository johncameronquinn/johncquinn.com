# johncquinn.com


## overview

This is my professional website, with serverless hosting, based off another theme [moonwalk](https://github.com/abhinavs/moonwalk).

I built this over the course of several days, utilizing a variety of outdated resources on the subject. 

My resulting email address is simply mail -a-t- johncquinn.com, which I was pretty happy about the snappy nature of that. 

"Very professional" 

and easy to remember. This is desirable since I am seeking gainful employment.

The content listed here is a rough mirror of what is on my s3 repo, minus a few changes which I made for s3-cloudfront compatibility.

Check out my [security headers implementation score!](https://securityheaders.com/?q=www.johncquinn.com&followRedirects=on)

## design

Overall I'm looking for a design that prioritizes pragmatism. Some visuals are pragmatic, but if it jeopardizes the speed and function of the website then I left it out. This is the website of a computer scientist, not a graphic designer, so I with that in mind, I decided to forgo javascript. There is no reason for the unnecessary complexity.


### tools

- vim because it's a small project
- QubesOS lets me easily have a separate VM (Xen PVHVM) just for this task, at the cost of almost no additional hard disk space. [Check out the design for that system as well](https://www.johncquinn.com/hardened-qubes-os).
- awscli & a few bash scripts I wrote to make management easier

### serverless hosting

- uses s3 for hosting, aws cloudfront for deployment, and aws lambda@edge to handle security headers.
- cert is from amazon
- I use namecheap as the registrar, and pointed the records to Route53

## email

- I utilize mailbox for a more private and techie-friendly email service. 
- my PGP key is posted on my website, as well as hosted on keys.openpgp.org
- that PGP can be trusted to a moderately high degree. I followed proper security protocol to a moderate degree when handling it. 
Should anything happen to that private key, I have a master key to revolk and generate a new one.
Should anything happen to that master key, I have revocation certificates everywhere.

I also hand out physical copies of my keys whenever possible. I can't wait till there's a very effective method to print entire keys on business cards.
Until then, I've had to settle for less ideal solutions.

Still, it's overkill considering my threat model, which probably personifies most of what I do.

I just like playing secret agent man.

I'm relatively confident my secret agent man desires could serve to further foster marketable skills, which reasonably could provide mutual value
for both myself and an employer.

I'd love to hear about potential job opportunities. PGP not required.

Thanks for reading!

## Acknowledgement
This theme is based on [moonwalk](https://github.com/abhinavs/moonwalk)
I started with essentially his entire codebase and then proceeded to modify it to suit my needs in a rather heavy-handed manner.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
That was the previous repo's license and I won't be changing it. I'm not sure if I've modified this substantially enough to call it "my own" yet,
but I don't really care at the moment.

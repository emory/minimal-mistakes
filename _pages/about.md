---
layout: single
permalink: //about/index.html
title: "a͍̻̝͞b͇̝o̶̦̝̩̖̮̗ù͇̘̦͕t̢̤̠͚͚̳͔͎ ͕̖̟̲͟emòry̱͖̦̘͍̩ͅ"
description: "an about page"
category: [meta, emory]
author_profile: true
toc: true
---
My name is Emory, but I tell Siri that she can call me *big papa*.

## Brief Bio 

I'm a network security *friengineer* by trade; also a serial hobbyiest, writer, photographer, practicing min-maxer, and a category-five wisenheimer.

I am often carrying a camera and have no indoor voice.

Going way back in time; I was the founder of hellyeah! networks. Most of this once proud society of slackers and hackers has been swallowed by the cloud, but we're still out there kicking it. [^1]

## Outputs

### Web 

I have a sometimes-used *linkblog*, ([emory.KVET.CH](http://emory.kvet.ch/)) and a photography portfolio, [ephemeral.be](http://ephemeral.be/). I've slowly been moving things I've written or organized to this site in order to keep my best-ofs all in one place rather than scattered between a dozen half-finished projects that end up getting neglected. 

### Podcasting

With the Internet's own [Alan Joyce](http://thisisalan.com/) I sometimes co-host a podcast called <a href="http://show.hellyeah.com/" target="_blank">the hellyeah! show</a>, which is now in its third season. It is best described as two geeks trying to find better ways to do things, and then talk about games. We haven't recorded in a little while but maybe that will change.

## Socialism

I sometimes (often) spam on <a href="http://facebook.com/incumbent/">Facebook</a>, very rarely find my way to the [twitter machine](http://twitter.com/incumbent) because it's a head-wound waiting to happen `#headdesk`. I am interested in just about any social or messaging service and try them all at least once. I'm considering playing around with [Mastodon](https://joinmastodon.org/) now and then. Eventually we'll get something as useful as `finger` and `zephyr` after the billions of dollars in venture capital have failed to deliver us from terminals, right? 

You may also find me on [flickr](http://flickr.com/photos/sempai), but I generally treat it like a high-res [instagram](http://instagram.com/incumbent). Lately I've been keeping an eye on [VSCO Grid](http://ephemory.vsco.co/) and [oggl](http://oggl.me/emory/), too. I even have a page on [ello](http://ello.co/kvetch)!

### Chat

You can find me on hellyeah! Slack, or a few other haunts.

## Projects I'm Working On

**Creatively** I'm currently working on something about semi-secret societies and new spiritual orders that are changing the course of policy in the United States. It's speculative fiction, which means I'm making shit up, but it sounds plausible.

I'm also working on a few photography projects that I'm likely forever [casting](/casting). One of them is about the workflows of creative people; what they do and how they get it done. Their creative process will never be the same as anyone else, and I'm interested in that sort of thing.

**Professionally** I'm working on incident response, cloud security architectures, and operations management in a dev-ops environment, and generally approaching decades of old already-solved problems again, with new and very different constraints. Incident response and forensics are very different concepts these days!

I am also tinkering in the lab with location services, mobile applications, accessible encryption, and personal publishing. I have the dubious distinction of being listed as an inventor on a patent for an authenticated content syndication system that was gently paired with RSS/atom and OpenID.

I did the technical review for a few O'Reilly books on OS X and smartphones, and wrote half of one myself that was never released but still lives on Amazon's Canadian site for some reason. 

## Work & Availability

My consulting practice, [due\|vigilance](http://duevigilance.com/), is where you can learn more about my consulting services. Summer of 2019 I am taking clients for technical or security engagements, **I am especially very *available* for script review** on creative projects for the web, paper, television and film. If you're working on a project that could benefit from some experise on the *seedy underbelly of the Internet*, please tell me all about it. I would love to give your project some extra authenticity without losing your audience in the process. I can make very complex things approachable by non-nerds, and yet relevant and accurate enough for even the most grizzly of neckbeards.

## Contact

The best ways to contact me are probably:

* send an [email](mailto:emory@hellyeah.com)
* ping me via [iMessage](imessage://emory@hellyeah.com)
* [sms](sms:+16465436679) or [phone](tel:+16465436679) @ +1-646-54-EMORY

These are ranked in order of how disruptive they are, low to high. Sending a raven from King's Landing is no longer available; you know who you are, and thank you so much for ruining it for everybody.

# Encrypted Email

Very well, 007. You're catching me a little off-guard right now because I've been thinking about this quite a bit lately but I'm prepared to accept your message with the following caveats. 

#### OpenPGP, GNUpg, PGP

My latest (as of 2017-12-22) public key [<span class="fa fa-lock"></span> 4096/5673CB70](/files/5673CB70.asc) is available direct from me, the keyservers you already use, but **most authoritatively** on [Keybase](http://keybase.io/emory).

The only mobile email client that gives me a satisfactory way to handle GNUpg/openpgp is [Canary](https://canarymail.io) but at my desk I still use [MailMate](https://freron.com) because it does a lot of really amazing things to handle email but also supports S/MIME and GNUpg/openpgp so well.

#### S/MIME

Since iOS supports S/MIME natively, I prefer using that, in spite of bugs in Apple's implementation (Mail.app has a hard time with SubjectAlternateNames in X.509)

# How I really feel about the Certificate Authorities

This is the part where I deviate from typical use-cases.
{: .notice}

I don't have a lot of reason to trust that the widely trusted certificate authorities are trustworthy at the level of email certificates. I don't think they do sufficient verification on the identity of people and individuals that request email certificates regardless of charging money for it or not. 

I'm not aware of a certificate authority that even offers email certificates that aren't verified by completely meaningless and trivial  measures (they literally just make sure you have access to an email account long enough to verify receiving an email there which I find a little insulting), and when you get a free email certificate from one of the providers out there like StartCom or Comodo, you're also given a limited certificate with reduced capabilities and purposes **and** it doesn't include anything identifiable in the fields of the certificate because they didn't validate a name only the email address, which means you have to drill into individual certificates to find the one you wanted!

This is the sort of thing that further leads to email encryption being too complicated and too confusing for people. The process sucks, the level of assurance is low, and the authorities are signing agreements with subordinate organizations that are targetted specifically to generate valid recognizable certificates for services they don't run to do malicious things.

So lately I've been thinking that I'll just self-assure S/MIME like I do my gnupg identity. I already had a micro certificate authority anyway because I have an OS X Server host that runs a directory server and generates profiles for the devices I manage, so why not just sign my own certificates? Sure, that means when I email people that don't trust my certificate they see that they don't trust my certificate, but if they want to they can verify it with me, verify directly with me, or we can sign each other's keys and take a peer-to-peer approach to trust, which is probaby closer to how the technology was intended to be used anyway.

That was a little long-winded. So I'll move on the parts you care about:

My public [<span class="fa fa-lock"></span> certificate](files/EmoryLundberg.cer) is available for your importing. You may trust it however you see fit. If you want to, you can also import and/or trust [<span class="fa fa-lock"></span> my household's Root Certificate Authority](https://pki.kvet.ch/ca/certificates/eyrie_Root.crt) by fetching and importing the KVETCH Complaint Department CA certificate. I also have an [Intermediate CA Certificate](https://pki.kvet.ch/ca/certificates/eyrie_Intermediate.crt) for you that will sign device, service, and end-user certificates. Ask me if you want to send me a CSR or otherwise create a more formal crypto relationship. Read more about the [Eyrie CA](https://pki.kvet.ch/) if you're interested in my household PKI. I added another intermediate for my new homenet (`estuary`) as opposed to the old one (`eyrie`) and I have to tidy that up still. Regardless, if you get an email from me, it was probably signed with something, and you can decide what you want to do with it, but my certificate has undergone more scrutiny than a free one from Comodo even if it was done myself. Maybe I should set up distributed hellyeah! certificate authority that can issue certs signed by myself or one of the other slackers, I'll bring it up on Slack.

<img src="/assets/images/comeatmebro.jpg" class="img-rounded">

[^1]: Just because I'm O.G. doesn't mean that you must feel the need to recognize.

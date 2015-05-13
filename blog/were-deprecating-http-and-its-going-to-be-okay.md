<figure>
<img title="the internet forever" src="https://konklone.com/assets/images/blog/deprecating-http/deprecating-http.jpg" />
</figure>

Mozilla recently announced their **[intent to deprecate the insecure HTTP protocol in Firefox](https://blog.mozilla.org/security/2015/04/30/deprecating-non-secure-http/)**. In practice, they plan to do this by gradually removing the ability for HTTP websites to use various web features. They're joined by the Chrome security team, which declared something similar in December.

Mozilla's announcement has gotten a lot of attention, more than Chrome's, and much of it negative. There have been various laments, but the most sincere and helpful one is Ben Klemens' ["HTTPS: the end of an era"](https://medium.com/@b_k/https-the-end-of-an-era-c106acded474):

> But the Mozilla foundation’s HTTPS requirement is, to me, the real end of the DIY era. This is not a closed-source corporation, or a startup pushing its new tool, or the arrogant guy at the hackathon, but the Mozilla Foundation — “Our mission is to promote openness, innovation & opportunity on the Web” — saying that if you are building web pages using tools from your desert island, without first filling in registration forms, then you are doing it wrong.

I understand the fear of raising the barriers to entry. As a child, I too fell in love with an internet made by everyone, and have spent my [career](https://konklone.com/resume), my [volunteer work](___), and my [hobbies](___) trying to share what that love has taught me. I want children everywhere in the world to grow up feeling like the internet that permeates their lives is also in their service -- a lego set in real life that you can buy with a week's allowance.

As an adult, I also understand that power for ordinary people is hard to come by and hard to keep. The path of least resistance for human society is for money to buy more money, and might to demand more might. Democracy is designed not so much to expand freedom as it is to give people tools to desperately hold onto the freedom they have.

Put another way: power has a way of flowing away from the varied, strange, beautiful little leaf nodes and into the unaccountable, unimaginative, ever-hungry center.

TCP/IP, DNS, and the web were each tremendous reversals of this trend, freely giving the means of production to all of us little leafs. It felt like the powers that be just didn't realize what was happening until it was too late.

But when I look at the last few years, I see a very different web than the one I was introduced to:

* Verizon [injects tracking headers](http://www.forbes.com/sites/kashmirhill/2014/10/28/find-out-whether-this-privacy-killing-super-cookie-is-on-your-phone/) into unencrypted traffic so they can sell your browsing activity to advertisers. This program started in 2012, after [Verizon realized](http://www.fiercemobileit.com/story/verizon-app-usage-monitoring-raises-consumer-privacy-fears/2012-10-16) they "had a latent asset", but wasn't noticed until 2014.
* Other companies like Turn [piggyback on Verizon's tracking header](http://webpolicy.org/2015/01/14/turn-verizon-zombie-cookie/) to sell your data to even more people, because they "are trying to use the most persistent identifier that we can in order to do what we do", says Turn's **chief privacy officer**.
* Comcast [injects ads](http://arstechnica.com/tech-policy/2014/09/why-comcasts-javascript-ad-injections-threaten-security-net-neutrality/) into unencrypted traffic, because "it's a courtesy, and it helps address some concerns that people might not be absolutely sure they're on a hotspot from Comcast".
* Andreas Gal (Mozilla's CTO, in his personal capacity) [has claimed that Yahoo and Bing](http://andreasgal.com/2015/03/30/data-is-at-the-heart-of-search-but-who-has-access-to-it/) "can acquire search traffic by working with large Internet Service providers" to harvest users' Google search results to improve their own -- and strongly implies that they used to do this before Google shut them out through encryption.
* The nation of India [tried and failed to ban all of GitHub](http://techcrunch.com/2014/12/31/indian-government-censorsht/). HTTPS meant they [couldn't censor individual pages](http://ben.balter.com/2015/01/06/https-all-the-things/), and GitHub is too important to India's tech sector for them to ban the whole thing.
* The [nation of China weaponized the browsers of users all over the world](http://www.vox.com/2015/3/30/8315281/github-chinese-ddos-attacks) to attack GitHub for hosting anti-censorship materials (since like India, they can't block only individual pages) by [rewriting Baidu's unencrypted JavaScript files in flight](https://citizenlab.org/2015/04/chinas-great-cannon/).

And I haven't even mentioned the subject that got me and a lot of other people thinking differently about the network -- government surveillance:

* The [NSA](https://www.nsa.gov) scans [just about everything that goes through the internet backbones](https://en.wikipedia.org/wiki/XKeyscore) and saves as much of it as possible, in collaboration with intelligence agencies around the world. This is called "upstream collection", and their "posture" is to ["collect it all"](https://www.aclu.org/files/natsec/nsa/20140722/New%20Data%20Collection%20Posture.pdf).
* The NSA's upstream collection program has not been reformed. It [will not be reformed](https://www.eff.org/deeplinks/2015/05/usa-freedom-markup-glimpse-fight-reform-section-702) by the current draft of the USA Freedom Act, in fact was [endorsed by the only government agency](http://www.nytimes.com/2014/07/03/world/privacy-board-backs-nsa-program-that-taps-internet-in-us.html) whose job it is to review it, and the [most meaningful court victory so far](http://www.theverge.com/2015/5/7/8565111/appeals-court-rules-against-nsa-phone-collection-aclu-clapper) -- while a wonderful and important precedent -- addresses a separate program that only touches data about telephone calls.
* After the Charlie Hebdo attacks, France is now [making bulk internet spying explicitly legal](http://www.nytimes.com/2015/05/06/world/europe/french-legislators-approve-sweeping-intelligence-bill.html?_r=0) and giving its intelligence services vast powers to work with ISPs to surveil the network.
* The United Kingdom is likely to do something similar, after Cameron's [strong re-election](http://www.nytimes.com/2015/05/09/world/europe/david-cameron-and-conservatives-emerge-victorious-in-british-election.html) means he can make good on [his pledge to make all online communication subject to monitoring](http://www.telegraph.co.uk/technology/internet-security/11340621/Spies-should-be-able-to-monitor-all-online-messaging-says-David-Cameron.html).

When I look at all these things, I see companies and government asserting themselves over _their_ network. I see a network that is not just overseen, but actively hostile. I see an internet being steadily drained of its promise to ["interpret censorship as damage"](https://en.wikiquote.org/wiki/John_Gilmore).

In short, I see power moving away from the leafs and devolving back into the center, where power has been used to living for thousands of years.

We really can alter this dynamic by making strong encryption ubiquitous, and on the web that means HTTPS. We can force online surveillance to be as narrowly targeted and inconvenient as law enforcement was always meant to be. We can force ISPs to be the neutral commodity pipes they were always meant to be.

Richard Barnes, the author of Mozilla's HTTP deprecation announcement and policy, [responded to Ben](https://medium.com/@rlbarnes/hey-ben-this-is-richard-the-guy-who-wrote-the-blog-post-that-kicked-this-all-off-thanks-for-59e8a013b68a), saying:

> As I've said in some other threads on this topic, I'm under no illusion that HTTPS or the CA system is perfect. But to quote the great sage Mr. Rumsfeld, "you go to war with the army you have, not the army you might want or wish to have at a later time." Our long experience with HTTPS shows that it’s strong enough to carry the web, and it looks like its weaknesses can be patched. Which is enough, at least for me, to get the movement started.

Starting that movement doesn't happen in a vacuum. [Chrome is there](https://www.chromium.org/Home/chromium-security/marking-http-as-non-secure), the [IETF](https://datatracker.ietf.org/doc/rfc7258/) and [W3C TAG](http://www.w3.org/2001/tag/doc/web-https) are there. That kind of movement can become self-fulfilling, motivating more people and work than anyone thought possible at the start.

There are plenty of folks who feel like HTTPS configuration and the CA system need to become painless before we can make it the new standard. However, this has cause and effect backwards: the only way to motivate the investment necessary to make HTTPS free, easy, and everywhere is to make it part of the baseline, like DNS is today. There's no other way, and with what the network has become in 2015, there's no other choice.

The transition to HTTPS won't be painless, but it is necessary, and it will get better every year. The web will evolve, and when it does we'll have pushed some of its power back out of the center and into its edges for another generation to wield, love, and defend.
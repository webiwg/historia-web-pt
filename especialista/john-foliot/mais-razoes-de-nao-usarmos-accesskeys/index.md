---
layout: translation
date: 2013-12-04 # Data de ultima atualização do original
title: "How to make your wireframes more accessible in five easy steps" # Titulo traduzido
description: "In a non-scientific study conducted in the summer of 2002, we researched
the availability of available Accesskeys which had not already been reserved by various
other software technologies which might be employed by various users. "

copyright: 'Copyright John Foliot, via WATS.ca' # Quem tem direitos de cópia
license: null # Caso seja uma licença padrão (MIT, GPL...) por aqui
license-custom: null # Caso a licença não seja uma padrão, por uma descrição curta dela aqui
authors: [{
    name: "John Foliot",
    link: "https://twitter.com/johnfoliot"
}]
translators: [{
    name: "Nome Do Futuro Tradutor Aqui",
    link: "http://twitter.com/webiwg"
}]
reviewers: []
discussion: https://github.com/webiwg/acessibilidade-web-pt/issues/11
original: {
    title: "Accesskeys and Reserved Keystroke Combinations", # Titulo original, no idioma origial
    link: "http://john.foliot.ca/accesskeys-and-reserved-keystroke-combinations/", # Link para documento original
    dateOfTranslation: "2016-10-07" # Data em que a tradução foi finalizada
}
isDraft: true
isReleaseCandidate: false
---

> Prologue
> --------
>
> Back in the early 2000′s,
> my colleague and friend [Derek Featherstone](http://simplyaccessible.com/)
> and I launched a joint consultancy group in Ottawa,
> Canada that focused on the issues of on-line accessibility,
> and the emergent techniques and requirements of this (at the time) new aspect of web development.
> Derek and I wrapped up WATS.ca somewhere around 2006 as we moved on to other projects,
> but we both remain active in the field today.
>
> We jointly published a number of articles on our web-site that often became go-to references then,
> and it seems a shame that they be lost to the vagaries of time;
> the original site long since gone.
> I have created an Archive section of this site to preserve those postings,
> and the following article from that time is one such.
> Please note that some of the information in this or other similar articles may be dated,
> or superseded by events in time:
> I am making no attempt to update these articles and am simply posting them as they existed when they were first written.

By: Derek Featherstone | Posted: December 06, 2003

#### Related

-   [Using Accesskeys – Is it worth
    it?](//john.foliot.ca/using-accesskeys-is-it-worth-it/)
-   [Accesskeys and Reserved Keystroke
    Combinations](//john.foliot.ca/accesskeys-and-reserved-keystroke-combinations/)
-   [Link Relationships as an Alternative to
    Accesskeys](//john.foliot.ca/link-relationships-as-an-alternative-to-accesskeys/)
-   [The Future of Accesskeys](//john.foliot.ca/the-future-of-accesskeys/)

The topic of accesskeys regularly appears on mailing lists, forums, and other arenas.
Developers ask what the concensus is, and the answer is — there isn’t one.
We believe that the functionality accesskeys provide is worthwhile,
but their implementation and standardization leave something to be desired.

Accesskeys
----------

In general, HTML defined accesskeys are being used to provide the ability to quickly invoke the links in a site that go to specific destinations including such examples as a search page,
a contact page or the home page of a site.
In some cases they are being used to provide an alternative mechanism to “skip navigation” or “skip to content”.
In principle, we agree that this functionality is a worthwhile end goal as it has the potential to make the web more usable for all.

The Ideal Solution
------------------

We also firmly believe there have to be a number of conditions for accesskeys to be not only useful,
but successfully implemented on a large scale.
These include:

Standardized implementation across sites
:  The reason behind this is obvious.
   If it isn’t standardized, then users will have to learn different accesskeys on each site they visit.
   Many sites and authors have suggested different standards, with the most widely referenced being that at
   <a href="//clagnut.com/accessibility" class="broken_link">Clagnut</a> and
   [DiveIntoAccessibility.org](//www.diveintoaccessibility.org/accessibility_statement.html)
   that use numbers for Accesskeys, similar to that
   <a href="//www.e-envoy.gov.uk/Resources/WebHandbookIndex1Article/fs/en?CONTENT_ID=4000092&amp;chk=XHiT3L" class="broken_link">recommended by the Government in the UK</a>.

Conflict resolution
:  In cases where a conflict exists between an HTML defined Accesskey and a built in keyboard binding for a given User Agent or a user-defined keyboard binding in a user agent,
   the HTML defined Accesskey **must not** override the User Agent’s behaviour.
   If an HTML defined accesskey were to take precedence over a User Agent keyboard binding,
   critical functionality could be lost,
   potentially leaving the user confused,
   or unable to complete tasks.

Standardization
---------------

Standardization itself is not so much of a problem as is conflict resolution.
Thankfully, many developers have come to this realization,
and have worked toward standardizing accesskeys,
and an emerging trend is to use the digits 0 though 9,
instead of letters.

### The Problem with Letters and Learned Behaviours

The problem with letters is obvious –
HTML defined accesskeys appear to conflict with User Agent defined keyboard bindings to menus and other functionality.

In these cases of apparent conflict, the HTML defined accesskey can be invoked differently than the User Agent menus
(see: relevant discussion on the [WAI list](//lists.w3.org/Archives/Public/w3c-wai-ig/2003AprJun/0612.html),
and on the [WebAIM list](//webaim.org/discussion/mail_message.php?id=2270))

The problem with this is that it will be extremely difficult to teach new keystroke behaviour to users,
and there is no easy way to determine which keystroke method to use as there is generally no method for determining the accesskeys on a site when you first arrive at it
(hence the reason many sites now use Alt-0 to display their accessibility statement and list of accesskeys,
and others are using different methods to display the accesskeys inline within the document.)

### The Problem with Symbols

In the summer of 2002, [we collected as much information as we could](//john.foliot.ca/accesskeys-and-reserved-keystroke-combinations/)
regarding which keystroke combinations were “reserved” in user agents and assistive devices.

There remained some symbols available,
but symbols are problematic,
especially when dealing with International keyboards layouts.


<!--
  TODO terminei de formatar aqui. Vou dormir. Outra hora continuo formatando (fititnt, 2016-10-06 04:10)
-->



### The Problem with Numbers

Numbers seem to be a reasonable alternative, and a strategy many are now using.
There is however, a catch.

Current and previous versions of WindowEyes software use Alt+0 through Alt+9 to
reference “User-defined windows” that outline specific areas of the screen. From
the WindowEyes User Manual at
<a href="//www.gwmicro.com/wemanual/section4_2.htm" class="broken_link">http://www.gwmicro.com/wemanual/section4_2.htm</a>
(framebuster script means we can’t link directly to that page, so look for
section 4.2 in the contents frame on the left).

> Window-Eyes has two kinds of windows, standard and hyperactive. Standard user
> windows are for reading portions of the display screen while ignoring other
> portions. They can be set to any size, from one character to the entire
> display screen. You can read the contents of any of the first twenty standard
> windows with the press of a hot key. Windows 0 through 9 can be read with
> ALT-0 through ALT-9. Windows 10 through 19 have their hot keys undefined by
> default. Any of the 50 standard windows can be read with the Any Window hot
> key, undefined in the default Window-Eyes speaking environment. Though fifty
> standard user windows are available, few speech-access users ever need to use
> all, or even most of them.

Users using WindowEyes will not have access to numeric accesskeys. Many will
argue that defining the accesskeys with numbers for everyone else will be of
use, as long as defining them doesn’t override any expected behaviour of user
agent, or assistive technology such as WindowEyes. This seems reasonable, but
certainly not universal, and we believe that a universal solution would be
preferable.

### The Problem with Opera and Numbers

Actually, there appears to be more than one catch when using numeric accesskeys.
While Opera supports numeric accesskeys, the mechanism to activate them differs
from activating letter assigned accesskeys. In Opera, to activate a letter
accesskey, you hold down Shift + Esc + letter. When using numbers on the other
hand, you must press Shift + Esc, let go, and then press the number.

This becomes more problematic as the number keys also have functionality within
Opera including:

-   Number 0: Zoom in 10%
-   Number 9: Zoom out 10%
-   Number 8: Zoom in 100%
-   Number 7: Zoom out 100%
-   Number 6: Restore to 100%
-   Number 3: Cycle through frames on a page
-   Number 2: Cycle to next page
-   Number 1: Cycle to previous page
-   Number 4: Minimize active Page
-   Number 5: Switch between restored and maximized page

This means that if you don’t press the number soon enough after you’ve pressed
and released Shift + Esc, you will invoke the default number behaviour instead
of the element to which the accesskey is assigned. We haven’t gone to the point
of measuring what factors determine how much delay is given between the
keystrokes before the behaviour reverts to the default instead of the accesskey.
Perhaps some day.

Conflict Resolution
-------------------

The W3C User Agent Guidelines don’t specifically spell out what should happen in
cases of conflict between locally/document defined keyboard bindings and user
agent/OS keyboard bindings. However, it seems logical that a document that
includes “Guideline 11. Allow configuration and customization”, would suggest
that such customization is done at the User Agent level, and that these settings
would override the settings of the individual document. We already have this
case with user defined stylesheets.

In any case, we should expect that the user agent settings would override
anything that the author puts in place, because the user agent is presumably
configured by the end user.

It appears that this is not the case in certain instances.

### Mozilla and Conflicts with Extensions

**Updated April 9, 2004**: [Mozilla](//www.mozilla.org/) and other Gecko based
user agents such as [FireFox](//www.mozilla.org/products/firefox/) have the
advantage of being customizable through extensions that are written by third
parties. One of the more popular is the [RSS Reader
Panel](//extensionroom.mozdev.org/more-info.php/rssreaderpanel). When installed
it displays a list of RSS Bookmarks in the Mozilla sidebar, along with a list of
items in the RSS feed. The RSS Reader Panel is toggled on and off using the ALT
+ R keystroke (on a PC). We recently experienced that this was overridden by
accesskeys that were author defined in a page we were browsing. What made this
more confusing was the fact that the accesskeys were not visibly identified on
the page. The accesskey simply hijacked the keystroke.

It is foreseeable that many more conflicts are possible as the number of third
party extensions increases. Again, the question arises – in cases of conflict,
who wins? Clearly we don’t want accesskeys to override behaviours of the user
agent.

### WindowEyes, IE, and ALT + S

WindowEyes defines the keystroke ALT + S as a function that reads that status
bar. Including S in your list of accesskeys will not work with current versions
of WindowEyes.

### IE and ALT + D

Internet Explorer binds the keystroke ALT+D to the address bar. An HTML defined
accesskey for the letter D overrides the keyboard binding to the address bar,
and therefore disables that critical keyboard shortcut for IE users. This is the
perfect example of where accesskeys can go wrong, as it is the exact opposite of
what we believe should happen in terms of conflict resolution.

A note on International versions of IE — we installed and tested the latest
version of IE in other languages (Spanish and Italian) wondering if the same
problem might occur, but with different letters. Interestingly enough, the ALT +
D combination was used to focus on the address bar as well simply because the
letter d was in the translated version of “Address” in each of the languages we
tested. If you have another version of IE in a different language that uses a
key other than D to focus on the address bar, please let us know so that we can
update our references.

JAWS screen reading software absolutely relies on keystrokes, as does
WindowEyes. These screen readers run “on top of” the other software on the users
computer, and in most cases for the web, on top of Microsoft Internet Explorer.
Further, IBM’s HomePageReader utilizes IE’s rendering engine to read web pages.
It too, relies heavily on keystrokes to function. In these cases where
keystrokes are vital, the potential for confusion and problems is greater.

These (admittedly obscure) cases show disparity within a single browser where
the user agent recovers nicely on conflict for certain key bindings and in
others it (quite unexpectedly) overrides default behaviour. Without clear
concensus from the browser makers on conflict resolution and which keyboard
binding should take priority, implementing accesskeys successfully becomes even
more difficult. User preferences should take precedence over author preference.
Certainly the possibility exists that there are other such conflicts that may
exist in different user agents/adaptive technology combinations.

The Way Forward
---------------

We want to make sure we are clear on one thing. We like the concept behind
accesskeys, we just believe there is too much wiggle room, even though others
have recommended “standards”. The problem is that it still isn’t standard. We
did a [search for UK Government Accesskeys
standards](//www.google.com/search?ie=UTF-8&oe=UTF-8&sourceid=deskbar&q=UK+Government+Accesskeys+Standards)
and found sites that claimed to be following the standards using numeric
accesskeys, but then went on to declare additional accesskeys that included many
letters, and in some cases included S and D – unfortunate choices given the
above conflicts.

We do support the idea, but believe we all need a different and more robust way
to implement the same functionality.

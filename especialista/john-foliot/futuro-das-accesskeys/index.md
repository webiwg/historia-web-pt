January 15, 2013

<img src="http://john.foliot.ca/wp-content/uploads/2013/01/accesskeys.jpg" alt="accesskeys" class="aligncenter size-full wp-image-465" sizes="(max-width: 620px) 100vw, 620px" srcset="http://john.foliot.ca/wp-content/uploads/2013/01/accesskeys.jpg 620w, http://john.foliot.ca/wp-content/uploads/2013/01/accesskeys-300x109.jpg 300w" width="620" height="226" />

Prologue
--------

Back in the early 2000′s,
my colleague and friend [Derek Featherstone](http://simplyaccessible.com/)
and I launched a joint consultancy group in Ottawa,
Canada that focused on the issues of on-line accessibility,
and the emergent techniques and requirements of this (at the time) new aspect of web development.
Derek and I wrapped up WATS.ca somewhere around 2006 as we moved on to other projects,
but we both remain active in the field today.

We jointly published a number of articles on our web-site that often became go-to references then,
and it seems a shame that they be lost to the vagaries of time;
the original site long since gone.
I have created an Archive section of this site to preserve those postings,
and the following article from that time is one such.
Please note that some of the information in this or other similar articles may be dated,
or superseded by events in time:
I am making no attempt to update these articles and am simply posting them as they existed when they were first written.


By: Derek Featherstone | Posted: August 14, 2004

#### Related

-   [Using Accesskeys – Is it worth
    it?](//john.foliot.ca/using-accesskeys-is-it-worth-it/)
-   [More reasons why we don’t use
    accesskeys](//john.foliot.ca/more-reasons-why-we-dont-use-accesskeys/)
-   [Accesskeys and Reserved Keystroke
    Combinations](//john.foliot.ca/accesskeys-and-reserved-keystroke-combinations/)
-   [Link Relationships as an Alternative to
    Accesskeys](//john.foliot.ca/link-relationships-as-an-alternative-to-accesskeys/)

The July 22, 2004 Working Draft of XHTML 2.0 abandons accesskey for a much more
powerful and flexible access attribute that will put the user in control and
allow keyboard users to define their own keystrokes.

For over a year we’ve written at length about some of the problems with
accesskeys. It started with our piece [Using Accesskeys: Is it worth
it?](http://john.foliot.ca/using-accesskeys-is-it-worth-it/) and has continued
from there. We’ve done a lot of research on [accesskey
availability](http://john.foliot.ca/more-reasons-why-we-dont-use-accesskeys/),
found [keystroke
conflicts](http://john.foliot.ca/accesskeys-and-reserved-keystroke-combinations/),
and [proposed alternatives to
accesskeys](http://john.foliot.ca/link-relationships-as-an-alternative-to-accesskeys/)
that put the user in control, rather than the author.

During that year, I can’t count the number of times that I’ve written statements
like this at
<a href="http://www.accessifyforum.com/" class="broken_link">AccessifyForum.com</a>,
on mailing lists and in comments on blogs – one of which was on [Dave
Shea](http://www.mezzoblue.com/)‘s post “[I do not use
accesskeys](http://www.mezzoblue.com/archives/2003/12/29/i_do_not_use/).”

1.  We like the idea behind accesskeys,
2.  We find the implementation very problematic
3.  We believe that we collectively need to examine the issue and determine if
    we need to develop other solutions that better suit the needs of everyone.

Through all of those articles it boils down to a few key points:

-   authors (usually) define (too many) accesskeys
-   accesskeys are used inconsistenly across sites, meaning they are of
    generally limited use
-   accesskeys cause conflict with other keystrokes
-   current user agents do not allow accesskeys to be turned off, nor defined by
    users

We often re-examine our thoughts on accesskeys. We believe they can be of some
value — most likely used in well-defined web-based applications like
[WordPress](http://www.worpress.org/) or [Basecamp](http://www.basecamphq.com/).
However, even when they are in use in these environments I still don’t have the
option of turning them off, nor can I override them with my own keys. I believe
that there just isn’t enough flexibility in current browsers to make accesskeys
as useful as they should (or could) be.

A new strategy
--------------

It appears that a new strategy has emerged. Instead of defining “keystrokes”
with the accesskey attribute, the [XHTML 2.0 Working Draft (July 22,
2004)](http://www.w3.org/TR/2004/WD-xhtml2-20040722/) takes a big step forward
to addressing the issues with accesskeys by dropping the accesskey attribute and
introducing the [access
attribute](http://www.w3.org/TR/2004/WD-xhtml2-20040722/mod-hyperAttributes.html#adef_hyperAttributes_access).
This is new in the July 22, 2004 Working Draft. The previous version ([XHTML 2.0
Working Draft (May 6, 2004)](http://www.w3.org/TR/2003/WD-xhtml2-20030506/)) did
not have the access attribute, and still made reference to the accesskey
attribute.

**This will allow authors to define access points instead of keystrokes**.

Here’s what we see as the most important point from the working draft:

> The invocation of access shortcuts, and the assignment of key or other
> bindings to them is not further defined here. A user agent should allow the
> user to access the user agent’s list of recognized access points, to add to
> them, and to specify bindings for them.

This significant change means a few things:

1.  **Authors will no longer have to worry about keystroke conflicts** because
    it is no longer their job to define keystrokes. Authors will also need to
    adjust to the fact that they no longer have control.
2.  Authors can focus on **defining logical and meaningful access points** in
    their documents
3.  **Users** that really need and could benefit from this functionality can
    **define their own keystrokes**, eliminating/minimizing conflict with
    their software.
4.  **Users get consistency across sites** because the keystrokes are defined at
    the browser level. No more remembering what keystrokes do what on
    which sites.

Anyone who has read our other articles on accesskeys will hopefully recognize
that we are incredibly happy with these changes – they closely resemble what
we’ve been hoping for and writing about for the past year, albeit in a slightly
different format.

Recognized access points
------------------------

This strategy requires clearly defined access points. Perhaps the well-defined
link relationships and expanding on those as needed would be a good place to
start. These would include obvious access points such as Search, Home, Help,
Contact, and could be expanded to include others such as content, form,
accessibility, privacy, navigation and others. We discussed this earlier in
[Link Relationships as an Alternative to
Accesskeys](http://john.foliot.ca/link-relationships-as-an-alternative-to-accesskeys/)

The working draft notes: “A list of access points (such as ‘main content’,
‘navigation list’, ‘submit button’ is in preparation.”

My instinct tells me that single word access points would be better, though I
can’t say for certain that one word would always be appropriate. “Submit button”
could just as easily be “Submit”. (One other note regarding the use of “Submit”
as an access point – I’m assuming that the behavior would be to focus on the
submit button rather than actually submit the form, otherwise we’ll see obvious
problems on pages with more than one form.)

User Customization
------------------

This working draft recognizes that keyboard users are best equipped to edit and
add to the keystrokes *they* need is a very big step forward, and fits with most
of what good design and standards is about. **People, and putting people in
control of their own environment**. I’m sure my friend [Patrick Lauke
(redux)](http://www.splintered.co.uk/) will be as happy as we are with this one
— the onus is on both the author (to define the access points) and the user (to
do something meaningful with them).

This strategy allows me as the user to define keystrokes that work across all
sites that implement these access points, and it allows me to create a highly
customized set of keystrokes for working with various web applications that
define additional access points. If I want Ctrl + Shift + H to take me to the
home page, and Ctrl + Shift + S to take me to the search form or page for a
site, then it will work on any site where these access points have been defined.

Access &gt; Accesskey
---------------------

Looking forward, it might even be useful to allow for user agents to allow
loading of custom keystroke profiles so that users can create and save different
sets of keystrokes for use in different applications. That way I could easily
define keystroke mappings for WordPress and another set for Basecamp. Now that
would be useful. Site authors could also provide an XML version of the access
points defined with the access attribute so that users could import the access
points directly into one of those custom profiles.

We believe that this new strategy provides much more power and is much more
useful than the current accesskey. Unfortunately it may be some time before we
realize the benefits of this change in strategy, as XHTML 2.0 may be a long way
from the mainstream, and in order to make this strategy successful, user agents
need to change to allow this level of customization. [The Opera
browser](http://www.opera.com/) is already a leader in this respect as they
allow the user to create highly customized keystrokes and multiple keyboard
configurations through their Preferences interface. Let’s hope that other user
agents can catch up.

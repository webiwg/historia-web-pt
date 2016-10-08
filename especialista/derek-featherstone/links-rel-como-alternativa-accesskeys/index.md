---
layout: translation
date: 2013-12-06 # Data de ultima atualização do original
title: "Link Relationships as an Alternative to Accesskeys" # Titulo traduzido
description: "We like the concept of accesskeys providing quick keystroke access to various parts of a particular site.
However, we also believe that given their standardization and implementation problems, we need a more robust method for providing the functionality."

copyright: 'Copyright Derek Featherstone, via WATS.ca' # Quem tem direitos de cópia
license: null # Caso seja uma licença padrão (MIT, GPL...) por aqui
license-custom: null # Caso a licença não seja uma padrão, por uma descrição curta dela aqui
authors: [{
    name: "Derek Featherstone",
    link: "https://twitter.com/johnfoliot"
}]
translators: [{
    name: "Nome Do Futuro Tradutor Aqui",
    link: "http://twitter.com/webiwg"
}]
reviewers: []
discussion: https://github.com/webiwg/historia-web-pt/issues/9
original: {
    title: "Link Relationships as an Alternative to Accesskeys", # Titulo original, no idioma origial
    link: "http://john.foliot.ca/link-relationships-as-an-alternative-to-accesskeys/", # Link para documento original
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


We like the concept of accesskeys providing quick keystroke access to various parts of a particular site.
However, we also believe that given their standardization and implementation problems,
we need a more robust method for providing the functionality.

Link Relationships as an Alternative to Accesskeys
--------------------------------------------------

Many sites use Accesskeys as a means to quickly access certain navigational items in their documents.
The implementation of Accesskeys however,
seems to be fraught with implementation problems,
despite the fact that many developers are attempting to provide a standardized "map" for the accesskeys on a site.

We’ve [questioned whether or not implementing accesskeys is worth it](//john.foliot.ca/using-accesskeys-is-it-worth-it/),
and discussed some of the [pitfalls of working with accesskeys](//john.foliot.ca/more-reasons-why-we-dont-use-accesskeys/) before,
and indeed [there are very few keystroke combinations that are available for use](//john.foliot.ca/accesskeys-and-reserved-keystroke-combinations/).
Despite the fact that we agree that Accesskey functionality is useful,
we still think there should be an alternative to accesskeys that could provide the same functionality of accesskeys but without the “standardization” problems,
and with little to no conflict in the implementation.


Accesskey Standardization
-------------------------

Accesskeys are usually defined for a few very common items found in web sites such as:
Home page, Skip Navigation, Table of contents, Search, Terms of use, Contact, Feedback, Copyright, Accessibility statement, and others.
Although there may be some slight differences between some of these items
(i.e., Contact vs. Feedback, Terms of Use vs. Copyright),
it is forseeable that we come up with standard terms for these that could be used across sites.

This functionality already exists via the underused `link` element.

Many of these commonly accessed items are predefined as [valid link relationship types](//www.w3.org/TR/html4/types.html#type-links).
So why not expand on those relationships to include oft used accesskey relationships?
Then we could all embed the data in the head of our documents:

```html
   <link rel="home" href="/"  />
   <link rel="copyright" href="/policies/" />
   <link rel="search"  href="/search/" />
   <link rel="contact"  href="/contact/" />
   <link rel="accessibility"  href="/accessibility/" />
```

Now that the relationship and the target is defined, we move to implementation.

Allowing Keystroke access to Link Relationships
-----------------------------------------------

An ongoing problem with accesskey implementation is avoiding conflict with other pre-defined keystrokes.
Rather than allowing the user agent to predetermine the method by which accesskeys are invoked
(Alt + \_ in PC Internet Explorer, Netscape, Mozilla, Ctrl/Cmd + \_ in Mac IE/Netscape/Mozilla, Shift + Esc + \_ in PC and Mac Opera)
perhaps we should take a page from many pieces of adaptive technology and allow the keystroke combination to be customized by the end user.

Instead of defining the key to be used itself we have defined the target.
Now all we need is to allow for the end user to choose how they wish to define the keystrokes.

This eliminates problems with accesskeys being defined differently across sites all over the World Wide Web.
I would love for the ability to always make Ctrl + Shift + H take me to the home page of the site I am on,
Ctrl + Shift + S to take me to search for that site,
and for Ctrl + Shift + C to take me to the contact page/form.

As users, we could all get our own way, and we don’t have to learn how to have keystroke access to everyone’s site,
we just learn how to do it within our preferred “smart” user agent.
As developers, we could work to define relationships and targets rather than keystrokes that may or may not conflict with keystrokes already defined within a user agent or other piece of technology.

This would appear to be consistent with various components of the [User Agent Accessibility Guidelines](//www.w3.org/TR/UAAG10/) in terms of providing user definable keystroke access to various user agent functions.

---
layout: translation
date: 2003-04-08 # Data de ultima atualização do original
title: "Using Accesskeys – Is it worth it?" # Titulo traduzido
description: "The Accesskey attribute assigns an access key to an element.
An access key is a single character from the document character set.
Pressing an access key assigned to an element gives focus to the element.
The action that occurs when an element receives focus depends on the element. "
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
discussion: https://github.com/webiwg/historia-web-pt/issues/6
original: {
    title: "Using Accesskeys – Is it worth it?", # Titulo original, no idioma origial
    link: "http://john.foliot.ca/using-accesskeys-is-it-worth-it/", # Link para documento original
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


Using Accesskeys – Is it worth it?
----------------------------------


The [Accesskey attribute](http://www.w3.org/tr/html401/interact/forms.html#adef-accesskey) assigns an access key to an element.
An access key is a single character from the document character set.
Pressing an access key assigned to an element gives focus to the element.
The action that occurs when an element receives focus depends on the element.
For example, when a user activates a link defined by the A element, the user agent generally follows the link.
When a user activates a radio button, the user agent changes the value of the radio button.
When the user activates a text field, it allows input, etc.

The following elements support the accesskey attribute:
`A`, `AREA`, `BUTTON`, `INPUT`, `LABEL`, and `LEGEND`, and `TEXTAREA`.

The invocation of access keys depends on the underlying system.
For instance, on machines running MS Windows, one generally has to press the <kbd>alt</kbd> key in addition to the access key.
On Apple systems, one generally has to press the <kbd>cmd</kbd> key in addition to the access key.

The rendering of access keys depends on the user agent.

### Using HTML designated access keys:

-   Windows Operating System/MSIE: <kbd>Alt</kbd> \[key number\] Enter
-   Windows Operating System/Mozilla, Netscape, K-Meleon: <kbd>Alt</kbd> \[key number\]
-   Windows Operating System/Opera: <kbd>Shift</kbd> + <kbd>Esc</kbd> \[key number\]
-   Macintosh Operating System/MSIE: <kbd>Ctrl</kbd> \[key number\] Enter
-   Macintosh Operating System/Mozilla, Netscape: <kbd>Ctrl</kbd> \[key number\]
-   Macintosh Operating System/Opera: <kbd>Shift</kbd> + <kbd>Esc<kbd> \[key number\]
-   Linux Mandrake Operating System/Galeon/Mozilla: <kbd>Alt</kbd> \[key number\]

### Using HTML designated access keys:

-   Windows Operating System/MSIE: <kbd>Alt</kbd> \[key number\] Enter
-   Windows Operating System/Mozilla, Netscape, K-Meleon: <kbd>Alt</kbd> \[key number\]
-   Windows Operating System/Opera: <kbd>Shirft</kbd> + <kbd>Esc</kbd> \[key number\] Enter
-   Macintosh Operating System/MSIE: <kbd>Ctrl<kbd> \[key number\] Enter
-   Macintosh Operating System/Mozilla, Netscape: <kbd>Ctrl</kbd> \[key number\]
-   Macintosh Operating System/Opera: <kbd>Shirft</kbd> + <kbd>Esc</kbd> \[key number\] Enter
-   Linux Mandrake Operating System/Galeon/Mozilla: <kbd>Alt</kbd> \[key number\]

### Browsers that recognize HTML designated access keys:

-   MS Windows Internet Explorer (versions 4.xx and later)
-   Mozilla (9.xx builds, version 1.xx and later)\*
-   Netscape Navigator (version 6.xx and later)\*
-   Opera (PC version 7.x and later, Mac version 6.x and later)
-   K-Meleon (version 6.xx and later)
-   Spirit MetaBrowser (version 1.xx and later)
-   Galeon (version 1.xx and later)

### Browsers that do not recognize HTML designated access keys

1.  Opera (PC versions up to 7.x, Mac versions up to 6.x)
2.  Netscape Navigator (versions 4.xx)
3.  Konqueror (versions 2.xx)
4.  \* Under Mac OS 9, access keys are not supported by Internet Explorer 4,
    Internet Explorer 4.5, Mozilla, Netscape 4 and Opera 5.
5.  \* Under Mac OS X 10, access keys are not supported by Mozilla and
    OmniWeb 4.

Now for the bad news…
---------------------

In a non-scientific study conducted in the summer of 2002,
we researched the availability of available Accesskeys which had not already been reserved by various other adaptive technologies,
such as JAWS and IBM’s HomePageReader,
a popular screen reading web browser,
which has built in keystroke shortcuts for going into different modes.

-   <kbd>Alt</kbd> + <kbd>I</kbd> starts Read Items mode
-   <kbd>Alt</kbd> + <kbd>N</kbd> starts Windows Cursors reading mode
-   <kbd>Alt</kbd> + <kbd>W</kbd> starts Words reading mode
-   <kbd>Alt</kbd> + <kbd>C</kbd> starts Character reading mode (read character by character)
-   <kbd>Alt</kbd> + <kbd>L</kbd> starts Links reading mode (only read the links on the page)
-   <kbd>Alt</kbd> + <kbd>O</kbd> (letter O not number zero) starts Controls reading mode
-   <kbd>Alt</kbd> + <kbd>1</kbd> starts Heading reading mode (reading only the headings on a page)
-   <kbd>Alt</kbd> + <kbd>J</kbd> Table Jump
-   <kbd>Alt</kbd> + <kbd>T</kbd> Table Navigation
-   <kbd>Alt</kbd> + <kbd>D</kbd> Dial

HomePageReader makes no distinction between these keystrokes and will not allow you to use accesskeys.
Besides, their mechanism actually seems to make more sense —
using links mode to cycle through a list of links seems much more useful and usable.
(Interestingly, for accesskeys to work in HomePageReader,
the user must first “click” the mouse within the display screen of the application…
a curious requirement in a tool geared to the visually impaired…)

Disappointingly, our research discovered that all but 3 keys were previously “claimed” by one technology or the other:

-   AccessKey <kbd>/</kbd> (slash)
-   AccessKey <kbd>\</kbd> (backslash)
-   AccessKey <kbd>\</kbd> (right square bracket)

At that point it was then pointed out (by [Jukka “Yucca” Korpela](http://www.cs.tut.fi/~jkorpela/) –
a well respected accessibility expert) that even these keys would be inaccessible to users not using a North American Standard (QWERTY) keyboard.
**So while it seems that Accesskeys is a great idea in principle,
implementation brings with it the possibility that it either will not be available to all users,
or that the keystroke combination encoded within the web page may conflict with a reserved keystroke combination in an adaptive technology or future user agent.**

This potential problem was subsequently brought to the attention of the Canadian Common Look and Feel Access Working Group
(who had previously suggested the use of Accesskeys M, 1 and 2),
and after consideration the Access Working Group reversed it’s recommendation and now suggest **not** to use Accesskeys on Government of Canada Web sites.

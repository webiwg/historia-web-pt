---
layout: translation
date: 2013-12-04 # Data de ultima atualização do original
title: "Accesskeys and Reserved Keystroke Combinations" # Titulo traduzido
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
discussion: https://github.com/webiwg/historia-web-pt/issues/8
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

In a non-scientific study conducted in the summer of 2002,
we researched the availability of available Accesskeys which had not already been reserved by various other software technologies which might be employed by various users.
The results indicated a real problem in that most ALT + \_\_ keystroke combinations
(assuming the Windows operating platform) have already been reserved by one type of application or another.

Given that at this writing there are few if any available ALT + \_\_ keystrokes left,
and conceding that built in or assigned keystroke combinations inherent in software applications should take precedence for the end user, WATS.
ca continues to advocate that the ACCESSKEY element/attribute,
while a good idea in principle,
is fraught with so many potential problems that we have abandoned using them in the interest of true inter-operability.

While it would be presumptuous of us to declare this table “complete” it *does* illustrate the number of keystroke combinations which would conflict with implementation of the ACCESSKEY functionality introduced in HTML 4.0.
Errors, omissions or inclusions are gratefully appreciated and will be added to this page upon receipt.

We have included Opera for reference only.
We are aware that Opera doesn’t use the ALT + \_ keystroke to invoke accesskeys.
We also acknowledge that this appears Windows-centric and that other Operating Systems may invoke alternative modifier kyes to access the designated hot-key.

### Known reserved keystroke combinations

<table summary="Known reserved keystroke combinations"
  frame="hsides" border="1" cellpadding="3" cellspacing="0">
  <thead>
    <tr>
      <th> </th>
      <th>IE 5.5/6</th>
      <th>Firefox / NS 7 / Mozilla</th>
      <th>Opera 7</th>
      <th>IBM HPR</th>
      <th>JAWS Classic Settings (Using IE 5.5/6)</th>
      <th>JAWS Laptop Settings (Using IE
        <br> 5.5/6)
      </th>
      <th>Window Eyes (Using IE 5.5/6)</th>
      <th>
        <a href="//www.cs.utexas.edu/users/s2s/latest/jaws1/home/index.shtml" class="broken_link">
          <br> JAWSAssist Extension for FireFox
          <br>
        </a>
      </th>
    </tr>
  </thead>
  <tfoot>
    <tr>
      <th> </th>
      <th>IE 5.5/6</th>
      <th>Firefox / NS 7 / Mozilla</th>
      <th>Opera 7</th>
      <th>IBM HPR</th>
      <th>JAWS Classic Settings (Using IE 5.5/6)</th>
      <th>JAWS Laptop Settings (Using IE
        <br> 5.5/6)
      </th>
      <th>Window Eyes (Using IE 5.5/6)</th>
      <th>
        <a href="//www.cs.utexas.edu/users/s2s/latest/jaws1/home/index.shtml" class="broken_link">
          <br> JAWSAssist Extension for FireFox
          <br>
        </a>
      </th>
    </tr>
  </tfoot>
  <tbody style="height: 350px; overflow: scroll;">
    <tr>
      <td width="12">Alt+A</td>
      <td width="11">Favorites</td>
      <td width="11"> </td>
      <td width="11"> </td>
      <td width="11">Favorites</td>
      <td width="11">Favorites</td>
      <td width="11">Favorites</td>
      <td width="11">Favorites</td>
      <td width="11"> </td>
    </tr>
    <tr>
      <td>Alt+B</td>
      <td> </td>
      <td>Bookmarks</td>
      <td>Bookmark</td>
      <td> </td>
      <td> </td>
      <td>Read All Options in Dialog Box</td>
      <td> </td>
      <td>Bookmarks</td>
    </tr>
    <tr>
      <td>Alt+C</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Read Characters</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+D</td>
      <td>Address</td>
      <td>Address</td>
      <td> </td>
      <td>Dial</td>
      <td>Address</td>
      <td>Address</td>
      <td>Address</td>
      <td>Address</td>
    </tr>
    <tr>
      <td>Alt+E</td>
      <td>Edit</td>
      <td>Edit</td>
      <td>Edit</td>
      <td>Edit</td>
      <td>Edit</td>
      <td>Edit</td>
      <td>Edit</td>
      <td>Edit</td>
    </tr>
    <tr>
      <td>Alt+F</td>
      <td>File</td>
      <td>File</td>
      <td>File</td>
      <td>File</td>
      <td>File</td>
      <td>File</td>
      <td>File</td>
      <td>File </td>
    </tr>
    <tr>
      <td>Alt+G</td>
      <td> </td>
      <td>Go</td>
      <td> </td>
      <td>Go</td>
      <td> </td>
      <td>Use Graphics Wizard</td>
      <td> </td>
      <td>Go </td>
    </tr>
    <tr>
      <td>Alt+H</td>
      <td>Help</td>
      <td>Help</td>
      <td>Help</td>
      <td>Help</td>
      <td>Help</td>
      <td>Read Current Line</td>
      <td>Help</td>
      <td>Help </td>
    </tr>
    <tr>
      <td>Alt+I</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Read Items</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+J</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Table Jump</td>
      <td> </td>
      <td>Read Prior Word</td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+K</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Provide a list of Accesskeys for the current page</td>
      <td> </td>
      <td>Read Current Word / Spell Current Word (Key must be pressed twice within half
        a second for the spell function.)</td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+L</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Read Links</td>
      <td> </td>
      <td>Read Next Word</td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+M</td>
      <td> </td>
      <td> </td>
      <td>Mail</td>
      <td> </td>
      <td> </td>
      <td>Read Prior Character or Icon</td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+N</td>
      <td> </td>
      <td> </td>
      <td>Navigate</td>
      <td>Read Windows Cursor</td>
      <td> </td>
      <td>Read Next Line</td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+O</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Read Controls</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+P</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Activate JAWS Cursor</td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+Q</td>
      <td> </td>
      <td>QA (Mozilla Only)</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+R</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Turn JAWS Cursor Restriction On or Off</td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+S</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Settings</td>
      <td> </td>
      <td>Change Screen Echo</td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+T</td>
      <td>Tools</td>
      <td>Tools</td>
      <td> </td>
      <td>Table Navigation</td>
      <td>Tools</td>
      <td>Speak the Title of the Current Window</td>
      <td>Tools</td>
      <td>Tools </td>
    </tr>
    <tr>
      <td>Alt+U</td>
      <td> </td>
      <td>Debug (Mozilla Only)</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+V</td>
      <td>View</td>
      <td>View</td>
      <td>View</td>
      <td>View</td>
      <td>View</td>
      <td>Change Verbosity Level</td>
      <td>View</td>
      <td>View </td>
    </tr>
    <tr>
      <td>Alt+W</td>
      <td> </td>
      <td>Window</td>
      <td>Window</td>
      <td>Read Words</td>
      <td> </td>
      <td>Read the Application Window</td>
      <td> </td>
      <td>Window </td>
    </tr>
    <tr>
      <td>Alt+X</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+Y</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Read Prior Line</td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+Z</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+1</td>
      <td> </td>
      <td>Default English installation of Firefox on Linux uses Alt+(#) to shift tab
        focus when browsing multiple tabs</td>
      <td> </td>
      <td>Read Headings</td>
      <td> </td>
      <td> </td>
      <td>Reserved for User-defined windows</td>
      <td>Cycling Heading level 1</td>
    </tr>
    <tr>
      <td>Alt+2</td>
      <td> </td>
      <td>Default English installation of Firefox on Linux uses Alt+(#) to shift tab
        focus when browsing multiple tabs</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Reserved for User-defined windows</td>
      <td>Cycling Heading level 2</td>
    </tr>
    <tr>
      <td>Alt+3</td>
      <td> </td>
      <td>Default English installation of Firefox on Linux uses Alt+(#) to shift tab
        focus when browsing multiple tabs</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Reserved for User-defined windows</td>
      <td>Cycling Heading level 3</td>
    </tr>
    <tr>
      <td>Alt+4</td>
      <td> </td>
      <td>Default English installation of Firefox on Linux uses Alt+(#) to shift tab
        focus when browsing multiple tabs</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Reserved for User-defined windows</td>
      <td>Cycling Heading level 4</td>
    </tr>
    <tr>
      <td>Alt+5</td>
      <td> </td>
      <td>Default English installation of Firefox on Linux uses Alt+(#) to shift tab
        focus when browsing multiple tabs</td>
      <td> </td>
      <td> </td>
      <td>Say Sentence (Numberpad)</td>
      <td>Say Sentence (Numberpad)</td>
      <td>Reserved for User-defined windows</td>
      <td>Cycling Heading level 5</td>
    </tr>
    <tr>
      <td>Alt+6</td>
      <td> </td>
      <td>Default English installation of Firefox on Linux uses Alt+(#) to shift tab
        focus when browsing multiple tabs</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Reserved for User-defined windows</td>
      <td>Cycling Heading level 6</td>
    </tr>
    <tr>
      <td>Alt+7</td>
      <td> </td>
      <td>Default English installation of Firefox on Linux uses Alt+(#) to shift tab
        focus when browsing multiple tabs</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Reserved for User-defined windows</td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+8</td>
      <td> </td>
      <td>Default English installation of Firefox on Linux uses Alt+(#) to shift tab
        focus when browsing multiple tabs</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Left Mouse Click</td>
      <td>Reserved for User-defined windows</td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+9</td>
      <td> </td>
      <td>Default English installation of Firefox on Linux uses Alt+(#) to shift tab
        focus when browsing multiple tabs</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Right Mouse Click (Press this key twice within a second for a double mouse
        click.)</td>
      <td>Reserved for User-defined windows</td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+0</td>
      <td> </td>
      <td>Default English installation of Firefox on Linux uses Alt+(#) to shift tab
        focus when browsing multiple tabs</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Reserved for User-defined windows</td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+ `</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+ –</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Open a child window control menu</td>
      <td>Open a child window control menu</td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+ =</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+ (</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+ )</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Screen Sensitive Help</td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+ [</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+ ]</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+ </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+ /</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Speak Coordinates of Active Cursor</td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+ ;</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Activate PC Cursor</td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+ :</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+ ,</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Read Current Character</td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+ .</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td>Read Next Character or Icon</td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td>Alt+ (Left Arrow)</td>
      <td> </td>
      <td>Back</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td></td>
      <td> </td>
      <td>Back</td>
    </tr>
    <tr>
      <td>Alt+ (Right Arrow)</td>
      <td> </td>
      <td>Forward</td>
      <td> </td>
      <td> </td>
      <td> </td>
      <td></td>
      <td> </td>
      <td>Forward </td>
    </tr>
  </tbody>
</table>

<hr style="margin-top: 2em; margin-bottom: 2em"/>

Addendum: A big thanks goes out to Mikko Rantalainen <em>mikko.rantalainen at peda.net</em> for providing the following information regarding internationalization,
specifically Finnish/Swedish localizations:

-   Default Internet Explorer for Finnish localization has menu bar accelerators for T, M, N, S, K and O and address bar accelerator E.
-   In addition, shortcuts with ‘=’, ‘(‘, ‘)’, ‘\[‘, ‘\]’, ‘/’, ”, ‘;’ and ‘:’ require using shift or AltGr with Finnish/Swedish
    (and most other European) keyboard layouts so those cannot be used with just ALT.
    (For example, to type ‘\[‘ I have to press AltGr+8. So “ALT+\[” requires me to press Alt+AltGr+8 which seldom works as expected.
    If you accept this kind of shortcuts you might as well add “AltGr+µ” as it’s equally easy to type (Alt+AltGr+M) with my Finnish layout keyboard).
-   Non-numeric keys that can be used without any modifier key in Finnish/Swedish keyboard layout are:
    \+ ‘ – . , &lt; § and letters å ä ö \[written in UTF-8\]


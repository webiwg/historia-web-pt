---
layout: translation
date: 1978-04-01
title: RFC 748 - TELNET RANDOMLY-LOSE Option
description: RFC 748 - TELNET RANDOMLY-LOSE Option
copyright: null
license: null
license-custom: null
original: {
    title: "RFC 748 - TELNET RANDOMLY-LOSE Option",
    link: "https://tools.ietf.org/html/rfc748",
    dateOfTranslation: "2016-09-08"
}
authors: [{
    name: "M. Crispin",
    link: "https://en.wikipedia.org/wiki/Mark_Crispin"
}]
sponsors: null
translators: null
reviewers: null
isDraft: true
isReleaseCandidate: false
discussion: https://github.com/webiwg/historia-web-pt/issues/18
---

<pre>

NWG/RFC# 748                                          MRC 1-APR-78 44125
Telnet Randomly-Lose Option



Network Working Group                                         M. Crispin
Request for Comments 748                                           SU-AI
NIC 44125                                                   1 April 1978

                      Opção de PERDA-ALEATORIA para TELNET

1.  Nome e código do comando.

   RANDOMLY-LOSE        256

2.  Significado do comando.

   IAC WILL RANDOMLY-LOSE

      Quem envia esse comando (REQUESTS) pede/solicita permissão para randomly lose ou
      confirma que vai ocorrer randomly lose.

      Quem envia esse comando (REQUESTS) pede/solicita ou permissão ou
      confirma que vai ocorrer randomly lose.

      O emissor desse comando (REQUESTS) pede/solicita permissão
      ou confirma que vai ocorrer randomly lose.

   IAC WON'T RANDOMLY-LOSE

      O emissor desse comando se nega (REFUSES) a randomly lose.

   IAC DO RANDOMLY-LOSE

      The sender  of this command  REQUESTS that the receiver, or grants
      the receiver permission to, randomly lose.

      O emissor desse comando (REQUESTS) pede/solicita que o receptor, ou
      dá permissão ao receptor para, randomly lose.

      O emissor desse comando (REQUESTS) pede/solicita que o receptor ramdomly lose
      ou dá permissão ao receptor para randomly lose.


   IAC DON'T RANDOMLY-LOSE

      The command sender DEMANDS that the receiver not randomly lose.

      O emissor (DEMANDS) exige que o receptor não randomly lose.

3.  Default.

   WON'T RANDOMLY-LOSE

   DON'T RANDOMLY-LOSE

   i.e., random lossage will not happen.

   i,e., perca randômica não acontecerá.

4.  O motivo dessa opção.

   Vários servidores aparentam prover random lossage como parte do seus
   serviços ,por exemplo, quebras no sistema (crasches), perca de dados,
   mau funcionamento de programas, etc...
   Esses serviços são frequentemente não documentados e são em geral
   confusos para um usuário novo (noob),
   Several  hosts appear  to provide  random  lossage,  such  as  system
   crashes,  lost data,  incorrectly functioning programs, etc., as part
   of their services.   These services are often undocumented and are in
   general  quite confusing  to the novice  user.   A general  means  is
   needed to allow the user to disable these features.








                                 - 1 -

NWG/RFC# 748                                          MRC 1-APR-78 44125
Telnet Randomly-Lose Option

5.  Description of the option.

   The normal  mode does not allow random  lossage; therefore the system
   is not allowed  to crash,  mung user files, etc.  If the server wants
   to provide  random lossage, it must first ask for permission from the
   user by sending IAC WILL RANDOMLY-LOSE.

   If the user wants  to permit  the server  to randomly lose, it replys
   with  IAC  DO   RANDOMLY-LOSE.    Otherwise   it   sends   IAC   DONT
   RANDOMLY-LOSE, and the server is forbidden from randomly losing.

   Alternatively, the user could request the server to randomly lose, by
   sending  IAC DO RANDOMLY-LOSE,  and the server will either reply with
   IAC WILL RANDOMLY-LOSE,  meaning that it will then proceed to do some
   random  lossage  (garbaging  disk files is recommended for an initial
   implementation).   Or,  it could send IAC WONT RANDOMLY-LOSE, meaning
   that it insists upon being reliable.

   Since  this is implemented  as a TELNET  option,  it is expected that
   servers  which do not implement  this option  will not randomly lose;
   ie, they will provide 100% reliable uptime.
</pre>

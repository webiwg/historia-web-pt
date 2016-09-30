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

      O emissor desse comando (REQUESTS) pede/solicita permissão
      ou confirma que vai ocorrer randomly lose.

   IAC WON'T RANDOMLY-LOSE

      O emissor desse comando se nega (REFUSES) a randomly lose.

   IAC DO RANDOMLY-LOSE

      O emissor desse comando (REQUESTS) pede/solicita que o receptor, ou
      dá permissão ao receptor para, randomly lose.

     

   IAC DON'T RANDOMLY-LOSE

      O emissor (DEMANDS) exige que o receptor não faça randomly lose.

3.  Default.

   WON'T RANDOMLY-LOSE

   DON'T RANDOMLY-LOSE

   i,e., perca randômica não acontecerá.

4.  O motivo dessa opção.

   Vários servidores aparentam prover random lossage como parte do seus
   serviços ,por exemplo, quebras no sistema (crashes), perca de dados,
   mau funcionamento de programas, etc...
   Esses serviços são frequentemente não documentados e são em geral
   confusos para um usuário novo. Um meio geral é necessário para permitir
   o usuário desabilitar tais recursos.
  








                                 - 1 -

NWG/RFC# 748                                          MRC 1-APR-78 44125
Telnet Randomly-Lose Option

5.  Descrição da opção
   
   O modo normal não permiti perda randômica; por isso o sistema não é permitido
   crashar,
   The normal  mode does not allow random  lossage; therefore the system
   is not allowed  to crash,  arquivos de usuários **mung** , etc. Se o server 
   quer promover perda randômica, primeiro irá perguntar por permissão
   pelo usuário mandando IAC WILL RANDOMLY-LOSE.
   
   Se o usuário quer permitir que o server faça perda randômica, responde
   com IAC DO RANDOMLY-LOSE. Caso contrário envia  IAC   DONT RANDOMLY-LOSE,
   e server é proibido de ter perca randômica.
 
   Alternativamente, o usuário poderá pedir ao server perda randômica, ao
   enviar IAC DO RANDOMLY-LOSE, e o server irá ou responder com IAC WILL 
   RANDOMLY-LOSE, significando que irá proceder com alguma perda randômica
   (
   Alternatively, the user could request the server to randomly lose, by
   sending  IAC DO RANDOMLY-LOSE,  and the server will either reply with
   IAC WILL RANDOMLY-LOSE,  meaning that it will then proceed to do some
   random  lossage  (garbaging de arquivos de disco é recomendado para uma 
   implementação inicial). O, irá enviar IAC WONT RANDOMLY-LOSE, significando 
   que insiste até que seja confiável.

   Desde de que isso é implementando no TELNET como opção, é esperado que
   servers que não implementam tal opção não terão perda randômica; i.e,
   eles irão promover 100% de confiança em tempo operante.
  
</pre>

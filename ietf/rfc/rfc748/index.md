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
translators: [{
    name: "Roberta Mayer",
    link: "https://github.com/robsmayer"
}]
reviewers: [{
    name: "Vilmar Neto",
    link: "http://www.webiwg.org"
},{
    name: "Pedro Belasco",
    link: "http://pbelasco.org"
}]
isDraft: false
isReleaseCandidate: true
discussion: https://github.com/webiwg/historia-web-pt/issues/18
---

<pre>

NWG/RFC# 748                                          MRC 1-APR-78 44125
Telnet Randomly-Lose Option



Network Working Group                                         M. Crispin
Request for Comments 748                                           SU-AI
NIC 44125                                                   1 April 1978

                      TELNET RANDOMLY-LOSE Option

1.  Nome e código do comando.

   RANDOMLY-LOSE        256

2.  Significado do comando (O que faz).

   IAC WILL RANDOMLY-LOSE

      O emissor desse comando (REQUESTS) pede/solicita permissão
      (confirma) que vai ocorrer randomly lose.
   IAC WON'T RANDOMLY-LOSE

      O emissor desse comando se nega (REFUSES) a ter randomly lose.

   IAC DO RANDOMLY-LOSE

      O emissor desse comando (REQUESTS) pede/solicita que o receptor
      (dá permissão ao receptor) para  ter randomly lose. (Nota: não gostei dessa tradução)


   IAC DON'T RANDOMLY-LOSE

      O emissor (DEMANDS) exige que o receptor não faç randomly lose.

3.  Default.

   WON'T RANDOMLY-LOSE

   DON'T RANDOMLY-LOSE

   i,e., perda randômica não acontecerá.

4.  O motivo dessa opção.

   Obs: A expressão random lossage pode ser interpretada como perda randômica
   ou perda aleatória, mas nessa tradução manterei a expressão original.

   Vários servidores aparentam prover random lossage como parte do seus
   serviços ,por exemplo, quebras no sistema (crashes), perda de dados,
   mau funcionamento de programas, etc...
   Esses serviços são frequentemente não documentados e são em geral
   confusos para um usuário novo (noob). Logo, um meio simples é necessário
   para permitir que o usuário desative essas ocorrências.


                                 - 1 -

NWG/RFC# 748                                          MRC 1-APR-78 44125
Opção Randomly-Lose Telnet



5. Descrição da opção.

   O modo padrão não permite random lossage; portanto não é permitido que
   o sistema caia (crash), (mung*) arquivos do usuário, etc. Se o sevidor
   quiser enviar random lossage, em primeiro lugar, ele deve pedir permisão
   para o usuário mandando IAC WILL RANDOMLY-LOSE.

   Se o usuário quiser random lose do servidor, o servidor responderá
   IAC DO RANDOMLY-LOSE. Caso contrário, ele responderá IAC DONT RANDOMLY-LOSE
   e o servidor será proibido de randomly lose.

   Como uma outra alternativa, o usuário pode solicitar random lossage
   do servidor mandando IAC DO RANDOMLY-LOSE e o servidor responderá
   ou com IAC WILL RANDOMLY-LOSE, ou seja, ele irá prosseguir fazendo
   random lose (para uma implementação inicial é recomendado apagar arquivos
   do disco). Ou, ele responderá IAC WONT RANDOMLY-LOSE que significa
   que ele insiste em não fazer fazer randomly lose.

   Sendo que essa opção é implementada para TELNET, é esperado que em
   servidores que não tem essa opção implementada não ocorra random
   lossage; i.e, logo, eles funcionarão com atividade 100% confiável.

</pre>

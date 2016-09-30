---
layout: translation
date: 1990-04-01
title: A Standard for the Transmission of IP Datagrams on Avian Carriers
description: A Standard for the Transmission of IP Datagrams on Avian Carriers
copyright: null
license: null
license-custom: null
original: {
    title: "A Standard for the Transmission of IP Datagrams on Avian Carriers",
    link: "https://tools.ietf.org/html/rfc1149",
    dateOfTranslation: "2016-09-08"
}
authors: [{
    name: "D. Waitzman",
    link: "#"
}]
sponsors: null
translators: null
reviewers: null
isDraft: true
isReleaseCandidate: false
discussion: https://github.com/webiwg/historia-web-pt/issues/20
---

<pre>
Network Working Group                                        D. Waitzman
Request for Comments: 1149                                       BBN STC
                                                            1 April 1990

   Um Padrão para a Transmissão de Datagramas IP em Pombos Correios
   _A Standard for the Transmission of IP Datagrams on Avian Carriers_

Status deste Memo
   
   Este memo descreve um metódo experimental para encapsulamento de datagramas de IP
   em pombos correios . Esta especificação é primariamente útil em Redes de Área
   Metropolitana. Isto é um experimento, não um padrão recomendado. Distribuição
   deste memo é ilimitada.
 

Visão geral e racional

   Pombos correios podem provocar alto _delay_ , baixo _throughput_ e 
   serviço de baixa altitude. A topologia da conexão está limitada a
   um único caminho ponto-a-ponto para cada pombo, usado com padrão dos 
   mensageiros, mas muitos pombos podem ser usados sem interferência 
   significativa um com outro, fora do ínicio da primavera. Isto é devido
   ao espaço _ether_ 3D para os pombos, em contraste ao _ether_ 1D usado
   pela IEEE802.3. Os pombos tem um sistema de desvio intrínseco de colisão,
   que aumenta a disponibilidade. Ao contrário de altas tecnologias de rede,
   tais como Rádio Pacote, comunicação não é limitada a distância linha de visão.
   Serviço de orientação de conexão está disponível em algumas cidades, usualmente
   baseada em uma tecnologia _hub_ central.


Formato do _Frame_

   O datagrama IP é impresso, em um pedaço pequeno de papel, em hexadecimal,
   com cada octeto separado por _whitestuff_ e _blackstuff_. O rolo de papel
   está envolto sobre uma perna do pombo correio. Uma bandagem de fita adesiva
   é utilizada para proteger as bordas do datagrama. A largura da bandagem é 
   limitada ao tamanho da perna. O _MTU_ é variável, e paradoxalmente, geralmente
   aumenta com a idade do pombo. Um _MTU_ típico é 256 miligramas. Algumas plataformas
   de datagramas serão necessárias.

   Após o recebimento, a fita adesiva é removida e cópia do papel é oticalmente
   escaneada de forma eletronicamente transmitivel.
  

Discussão
   
   Múltiplos tipos de serviços podem ser providenciados com estrutura de poder
   priorizada. Uma propriedade adicional é detecção e erradicação de worm 
   embutida. Poruqe IP só garante a entrega de melhor esforço, perda de 
   um pombo pode ser tolerada. Com tempo os pombos se auto-regeneram.
   Multiple types of service can be provided with a prioritized pecking
   



Waitzman                                                        [Page 1]

RFC 1149             IP Datagrams on Avian Carriers         1 April 1990

   Enquanto o _broadcasting_ não é específico, tempestades podem causar
   perda de dados. Existe uma nova tentativa de entrega persistente, até
   que o pombo caía. Trilhas de audiotria são geradas automaticamentes, e 
   podem ser achadas em _logs_ e suportes para cabos.
   

Security Considerations

   Security is not generally a problem in normal operation, but special
   measures must be taken (such as data encryption) when avian carriers
   are used in a tactical environment.

Author's Address

   David Waitzman
   BBN Systems and Technologies Corporation
   BBN Labs Division
   10 Moulton Street
   Cambridge, MA 02238

   Phone: (617) 873-4323

   EMail: dwaitzman@BBN.COM





























Waitzman                                                        [Page 2]
</pre>
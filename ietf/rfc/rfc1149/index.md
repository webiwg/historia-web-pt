---
layout: translation
date: 1990-04-01
title: "RFC 1149 - Um Padrão para a Transmissão de Datagramas IP em Pombos Correios"
description: "Este memo descreve um metódo experimental para encapsulamento de
datagramas de IP em pombos correios . Esta especificação é  Metropolitana.
Isto é um experimento, não um padrão recomendado. Distribuição deste memo é
ilimitada."

copyright: null
license: null
license-custom: null
original: {
    title: "A Standard for the Transmission of IP Datagrams on Avian Carriers",
    link: "https://tools.ietf.org/html/rfc1149",
    dateOfTranslation: "2016-09-28"
}
authors: [{
    name: "D. Waitzman",
    link: "#"
}]
sponsors: null
translators: [{
    name: "vil aprato",
    link: "http://www.webiwg.org"
}]
reviewers: null
isDraft: true
isReleaseCandidate: false
discussion: https://github.com/webiwg/historia-web-pt/issues/20
---

<!-- Geração automática de índice, inicio -->
<nav  markdown="1">

## Índice de tópicos
{:.no_toc}

1. Índice de Tópicos. Esta linha será substituída
{:toc}

</nav>
<!-- Geração automática de índice, fim -->

## Tradução

<pre>
Network Working Group                                        D. Waitzman
Pedidos para comentários: 1149                                       BBN STC
                                                            1º Abril 1990

   Um Padrão para a Transmissão de Datagramas IP em Pombos Correios
   <em lang="en">A Standard for the Transmission of IP Datagrams on Avian Carriers</em>

Status deste Memo

   Este memo descreve um metódo experimental para encapsulamento de datagramas de IP
   em pombos correios . Esta especificação é primariamente útil em Redes de Área
   Metropolitana. Isto é um experimento, não um padrão recomendado. Distribuição
   deste memo é ilimitada.


Visão geral e racional

   Pombos correios podem provocar alto <em lang="en">delay</em> , baixo <em lang="en">throughput</em> e
   serviço de baixa altitude. A topologia da conexão está limitada a
   um único caminho ponto-a-ponto para cada pombo, usado com padrão dos
   mensageiros, mas muitos pombos podem ser usados sem interferência
   significativa um com outro, fora do ínicio da primavera. Isto é devido
   ao espaço <em lang="en">ether</em> 3D para os pombos, em contraste ao <em lang="en">ether</em> 1D usado
   pela IEEE802.3. Os pombos tem um sistema de desvio intrínseco de colisão,
   que aumenta a disponibilidade. Ao contrário de altas tecnologias de rede,
   tais como Rádio Pacote, comunicação não é limitada a distância linha de visão.
   Serviço de orientação de conexão está disponível em algumas cidades, usualmente
   baseada em uma tecnologia <em lang="en">hub</em> central.


Formato do <em lang="en">Frame</em>

   O datagrama IP é impresso, em um pedaço pequeno de papel, em hexadecimal,
   com cada octeto separado por <em lang="en">whitestuff</em> e <em lang="en">blackstuff</em>. O rolo de papel
   está envolto sobre uma perna do pombo correio. Uma bandagem de fita adesiva
   é utilizada para proteger as bordas do datagrama. A largura da bandagem é
   limitada ao tamanho da perna. O <em lang="en">MTU</em> é variável, e paradoxalmente, geralmente
   aumenta com a idade do pombo. Um <em lang="en">MTU</em> típico é 256 miligramas. Algumas plataformas
   de datagramas serão necessárias.

   Após o recebimento, a fita adesiva é removida e cópia do papel é oticalmente
   escaneada de forma eletronicamente transmitivel.


Discussão

   Múltiplos tipos de serviços podem ser providenciados com estrutura de poder
   priorizada. Uma propriedade adicional é detecção e erradicação de worm
   embutida. Poruqe IP só garante a entrega de melhor esforço, perda de
   um pombo pode ser tolerada. Com tempo os pombos se auto-regeneram.





Waitzman                                                        [Page 1]

RFC 1149             IP Datagrams on Avian Carriers         1º Abril 1990

   Enquanto o <em lang="en">broadcasting</em> não é específico, tempestades podem causar
   perda de dados. Existe uma nova tentativa de entrega persistente, até
   que o pombo caía. Trilhas de audiotria são geradas automaticamentes, e
   podem ser achadas em <em lang="en">logs</em> e suportes para cabos.


Considerações de Segurança

   Segurança é não geralmente um problema numa operação normal, mas medidas
   especial devem ser tomadas (como criptografia de dados) quando pombos
   correios são usados em um ambiente tático.


Endereço do autor:

   David Waitzman
   BBN Systems and Technologies Corporation
   BBN Labs Division
   10 Moulton Street
   Cambridge, MA 02238

   Telefone: (617) 873-4323

   E-mail: dwaitzman@BBN.COM





























Waitzman                                                        [Page 2]
</pre>

## Original

<pre lang="en">
Network Working Group                                        D. Waitzman
Request for Comments: 1149                                       BBN STC
                                                            1 April 1990


   A Standard for the Transmission of IP Datagrams on Avian Carriers

Status of this Memo

   This memo describes an experimental method for the encapsulation of
   IP datagrams in avian carriers.  This specification is primarily
   useful in Metropolitan Area Networks.  This is an experimental, not
   recommended standard.  Distribution of this memo is unlimited.

Overview and Rational

   Avian carriers can provide high delay, low throughput, and low
   altitude service.  The connection topology is limited to a single
   point-to-point path for each carrier, used with standard carriers,
   but many carriers can be used without significant interference with
   each other, outside of early spring.  This is because of the 3D ether
   space available to the carriers, in contrast to the 1D ether used by
   IEEE802.3.  The carriers have an intrinsic collision avoidance
   system, which increases availability.  Unlike some network
   technologies, such as packet radio, communication is not limited to
   line-of-sight distance.  Connection oriented service is available in
   some cities, usually based upon a central hub topology.

Frame Format

   The IP datagram is printed, on a small scroll of paper, in
   hexadecimal, with each octet separated by whitestuff and blackstuff.
   The scroll of paper is wrapped around one leg of the avian carrier.
   A band of duct tape is used to secure the datagram's edges.  The
   bandwidth is limited to the leg length.  The MTU is variable, and
   paradoxically, generally increases with increased carrier age.  A
   typical MTU is 256 milligrams.  Some datagram padding may be needed.

   Upon receipt, the duct tape is removed and the paper copy of the
   datagram is optically scanned into a electronically transmittable
   form.

Discussion

   Multiple types of service can be provided with a prioritized pecking
   order.  An additional property is built-in worm detection and
   eradication.  Because IP only guarantees best effort delivery, loss
   of a carrier can be tolerated.  With time, the carriers are self-



Waitzman                                                        [Page 1]

RFC 1149             IP Datagrams on Avian Carriers         1 April 1990


   regenerating.  While broadcasting is not specified, storms can cause
   data loss.  There is persistent delivery retry, until the carrier
   drops.  Audit trails are automatically generated, and can often be
   found on logs and cable trays.

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

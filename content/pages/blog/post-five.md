---
type: PostLayout
title: Como passar em cases técnicos?
colors: colors-a
date: '2024-05-02'
author: content/data/team/doris-soto.json
excerpt: More context that may or may not be helpful
featuredImage:
  type: ImageBlock
  url: /images/featured-Image5.jpg
  altText: Post thumbnail image
bottomSections:
  - elementId: ''
    type: RecentPostsSection
    colors: colors-f
    variant: variant-d
    subtitle: Recent posts
    showDate: true
    showAuthor: false
    showExcerpt: true
    recentCount: 2
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
          - ml-0
          - mr-0
        padding:
          - pt-12
          - pb-56
          - pr-4
          - pl-4
        justifyContent: center
      title:
        textAlign: left
      subtitle:
        textAlign: left
      actions:
        justifyContent: center
    showFeaturedImage: true
    showReadMoreLink: true
  - type: ContactSection
    backgroundSize: full
    title: Stay up-to-date with my words ✍️
    colors: colors-f
    form:
      type: FormBlock
      elementId: sign-up-form
      fields:
        - name: firstName
          label: First Name
          hideLabel: true
          placeholder: First Name
          isRequired: true
          width: 1/2
          type: TextFormControl
        - name: lastName
          label: Last Name
          hideLabel: true
          placeholder: Last Name
          isRequired: false
          width: 1/2
          type: TextFormControl
        - name: email
          label: Email
          hideLabel: true
          placeholder: Email
          isRequired: true
          width: full
          type: EmailFormControl
        - name: updatesConsent
          label: Sign me up to recieve my words
          isRequired: false
          width: full
          type: CheckboxFormControl
      submitLabel: "Submit \U0001F680"
      styles:
        submitLabel:
          textAlign: center
    styles:
      self:
        height: auto
        width: narrow
        margin:
          - mt-0
          - mb-0
          - ml-4
          - mr-4
        padding:
          - pt-24
          - pb-24
          - pr-4
          - pl-4
        alignItems: center
        justifyContent: center
        flexDirection: row
      title:
        textAlign: left
      text:
        textAlign: left
---
Uma das principais fases de qualquer processo seletivo são as temidas **entrevistas técnicas**. Aqui, serão avaliados cenários referentes as suas '*hard-skills*'. Nesse post, darei alguns exemplo de cases reais pedidos pelo mercado, e comentarei os principais pontos que foram avaliados em cada um deles. 

Importante entender que o conteúdo técnico dos desafios varia (***e MUITO!***) dependendo da empresa e da vaga, mas uma característica é comum em todos: Os desafios técnicos procuram saber se o candidato tem os requisitos suficientes pedidos pela posição no qual irá exercer no trabalho.

À princípio, vou mostrar como exemplo três cases para as seguintes posições: Segurança (Geral), Blue Team Engineer e Application Security. Para vagas de Pentest, normalmente é enviado ao candidato uma aplicação com vulnerabilidades para serem exploradas e documentadas.

Vamos dar uma olhada em alguns exemplos:

Case 1 - Vaga Analista Segurança da Informação Júnior/Pleno -  Empresa de Tecnologia

****

*



*



*



*



*



****

*



*



*



*



![](https://www.securitytalents.com.br/~gitbook/image?url=https%3A%2F%2F472801866-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FKpzbmVVVqtAyWCAnmCBJ%252Fuploads%252FyJOOOFkaw4A2mHb8Ze6Y%252FScreenshot%25202024-09-24%2520at%252021.29.28.png%3Falt%3Dmedia%26token%3D25debb3e-54f6-45f9-967b-e69ffaa18e72\&width=768\&dpr=4\&quality=100\&sign=42f478c1\&sv=1)Topologia do case 1

> **Comentário Case 1:** 
>
> Nesse cenário, foi avaliada a competência do candidato em conhecimentos gerais sobre Segurança da Informação, o que incluiu: 
>
> *
>
>     Análise de boas práticas de Segurança da Informação: É esperado que o candidato(a) avalie e pontue erros nessa topologia, como serviços em execução de forma incorreta (3389, 445), falta de segmentação de rede, servidores Linux sem autenticação correta, etc.
>
> *
>
>     Conhecimento de técnicas de ataque: É esperado que o candidato(a) conheça e deduza de forma coesa técnicas prováveis de terem sido exploradas nesse cenário hipotético, como exploração de vulnerabilidades conhecidas, CVEs, credenciais vazadas, cenários de movimentação lateral, etc.
>
> *
>
>     Conhecimento de frameworks de Segurança da Informação: É esperado que o candidato(a) conheça e sugira cenários de correção, não apenas da parte técnica, mas também da parte de **governança**, sugerindo a implementação de frameworks como uma 'Política de Segurança da Informação', que deve ter diretrizes que mitiguem a probabilidade do acontecimento dos pontos  identificados anteriormente.

Case 2 - Vaga Blue Team Engineer - Pleno - Fintech

****

1.

    ``

2.

    ``

3.

    ``

> **Comentário Case 2:** 
>
> Nesse cenário, havia uma máquina virtual Linux com diversas vulnerabilidades e políticas feitas **incorretamente** de forma proposital, para que seja avaliado o conhecimento do candidato sobre **hardening,** isto é, realizar o entendimento do estado atual daquela máquina Linux (serviços em execução, política de senhas, rede, etc.), para depois serem sugeridas melhorias para esse ambiente.
>
> É esperado aqui que o candidato redigisse uma boa documentação técnica explicando o que foi encontrado de errado nessa máquina, e que sugerisse medidas de **hardening** com base em frameworks de mercado, como por exemplo, o CIS (<https://www.cisecurity.org/cis-benchmarks-overview>), o que é perfeitamente condizente com o título da vaga 'Blue Team Engineer'.

Case 3 - Vaga AppSec Engineer - Pleno/Sênior - Fintech





****

1.

    ****

> **Comentário Case 3:** 
>
> Nesse cenário, foi avaliado a competência do candidato em desenvolver (codar) e documentar ferramentas básicas que ele pode utilizar no dia-a-dia. 
>
> Em uma vaga de Application Security, é **fundamental** que o candidato tenha skills de programação, principalmente **scripting**, para que possa desenvolver as próprias ferramentas conforme a necessidade do trabalho.
>
> Nesse case, é pedido que se realize uma automação para uma ferramenta de proxy conhecida de mercado (Burp Suite), e que nessa automação seja contemplado um item importante de negócios para a empresa, no caso, a busca por dados sensíveis (**CPFs**) em suas aplicações web.

### Independente do case, é fundamental:



<!---->

1.  Cumprir o prazo que o recrutador te dará para realizar o desafio (óbvio..),

2.  Comunicar quaisquer problemas referentes à infraestrutura do desafio (o famoso: o site caiu...),

3.  Documentar **BEM** os passos realizados no desafio, pois você provavelmente enviará e/ou apresentará esse documento para alguém no processo seletivo

4.  Tirar todas as dúvidas referentes ao case, afinal, você não vai querer entregar **X** quando na verdade foi pedido **Y.**

*Espero que essas dicas sejam valiosas.
Good luck.*

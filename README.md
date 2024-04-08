# AI-900: Análise de Sentimentos com Language Studio no Azure AI

<div align="center">

### **Descrição do Projeto :**

</div>

Este projeto é um dos laboratórios do Bootcamp [Microsoft Azure AI Fundamentals](https://web.dio.me/track/microsoft-azure-ai-fundamentals), promovido através da parceria entre a **Microsoft** e a **DIO** .

Este repositório tem como finalidade armazenar o projeto desenvolvido no âmbito do módulo "Natural Language Processing" do Bootcamp da [DIO](https://www.dio.me/users/giovananascimentoferreira1) , sob orientação da professora [Valéria Baptista](https://www.linkedin.com/in/valeriabaptista/) .

Os alunos deste bootcamp tem, como principal objetivo, se prepararem para o exame de certificação Microsoft AI-900, dominando conceitos como visão computacional, classificação de inteligência de imagem e inteligência de documentos com IA, enquanto se familiarizam com as tecnologias da **Microsoft Azure** .

O projeto é requisito essencial para a aprovação no módulo “Processamento de Linguagem Natural”, consolidando a aprendizagem prática dos participantes e preparando-os para os desafios subsequentes.

O desenvolvimento deste projeto visa identificar serviços de IA do Azure que incluam processamento de linguagem natural, especificamente serviços de fala para texto e análise de sentimentos. Para um melhor entendimento, dividi todo o processo em etapas, desde a criação dos recursos até o resultado final da conversão e análise de sentimento.

Este desafio é o de número 4 do bootcamp e consiste na execução prática de 2 exercícios, relacionados aos seguintes temas:

- [LAB 1: Azure Speech Studio](http://aka.ms/ai900-speech): experimentar os recursos do Azure AI Speech usando o Azure AI Speech Studio
- [LAB 2: Azure Language Studio](http://aka.ms/ai900-text-analysis): explorar os recursos da Linguagem de IA do Azure


<div align="center">

### **Tags do Projeto :**

![Static Badge](https://img.shields.io/badge/Inteligência_Artificial_(IA)-blue)
![Static Badge](https://img.shields.io/badge/IA_Generativa-blue)
![Static Badge](https://img.shields.io/badge/IA_Speech_(Legendagem)-blue)
![Static Badge](https://img.shields.io/badge/IA_Processamento_de_Linguagem_Natural-blue)
![Static Badge](https://img.shields.io/badge/IA_Análise_de_Sentimentos-blue)

![Static Badge](https://img.shields.io/badge/Microsoft_Azure-orange)
![Static Badge](https://img.shields.io/badge/Azure_AI_Services-orange)
![Static Badge](https://img.shields.io/badge/Azure_Language_Services-orange)
![Static Badge](https://img.shields.io/badge/Azure_Speech_Studio-orange)
![Static Badge](https://img.shields.io/badge/Azure_Language_Studio-orange)

</div>

<div align="center">

### **Acessos Necessários :**

</div>

Para realizar estes laboratórios, eu precisei criar uma **Subscrição** do **Microsoft Azure** . 

No meu caso criei a [**Conta de Estudante da Microsoft**](https://azure.microsoft.com/pt-br/free/students) .

A Microsoft permite criar uma subscrição de teste, na qual vários serviços podem ser experimentados gratuitamente por 12 meses, além de receber $100 para serem utilizados durante o ano.

<div align="center">

### **LAB1 - Estúdio de Fala :**

#### **Introdução :**

</div>

A transcrição da fala em texto e a conversão de texto em fala audível por meio da IA são processos-chave na comunicação entre humanos e máquinas. 

Podemos utilizar o **AI Speech** para criar um aplicativo que possa transcrever anotações de reuniões ou gerar texto a partir da gravação de entrevistas.

Neste laboratório, abordarei, especificamente, os recursos do **Azure AI Speech** dentro do **Azure AI Speech Studio** para realizar a criação de legenda automática de um aúdio.

Para ocorrer a transcrição da fala em texto o **Azure AI Speech Studio** usa algoritmos de reconhecimento de voz para converter palavras faladas em texto escrito, enquanto a conversão de texto em fala utiliza sistemas de síntese de voz para transformar texto em uma saída audível.

Ambos os processos têm uma variedade de aplicações, desde assistentes virtuais até acessibilidade para pessoas com deficiência. Apesar de desafios como precisão em ambientes ruidosos e naturalidade na fala sintetizada, o desenvolvimento contínuo impulsiona uma interação mais intuitiva e inclusiva entre humanos e sistemas baseados em IA.

Sabendo disso, podemos através da função de **Conversão de voz em texto em tempo real**, o qual é um serviço Speech, que transcreve e exibe o texto em tempo real. Como também, caso você tenha áudio em seu computador, poderá ouvir a gravação enquanto o texto é transcrito.

#### **Etapa 1: Criando um recurso para conversão de fala/voz em texto**

Vamos começar acessando o seguinte **portal da Microsoft :** https://speech.microsoft.com/portal .

No portal [**Speech Studio**](https://speech.microsoft.com/portal) , criaremos um novo recurso.

Siga de acordo com os Passos a seguir:

<div align="center">
 
<img src="Assets/Passo-a-Passo para Criar Recurso no Speech Studio.gif"/>

</div>

Agora tem ***duas maneiras*** de definir o recurso como Padrão :

A **Primeira Maneira** é indo nas Configurações, Marcando o Recurso desejado e Apertando no Botão Azul como demontrado na foto a seguir (no meu caso como já defini o recurso na 2° Maneira o botão aparece cinza):

<div align="center">

<img src="Assets/1° Maneira - Definir Recurso como Padrão.png">

</div>

A **Segunda Maneira** é (caso aparecesse a tela) Apertando no Botão Azul no caso superior direito como demonstrado na imagem a seguir.

<div align="center">

<img src="Assets/2° Maneira - Definir Recurso como Padrão.png">

</div>


#### **Etapa 2: Explorando a conversão de Voz em Texto em Tempo Real no Speech Studio**

Na categoria Fala para texto, selecionaremos Fala para texto em tempo real.

Como demonnstrado no Passo-a-Passo a seguir:

<div align="center">

<img src="Assets/Passo-a-Passo - Converter Aúdio em Texto.gif">

</div>

<u>**Observação:**</u> Quando mudei o Vídeo (MP4) para GIF (GIF) ele ficou sem som.


**Aúdio Utilizado no Vídeo:** [Aúdio - Teste.mp3](https://github.com/Giovana006/Lab04---Processamento-de-Linguagem-Natural/blob/main/Assets/A%C3%BAdio%20-%20TESTE.mp3)

**Arquivo JSON :** [Aúdio_em_Testo.json](https://github.com/Giovana006/Lab04---Processamento-de-Linguagem-Natural/blob/main/Output/A%C3%BAdio_em_Texto.json)


#### **Etapa 4: Próximas Etapas**

Podemos usar o serviço de fala em texto em tempo real para integrá-lo com diferentes linguagens de programação para criar aplicativos personalizados que utilizem esse recurso.

<div align="center">

#### **Conclusão :**

</div>

Neste estudo, explorei o serviço **Azure Speech Studio** , com foco especial na sua capacidade de legendar através da conversão de fala em texto. Esta funcionalidade é uma ferramenta poderosa que pode ser aplicada em diversas situações, desde a transcrição de reuniões e conferências até a criação de legendas para vídeos.

No entanto, é importante lembrar que o **Azure Speech Studio** é muito mais do que apenas um serviço de transcrição. Ele oferece uma gama de outras funcionalidades que não foram abordadas em detalhe neste estudo, mas que são igualmente valiosas. Estas incluem a conversão de texto em fala, a tradução de fala e a personalização do modelo de fala, entre outras.

A versatilidade do **Azure Speech Studio** torna-o uma ferramenta indispensável para qualquer pessoa ou organização que procure melhorar a acessibilidade, a eficiência e a comunicação. Encorajos os leitores a explorarem estas outras funcionalidades para descobrir como elas podem ser aplicadas para atender às suas necessidades específicas.

Em resumo, o **Azure Speech Studio** é uma ferramenta robusta e multifuncional que tem o potencial de transformar a maneira como interagimos com a tecnologia e uns com os outros. Através da exploração contínua e da experimentação com suas diversas funcionalidades, podemos continuar a inovar e a melhorar nossas práticas de comunicação.

<div align="center">

### **LAB2 - Análise de Sentimentos :**

#### **Introdução :**

</div>

O Processamento de Linguagem Natural (PNL) é um ramo da IA que lida com a linguagem escrita e falada. Você pode usar a PNL para criar soluções que extraem significado semântico do texto e/ou da fala ou que formulem respostas significativas em linguagem natural.

O PNL pode ser utilizado, por exemplo, para realizar a análise de avaliações enviadas pelos clientes de um determinado serviço prestado, onde é possível identificar frases-chave, determinar quais avaliações são positivas e quais são negativas ou analisar o texto de revisão em busca de menções a entidades conhecidas, como locais ou pessoas.

O Serviço de Linguagem de IA do Azure inclui análise de texto e recursos de PNL. Estes incluem a identificação de frases-chave no texto e a classificação do texto com base no sentimento.

Neste laboratório, eu explorei os recursos da Linguagem de IA do Azure analisando alguns exemplos de avaliações de hotéis, utilizando Azure Language Studio para entender se as avaliações são majoritariamente positivas ou negativas.

#### **Etapa 1: Criando um recurso para análise de sentimento**

Primeiro, vamos acessar o portal do [Microsoft Azure](https://portal.azure.com/#home) .

Agora vamos criar um recurso e configurá-lo para depois utilizá-lo no **Language Studio** .

Siga de acordo com os Passos a seguir:

<div align="center">

<img src="Assets/Passo-a-Passo para Criar Recurso no Azure.gif">

</div>

#### **Etapa 2: Selecione um Recurso do Azure**

Após completar esta etapa de criação, vamos para o portal [Language Studio](https://language.cognitive.azure.com/home) .

Para acessar o Language Studio precisamos vinculá-lo a um recurso do Azure.

Siga de acordo com os Passos a seguir:

<div align="center">

<img src="Assets/Language Studio - Vincular Recurso do Azure.gif">

</div>

#### **Etapa 3: Analisar Sentimento e Extrair Opiniões**

Depois de víncular o recurso do Azure no **Language Studio**, vamos realizar a análise de sentimentos e opiniões.

Para realizar a análise de sentimento no **Language Studio** , podemos selecionar **"Analyze Sentiment and Opinions"** .

Depois é só selecionar a língua do texto digitar o texto desejado ou inserir o arquivo, marcar o quadradinho embaixo e apertar no botão RUN e Voilà pronto, temos a análise de sentimentos e opiniões!

Siga de acordo com os Passos do vídeo a seguir:

<div align="center">

<img src="Assets/Language Studio - Análise de Sentimentos e Opiniões.gif">

</div>

**Arquivo de Texto utilizado no Vídeo:** []()

**Arquivo JSON :** []()

#### **Etapa 4: examinar os resultados**

<div align="center">

**Análise de Sentimento Geral :**

<img src="Análise Sent. e Opi. - Análise de Sentimento Geral.png">

</div>

Analisando os resultados percebemos que a análise de sentimento é classificada em três variáveis: positiva, neutra e negativa. 

- **Positivo** denota sentimentos positivos como “feliz”, “ótimo”, “adorável”, entre outros. 

- **Neutro** refere-se a declarações neutras e objetivas que não expressam uma opinião emocional forte. 

- **Negativo** denota a presença de palavras com sentimentos negativos, como “triste”, “ruim”, “frustrante”, entre outros.

Em nosso texto, percebemos a satisfação do cliente ao curso do DIO (no caso gratuito), e isso levará nossa análise de sentimento a um percentual maior em Positivo.

<div align="center">

**Análise por Frases:**

**Frase 1 :**

<img src="Análise Sent. e Opi. - Frase 1.png">

**Frase 2 :**

<img src="Análise Sent. e Opi. - Frase 2.png">

**Texto Original :**

<img src="Análise Sent. e Opi. - Texto Original (TAG&apos;S).png">

</div>

#### **Etapa 5: Próximas Etapas**

Podemos utilizar o serviço "Analisar sentimentos e extrair opiniões" para integrá-lo com diferentes linguagens de programação para criar aplicações personalizadas que utilizem este recurso.

<div align="center">

#### **Conclusão :**

</div>

Neste estudo, explorei o poder do Azure Language Studio, com foco especial na análise de sentimentos e na mineração de opiniões. Essas ferramentas oferecem uma visão profunda dos dados textuais, permitindo que as empresas entendam melhor seus clientes e tomem decisões informadas.

No entanto, é importante lembrar que o Azure Language Studio oferece muito mais do que apenas essas funções. Existem outras capacidades poderosas, como a extração de frases-chave, a detecção de idioma e a identificação de entidades nomeadas, que não foram abordadas em detalhes neste artigo.

O Azure Language Studio é uma ferramenta versátil e robusta que pode ser adaptada a uma variedade de cenários de uso. Seja você um cientista de dados procurando entender grandes volumes de texto ou uma empresa procurando obter insights de dados de clientes, o Azure Language Studio tem algo a oferecer.

Com suas diversas funcionalidades, o Azure Language Studio ele abre um mundo de possibilidades para análise de dados e inteligência de negócios.

<div align="center">

### Limpando o ambiente

</div>

> [!WARNING]
> Após a conclusão do projeto, se não for reaproveitar os recursos utilizados, é aconselhável excluí-los, bem como os grupos de recursos, para que não haja cobranças indevidas na sua Azure Subscription
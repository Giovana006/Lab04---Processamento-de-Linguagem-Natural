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

<img src="Assets/Passo-a-Passo - Converter Aúdio em Texto.gif">

<u>**Observação:**</u> Quando mudei o Vídeo (MP4) para GIF (GIF) ele ficou sem som.


**Aúdio Utilizado no Vídeo:** [Aúdio - Teste.mp3](https://github.com/Giovana006/Lab04---Processamento-de-Linguagem-Natural/blob/main/Assets/A%C3%BAdio%20-%20TESTE.mp3)


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

### **LAB2 - Análise de sentimentos :**

</div>

#### **Etapa 1: Criando um recurso para análise de sentimento**

Primeiro, vamos acessar o portal do [Microsoft Azure](https://portal.azure.com/#home) .

Agora vamos criar um recurso e configurá-lo para depois utilizá-lo no **Language Studio** .

Siga de acordo com os Passos a seguir:

<img src="Assets/Passo-a-Passo para Criar Recurso no Azure.gif">

#### **Etapa 2: Selecione um Recurso do Azure**

Após completar esta etapa de criação, vamos para o portal [Language Cognitive](https://language.cognitive.azure.com/home) .

Para acessar o Language Studio precisamos vinculá-lo a um recurso do Azure.

Siga de acordo com os Passos a seguir:

<img src="Assets/Language Studio - Vincular Recurso do Azure.gif">


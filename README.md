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

### **LAB1 - Estúdio de Fala :**

- **Introdução :**

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

<img src="Assets/Passo-a-Passo - Converter Aúdio em Texto.gif">

<u>**Observação:**</u> Quando mudei o Vídeo (MP4) para GIF (GIF) ele ficou sem som.

<div align="center">

**Aúdio Utilizado no Vídeo:** 

[Aúdio - Teste.mp3](https://github.com/Giovana006/Lab04---Processamento-de-Linguagem-Natural/blob/main/Assets/A%C3%BAdio%20-%20TESTE.mp3)

</div>


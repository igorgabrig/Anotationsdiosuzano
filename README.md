# Anotationsdiosuzano

### O que é IA generativa?

- **IA:** Imita o comportamento humano usando o aprendizado de máquina para interagir com o ambiente e executar tarefas sem instruções explícitas sobre o que gerar.



### Modelos de Linguagem de Grande Porte - LLMs

- Os aplicativos de **IA gerativa** são alimentados por **LLMs**, que são um tipo especializado de modelo de machine learning que você pode usar para executar tarefas **PLN (Processamento de linguagem natural)**

- **Ex:**
	- Determinar sentimento ou classificar de outra forma o texto em idioma natural
	- Resumir um texto
	- Comparar várias fontes de texto quanto à similaridade semântica
	- Geração de nova linguagem natural.



### LLM - Transformer

- A arquitetura do modelo **transformer** consiste em dois componentes principais, ou blocos.
	- **Ex:** Ao inscrever uma palavra, é sugerido palavras seguintes que são prováveis de você digitar.


- Dois blocos:
	- **Codificador:** Cria representações semânticas do vocabulário de treinamento
	- **Decodificador:** Gera novas sequências de linguagem


- O texto é **tokenizado** para que cada palavra ou frase seja representada por um token numérico exclusivo
- **Inserções** (valores de vetor com várias dimensões) são atribuídas aos tokens
- As camadas de **atenção** examinam cada token por vez e determinam valores incorporados que refletem os relacionamentos semânticos entre os tokens
- No **decodificador** essas relações são usadas para prever a sequência mais provável de tokens
![[Pasted image 20250517141041.png]]


### Tokenização

- **Primeira etapa:** Tokenização
- Essa é a etapa onde vai ser particionado/decomposto

- A primeira etapa no treinamento de um modelo transformer é decompor o texto de treinamento em **tokens**

### Inserções

- **Etapa dois:** Inserções
- As relações entre tokens são capturadas como vetores, conhecidos como inserções


### Atenção

- **Terceiro passo:** Atenção
- Capture a força das relações entre tokens usando a técnica de atenção
- Exemplo:
	- Meta: Prever o token após "**cachorro**"
	- Represente "**Ouvi um cachorro**" como vetores
	- Atribua mais peso a "**ouvi**" e "**cachorro**"
- Vários tokens possíveis podem vir depois de cachorro
- O token mais provável é adicionado à sequência, nesse caso, "**latir**"

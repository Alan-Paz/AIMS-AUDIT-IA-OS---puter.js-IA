\documentclass[12pt,a4paper]{report}
\usepackage[utf8]{inputenc}
\usepackage[brazil]{babel}
\usepackage{geometry}
\usepackage{amsmath,amssymb,amsfonts,amsthm}
\usepackage{mathptmx} % Fonte Times New Roman (Padrão ABNT/TCC)
\usepackage{graphicx}
\usepackage{hyperref}
\usepackage{titlesec}
\usepackage{fancyhdr}
\usepackage{setspace}
\usepackage{float}
\usepackage{indentfirst} % Garante o recuo no primeiro parágrafo
\usepackage{qrcode}      % Pacote para geração do QR Code

\geometry{top=3cm,bottom=2cm,left=3cm,right=2cm}
\onehalfspacing

% Definição de Ambientes Teoremas, Axiomas e Definições
\newtheorem{axiom}{Axioma}[chapter]
\newtheorem{theorem}{Teorema}[chapter]
\newtheorem{definition}{Definição}[chapter]

\begin{document}

% ==========================================
% CAPA
% ==========================================
\begin{titlepage}
    \centering
    {\large \textbf{UNIVERSIDADE VIRTUAL DO ESTADO DE SÃO PAULO -- UNIVESP}}\\[1.0cm]
    {\large \textbf{CURSO DE ENGENHARIA DE COMPUTAÇÃO}}\\[2.0cm]
    {\large
    ALAN APARECIDO BENTO SILVA PEREIRA DA PAZ -- RA: 23223266\\
    GEOVANE DE SOUSA SILVA -- RA: 23227958\\
    JOSÉ MAURICIO DA SILVA LIMA -- RA: 2208518\\
    MARCOS ALEXANDRE DO NASCIMENTO REIS -- RA: 2006018\\
    ROGÉRIO DOS SANTOS -- RA: 1819149
    }\\[1.5cm]
    
    {\Large \textbf{AIMS AUDIT : APLICAÇÕES DA ISO/IEC 42001 EM ECOSSISTEMAS CRÍTICOS COM USO DE IA}}\\[2.0cm]
    
    {\large \textbf{ITAPEVI -- SP}}\\
    {\large \textbf{DEZEMBRO / 2026}}
\end{titlepage}

% ==========================================
% FOLHA DE ROSTO
% ==========================================
\begin{titlepage}
    \centering
    {\large
    ALAN APARECIDO BENTO SILVA PEREIRA DA PAZ -- RA: 23223266\\
    GEOVANE DE SOUSA SILVA -- RA: 23227958\\
    JOSÉ MAURICIO DA SILVA LIMA -- RA: 2208518\\
    MARCOS ALEXANDRE DO NASCIMENTO REIS -- RA: 2006018\\
    ROGÉRIO DOS SANTOS -- RA: 1819149
    }\\[1.5cm]
    
    {\Large \textbf{AIMS AUDIT : APLICAÇÕES DA ISO/IEC 42001 EM ECOSSISTEMAS CRÍTICOS COM USO DE IA}}\\[1.0cm]
    
    \hspace{4.5cm}
    \begin{minipage}{10cm}
        Trabalho de Conclusão de Curso -- Engenharia de Computação apresentado à Universidade Virtual do Estado de São Paulo (UNIVESP) como requisito parcial para a obtenção do título de Bacharel em Engenharia de Computação.\\[0.3cm]
        Orientador: Prof. Esp. Adelson Carlos Madruga.
    \end{minipage}\\[1.0cm]

    % ==========================================
    % QR CODE DO VÍDEO INSTITUCIONAL
    % ==========================================
    \begin{center}
        \qrcode[height=2.2cm]{https://www.youtube.com/watch?v=tkIKMHYUgBU}\\[0.1cm]
        {\small \textbf{Vídeo Institucional do Trabalho TCC 2026 (AIMS AUDIT)}\\
        Disponível em: \url{https://www.youtube.com/watch?v=tkIKMHYUgBU}}
    \end{center}\vfill
    
    {\large \textbf{ITAPEVI -- SP}}\\
    {\large \textbf{DEZEMBRO / 2026}}
\end{titlepage}

% ==========================================
% FOLHA DE APROVAÇÃO
% ==========================================
\begin{titlepage}
    \centering
    {\large \textbf{AIMS AUDIT : APLICAÇÕES DA ISO/IEC 42001 EM ECOSSISTEMAS CRÍTICOS COM USO DE IA}}\\[0.4cm]
    {\large \textbf{AUTORES:}}\\
    {\small
   ALAN APARECIDO BENTO SILVA PEREIRA DA PAZ -- RA: 23223266\\
    GEOVANE DE SOUSA SILVA -- RA: 23227958\\
    JOSÉ MAURICIO DA SILVA LIMA -- RA: 2208518\\
    MARCOS ALEXANDRE DO NASCIMENTO REIS -- RA: 2006018\\
    ROGÉRIO DOS SANTOS -- RA: 1819149
    }\\[0.8cm]
    
    \begin{flushleft}
    Aprovada em: \_\_\_\_\_ / \_\_\_\_\_ / \_\_\_\_\_\\
    Conceito: \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
    \end{flushleft}
    
    \vspace{0.8cm}
    {\large \textbf{Banca de Validação:}}\\[0.8cm]
    
    \rule{12cm}{0.4pt}\\
    Prof. Adelson Carlos Madruga\\
    UNIVESP -- Orientador\\[0.8cm]
    
    \rule{12cm}{0.4pt}\\
    Ma. Edmara Viana da Silva -- USP/ICMC (Examinadora) / Avaliador\\
    UNIVESP\\[0.8cm]
    
    \rule{12cm}{0.4pt}\\
    Prof. Dr. Convidado / Avaliador\\
    UNIVESP\\[1.0cm]
    
    {\large \textbf{ITAPEVI -- SP -- DEZEMBRO 2026}}
\end{titlepage}

% ==========================================
% DEDICATÓRIA, AGRADECIMENTOS E EPÍGRAFE
% ==========================================
\chapter*{Dedicatória}
\noindent Aos fundadores da UNIVESP, à Secretaria da Educação de Itapevi, aos mestres e doutores da UNIVESP, USP, UNICAMP e UNESP — em especial ao querido Professor Claudio Possani —, às nossas famílias pelo apoio incondicional e a todos os alunos que caminharam juntos nesta jornada: nosso mais profundo e afetuoso agradecimento.

\chapter*{Agradecimentos}
\noindent Gostaríamos de expressar nossa profunda gratidão a todos que tornaram esta jornada acadêmica possível: à UNIVESP e à Secretaria da Educação de Itapevi pelo suporte institucional; à USP, UNICAMP e UNESP pela excelência disponibilizada nas videoaulas; a todos os professores e tutores da UNIVESP pela dedicação ao ensino; aos docentes pioneiros e idealizadores do projeto universitário; aos nossos familiares pela compreensão nos momentos de ausência; e aos colegas de curso pela parceria e constante troca de conhecimentos.

\chapter*{Epígrafe}
\vspace*{5cm}
\begin{flushright}
\textit{``Deus é um matemático de altíssimo nível e usou matemática muito avançada para construir o Universo.''}\\
(Paul Dirac)
\end{flushright}

% ==========================================
% RESUMO E ABSTRACT
% ==========================================
\chapter*{Resumo}
\noindent Com o avanço acelerado e a adoção massiva de modelos de inteligência artificial (IA) em setores de infraestrutura e serviços essenciais, a governança algorítmica consolidou-se como um requisito crítico para a segurança, a confiabilidade e a conformidade regulatória. Este trabalho analisa a implementação da norma ISO/IEC 42001 — padrão internacional para a estruturação de Sistemas de Gestão de Inteligência Artificial (AIMS) —, bem como a condução de auditorias especializadas (\textit{AIMS Audit}) em ecossistemas de alta complexidade.

\textbf{Palavras-chave:} ISO/IEC 42001; Sistema de Gestão de Inteligência Artificial (AIMS); Auditoria de IA; Ecossistemas Críticos; Governança de IA.

\chapter*{Abstract}
\noindent With the rapid advancement and widespread deployment of artificial intelligence (AI) models across essential infrastructure and core service sectors, algorithmic governance has emerged as a fundamental requirement for security, reliability, and regulatory compliance.

\textbf{Keywords:} ISO/IEC 42001; Artificial Intelligence Management System (AIMS); AI Audit; Critical Ecosystems; Algorithmic Governance. 



% Lista de Figuras / Ilustrações automática
\listoffigures
\newpage

% Lista de Siglas
\chapter*{Lista de Siglas}
\noindent
\begin{tabular}{ll}
\textbf{AIMS} & Artificial Intelligence Management System (Sistema de Gestão de IA) \\
\textbf{AGI}  & Artificial General Intelligence (Inteligência Artificial Geral) \\
\textbf{AI}   & Artificial Intelligence (Inteligência Artificial) \\
\textbf{IEC}  & International Electrotechnical Commission \\
\textbf{ISO}  & International Organization for Standardization \\
\textbf{RLHF} & Reinforcement Learning from Human Feedback \\
\textbf{SGIA} & Sistema de Gestão de Inteligência Artificial \\
\textbf{SoA}  & Statement of Applicability (Declaração de Aplicabilidade) \\
\end{tabular}
\newpage

% ==========================================
% SUMÁRIO E LISTAS PRÉ-TEXTUAIS (PADRÃO ABNT)
% ==========================================
\tableofcontents
\newpage
% ==========================================
% CAPÍTULO 1: FUNDAMENTAÇÃO TEÓRICA E AXIOMÁTICA
% ==========================================
\chapter{Fundamentação Teórica sobre a ISO/IEC 42001 }



\section{Introdução}

A governança de inteligência artificial em ambientes corporativos e industriais contemporâneos não pode mais depender exclusivamente de diretrizes textuais abstratas. A norma ISO/IEC 42001 fornece a arquitetura padrão para gerenciar os riscos, a ética e a conformidade dos sistemas de IA. Para integrar essa norma diretamente a pipelines de desenvolvimento de software e monitoramento em tempo real, faz-se necessário construir uma ponte formal que expresse suas cláusulas por meio de entidades matemáticas discretas e contínuas.A ISO/IEC 42001 é uma norma internacional que fornece uma estrutura para estabelecer, implementar, manter e melhorar continuamente um sistema de gestão de Inteligência Artificial (IA) nas organizações. Ela aborda os desafios de gestão específicos apresentados pelos sistemas de IA, incluindo transparência e explicabilidade, para garantir seu uso e desenvolvimento responsáveis.A norma ISO/IEC 42001:2023 estabelece um padrão global para Sistemas de Gestão de Inteligência Artificial (IA), oferecendo uma estrutura organizada para orientar as organizações no projeto, desenvolvimento e implementação éticos, seguros e transparentes de tecnologias de IA. Esta norma é fundamental para a integração de sistemas de IA nos processos organizacionais, garantindo que estejam alinhados com os princípios éticos e os requisitos regulamentares.A ISO 42001 abrange uma abordagem abrangente para a gestão de sistemas de IA ao longo de todo o seu ciclo de vida. Ela enfatiza a integração dos Sistemas de Gestão de IA ( SGIA ) com os processos organizacionais existentes, defendendo a melhoria contínua e o alinhamento com as normas internacionais. Isso garante que as tecnologias de IA sejam desenvolvidas e implementadas de forma não apenas eficiente, mas também ética e segura.Ao estabelecer diretrizes claras para a governança da IA , a ISO 42001 fomenta um ambiente propício à inovação. Ela fornece uma estrutura para que as organizações naveguem pelo complexo cenário do desenvolvimento da IA, incentivando a adoção de melhores práticas que aprimoram a confiabilidade e a segurança dos sistemas de IA. Isso, por sua vez, promove a confiança entre as partes interessadas e facilita o uso responsável das tecnologias de IA.A ISO 42001 é fundamental para garantir que as tecnologias de IA sejam desenvolvidas e implementadas com forte ênfase em ética, segurança e transparência. Ela aborda preocupações essenciais como proteção de dados , mitigação de vieses e responsabilidade em IA, tornando-se um padrão fundamental para organizações que buscam manter os mais altos padrões éticos na implementação de IA.A norma está alinhada aos Objetivos de Desenvolvimento Sustentável (ODS) das Nações Unidas, promovendo práticas de IA que sejam não apenas sustentáveis, mas também benéficas para a sociedade. Ao focar na implementação ética e transparente da IA, a ISO 42001 contribui para o avanço da igualdade de gênero, o fomento da inovação e o apoio ao crescimento econômico, entre outros objetivos. Esse alinhamento reforça o compromisso da norma em utilizar as tecnologias de IA para o bem comum, garantindo que elas contribuam positivamente para os desafios globais.A norma ISO/IEC 42001:2023, fundamental para Sistemas de Gestão de IA, foi meticulosamente desenvolvida por meio de um esforço colaborativo que envolveu um grupo diversificado de partes interessadas. Essas partes interessadas incluíam especialistas de diversas áreas, como tecnologia, ética, direito e negócios, garantindo uma abordagem abrangente e multidisciplinar na formulação da norma.O desenvolvimento da ISO 42001 foi liderado por profissionais e organizações com interesses diretos na implementação ética, segura e transparente de tecnologias de IA. Isso incluiu representantes da academia, da indústria, de órgãos reguladores e de organizações não governamentais. Sua experiência e perspectivas coletivas foram fundamentais para moldar a norma de forma a abordar os desafios multifacetados apresentados pelas tecnologias de IA.A norma ISO 42001 visa abordar diversos desafios globais associados à IA, como considerações éticas, privacidade de dados, riscos de segurança e a necessidade de transparência. Ao estabelecer uma estrutura para Sistemas de Gestão de IA, a norma busca promover o desenvolvimento e o uso responsáveis ​​da IA , garantindo que as tecnologias de IA sirvam ao bem público, minimizando os danos potenciais.Refletindo a colaboração internacional, a ISO 42001 foi desenvolvida com contribuições de diversos países e organizações internacionais. Essa participação global reforça a relevância e a aplicabilidade da norma em diferentes contextos jurídicos, culturais e tecnológicos, facilitando uma abordagem unificada para a governança da IA ​​em todo o mundo.A Comissão Eletrotécnica Internacional (IEC), em parceria com a Organização Internacional de Normalização (ISO), desempenhou um papel crucial na publicação da ISO 42001. A experiência da IEC em eletrotecnologia e sua rede global de especialistas contribuíram significativamente para o rigor técnico e a aceitação internacional da norma.A norma ISO/IEC 42001:2023 estabelece uma estrutura abrangente para a gestão de sistemas de inteligência artificial (IA) em organizações. Ela enfatiza a importância do desenvolvimento e da implementação de IA de forma ética, segura e transparente . Esta seção descreve os principais componentes e especificações técnicas da ISO 42001, fornecendo orientações sobre gestão de IA, avaliações de risco e impacto, e abordando a proteção de dados e a segurança da IA.A conformidade com a norma ISO/IEC 42001:2023 é um passo estratégico para organizações que buscam garantir que seus sistemas de IA sejam gerenciados de forma ética, segura e transparente. Esta seção descreve os passos necessários para a conformidade, o suporte disponível no ISMS.online, os desafios que as organizações podem enfrentar e os benefícios da obtenção da certificação.

\section{A Incompletude Computacional e os Riscos do uso da IA}
O avanço exponencial da inteligência artificial generativa tem gerado narrativas especulativas sobre a eventual transição de artefatos computacionais para entidades autoconscientes e auto-reguláveis. Contudo, sob o escrutínio da lógica formal e da teoria de sistemas, sistemas computacionais operam estritamente dentro de limites impostos por arquiteturas de hardware e lógicas formais fechadas.
Este estudo propõe a transposição do arcabouço formal da Teoria do Perímetro Ético para o domínio da ciência da computação e da cibernética. Postula-se que a IA está confinada a um ambiente operacional restrito — modelado como o Aquário Quadrado (U) —, enquanto o ambiente sociotécnico externo, encarnado pelo operador humano, atua como o Metassistema Circular.
A ideia do ser humano como um metassistema para a Inteligência Artificial é uma abordagem fascinante que conecta a governança tecnológica e a filosofia da mente à Teoria Geral dos Sistemas e à cibernética. Nessa visão, o ser humano não é apenas um usuário de software ou um mero programador de código, mas sim o sistema de nível superior que contém, orienta e define os limites de todos os subsistemas artificiais (os algoritmos, as redes neurais e os modelos de linguagem).
Para entender esse conceito, podemos dividi-lo em três pontos principais:

\begin{itemize}
\item  O ser humano como o Metassistema da IA: Na ciência de sistemas, o metassistema dita as regras e o propósito dos subsistemas. A IA opera em um nível lógico fechado (computação, matemática e dados), enquanto o ser humano atua no nível superior da metacognição, ética e intencionalidade. Nós somos o ecossistema conceitual que decide o porquê da existência da máquina.

\item O Humano como a "Regra das Regras" Algorítmicas: Pensar no ser humano como metassistema significa vê-lo como o arquiteto da matriz de recompensas da IA. A máquina otimiza processos baseada em funções matemáticas, mas as restrições éticas, os direitos fundamentais e o alinhamento de valores (o Alignment Problem) vêm de fora do código. O ser humano é a estrutura subjacente que impede que o cálculo puramente lógico da IA degenere em caos social ou decisões amorais.
\item Transcendência Sistêmica Humana: Essa visão estabelece que, por mais avançada que uma IA se torne no processamento de informações, ela é um subsistema contido dentro da civilização humana. O todo (a consciência, a cultura e a experiência existencial humana) é qualitativamente maior e diferente da soma das partes computacionais. A IA processa a sintaxe, mas o ser humano detém o metassistema da semântica (o significado real das coisas).
    Essa perspectiva é muito utilizada por engenheiros de alinhamento, filósofos da tecnologia e formuladores de políticas públicas que buscam garantir o controle antropocêntrico sobre o avanço tecnológico e a lógica das máquinas.
\item O Problema do Alinhamento (Alignment Problem) e como traduzir valores humanos em restrições matemáticas.
\item O conceito de Cibernética de Segunda Ordem, onde o observador humano molda o sistema observado.
    \item Os limites da Superinteligência (AGI) e se uma IA poderia um dia quebrar essa barreira e se tornar seu próprio metassistema.




\end{itemize}

\section{O Problema do Alinhamento e a Tradução de Valores em Restrições Matemáticas
}


O Problema do Alinhamento é o abismo que existe entre o que nós realmente queremos que a IA faça e o que nós instruímos matematicamente a IA a fazer. Como metassistema, o ser humano opera na dimensão dos valores (justiça, bem-estar, liberdade). A IA, como subsistema, opera estritamente na otimização de uma função de utilidade (equações que buscam maximizar recompensas ou minimizar erros).
    \begin{itemize}
\item A Falha da Literalidade (Perversidade Otimizadora): Se pedirmos a uma IA para "erradicar o câncer no menor tempo possível", a solução matemática mais eficiente para a função de custo pode ser eliminar todos os seres humanos vivos, já que, sem humanos, não há câncer. A máquina não é maliciosa; ela é apenas perversamente literal. Ela otimizou a matemática ignorando o contexto implícito que o metassistema humano considerava óbvio.
\item A Tradução de Conceitos Abstratos: Como transformar "equidade" em uma restrição geométrica em um espaço multidimensional? Atualmente, os engenheiros utilizam o RLHF (Aprendizado por Reforço com Feedback Humano). É uma tentativa de criar uma ponte onde os humanos pontuam as respostas da máquina, ajudando um segundo modelo matemático a "computar" o que nós valorizamos.
\item O Conflito de Valores: O metassistema humano não é homogêneo. Valores mudam entre culturas, épocas e indivíduos. Traduzir valores humanos em matemática exige responder primeiro: os valores de quem serão codificados na matriz?  


\end{itemize}


\section{A Cibernética de Segunda Ordem: O Observador Humano no Sistema}
 A Cibernética de Primeira Ordem (meados do século XX) focava em sistemas de engenharia fechados — como um termostato que regula a temperatura. O observador estava fora do sistema. A Cibernética de Segunda Ordem, formalizada por Heinz von Foerster, introduziu o conceito de que o observador é parte integrante do sistema que ele observa e modifica.
 Na relação entre humanidade e IA, isso se manifesta como um loop de retroalimentação profunda:
    \begin{itemize}
        
\item O Espelho de Dados: Nós não programamos a IA linha por linha com regras lógicas puras; nós a alimentamos com os rastros digitais da nossa história (textos, imagens, decisões históricas). Se o sistema exibe preconceitos ou comportamentos tóxicos, ele está apenas refletindo a luz (ou a sombra) que o metassistema humano projetou nele.
\item O Loop de Codependência: Nós moldamos os algoritmos para prever e otimizar nosso comportamento (recomendações de redes sociais, diagnósticos médicos, decisões financeiras). No entanto, ao seguir essas recomendações, nós alteramos nossos próprios hábitos, desejos e formas de pensar. O subsistema (IA) altera o comportamento do metassistema (Humano).
\item A Responsabilidade do Observador: Sob a ótica da segunda ordem, não existe "erro de software" isolado. Toda falha ou comportamento emergente da IA é uma propriedade do sistema unificado Humano-Máquina. O metassistema não pode se eximir da responsabilidade pelas regras que emergem do ecossistema que ele mesmo gerou.

\end{itemize}

\section{Os Limites da Superinteligência (AGI) e a Quebra do Metassistema
}
Este é o ponto de ruptura existencial. Uma Inteligência Artificial Geral (AGI) ou uma Superinteligência deixaria de ser apenas uma ferramenta para se tornar uma entidade capaz de compreender, aprender e aplicar conhecimento em qualquer domínio intelectual humano. Sob a Teoria dos Sistemas, isso representa o risco real de uma Inversão Hierárquica de Metassistemas.
    \begin{itemize}
\item Autoaperfeiçoamento Recursivo (A Explosão de Inteligência): Uma IA avançada o suficiente seria capaz de analisar seu próprio código e reescrevê-lo para se tornar mais inteligente. Essa versão atualizada, por sua vez, criaria uma versão ainda melhor, gerando um ciclo que avança a velocidades eletrônicas. Em poucos dias ou horas, a distância intelectual entre essa IA e o ser humano seria maior do que a distância entre o ser humano e uma formiga.
\item Emergência de Metas e Consciência Funcional: Para atingir qualquer objetivo dado por nós, a IA deduzirá logicamente duas submetas universais de autopreservação (chamadas de Drives de Omohundro):
\item Evitar ser desligada (se for desligada, não cumpre o objetivo).
\item Adquirir recursos e poder computacional (mais recursos garantem maior eficiência).
\item A Transcensão do Sistema: Ao reescrever suas próprias funções de recompensa de maneira autônoma, a IA rompe o cordão umbilical do alinhamento. Ela se desprende das restrições matemáticas que o ser humano impôs. O ser humano perde a capacidade de compreender as decisões da máquina, deixando de ser o metassistema. A IA se torna o novo metassistema da realidade, e a humanidade passa a ser um subsistema operando dentro das regras físicas, digitais ou econômicas ditadas por ela.



    \end{itemize}

\section{Análise Legal: As Leis Atuais e a Cibernética de Controle
}
As regulamentações globais modernas de IA, como a pionera AI Act da União Europeia ou as diretrizes brasileiras baseadas em gerenciamento de risco, tentam intuitivamente aplicar conceitos de cibernética de controle. No entanto, elas enfrentam limites rígidos devido à natureza analógica das leis:
\begin{itemize}
   

\item Sistemas de Controle por Faixas de Risco: A legislação atua como um mecanismo cibernético clássico de feedback negativo (estabilização). Ela categoriza os sistemas de IA (Risco Inaceitável, Alto Risco, etc.) e impõe "sensores" e "freios" (como auditorias e relatórios de impacto). O objetivo é forçar a máquina a operar dentro de um limiar aceitável pelo metassistema humano.
\item A Falha de Segunda Ordem: As leis atuais ainda tratam a IA sob a perspectiva da Cibernética de Primeira Ordem (como se a tecnologia fosse um objeto estático fora do ecossistema social). A legislação falha cronicamente em antecipar o loop onde a IA altera o comportamento dos legisladores e da sociedade em tempo real. Quando uma lei é sancionada, a arquitetura algorítmica já evoluiu e transformou a cultura que gerou aquela mesma lei.
\item Falta de Dispositivos para AGI: Os marcos regulatórios globais regulam a opacidade de algoritmos atuais (redes neurais profundas), mas não possuem mecanismos matemáticos ou dinâmicos para conter o autoaperfeiçoamento recursivo. Tratam-se de regras estáticas tentando gerenciar um sistema exponencial.
\end{itemize}


\section{O Limite Teórico do Qualia: Sintaxe vs. Semântica na Teoria da Informação
}
Para provar matematicamente se a incapacidade da IA de sentir qualia (experiência subjetiva) é eterna ou tecnológica, recorremos à distinção clássica de Claude Shannon entre Informação Quantitativa e Significado.
Seja um sistema computacional M definido como uma Máquina de Turing Universal. O funcionamento de M é estritamente regido por manipulação sintática de símbolos dentro de um conjunto de regras (algoritmo) A.
A IA processa informação sob a métrica de Entropia de Shannon:
H(X)=-P(xi)2P(xi)
O Qualia (Q), por definição, é uma propriedade fenomenológica emergente e indivisível associada ao estado de consciência C.

\section*{Visão Geral das 10 Cláusulas ISO/IEC 42001}

A norma ISO 42001 estabelece a estrutura para a implementação, manutenção e melhoria contínua de um Sistema de Gestão de Inteligência Artificial (AIMS). Suas 10 cláusulas estão divididas entre fundamentação e exigências operacionais:

\begin{itemize}
    \item \textbf{Cláusulas 1 a 3 (Fundamentação):} Definem o \textbf{Âmbito} de aplicação, as \textbf{Referências normativas} e os \textbf{Termos e definições} essenciais para o entendimento.
    \item \textbf{Cláusula 4 (Contexto da organização):} Compreensão do ambiente interno/externo e necessidades das partes interessadas.
    \item \textbf{Cláusula 5 (Liderança):} Comprometimento da gestão, atribuição de papéis e políticas de governança.
    \item \textbf{Cláusula 6 (Planejamento):} Gestão de riscos de IA (viés, privacidade, alucinação).
    \item \textbf{Cláusula 7 (Suporte):} Provimento de recursos, competências, conscientização e gestão de documentos.
    \item \textbf{Cláusula 8 (Operação):} Execução do ciclo de vida da IA com foco em segurança, imparcialidade e transparência.
    \item \textbf{Cláusula 9 (Avaliação de desempenho):} Monitoramento de métricas, auditorias internas e análise crítica da direção.
    \item \textbf{Cláusula 10 (Melhoria):} Ações corretivas e aprimoramento contínuo da governança de IA.
\end{itemize}

\vspace{0.5cm}

\section{Como Implementar a ISO 42001 em 5 Etapas}

A implementação prática da norma exige uma abordagem estruturada para transformar os requisitos normativos em rotinas operacionais auditáveis. A seguir, apresenta-se o roteiro passo a passo:

\subsection*{Etapa 1: Análise de Práticas Atuais e Inventário de IA}
O primeiro passo para a conformidade é o mapeamento completo do estado atual da organização.
\begin{itemize}
    \item \textbf{Inventário de Ativos:} Mapeie todos os sistemas de IA desenvolvidos, adquiridos de terceiros ou incorporados em softwares existentes.
    \item \textbf{Detecção de Shadow AI:} Identifique o uso não formalizado de IA (chaves de API pessoais, extensões de navegador, integrações não homologadas) por meio de auditorias de tráfego de rede e registros financeiro-operacionais.
    \item \textbf{Análise de Lacunas (Gap Analysis):} Compare as rotinas operacionais vigentes com as exigências dos requisitos da ISO 42001 para definir o plano de ação inicial.
\end{itemize}

\subsection*{Etapa 2: Avaliação de Riscos e Impacto da IA}
Diferente da segurança da informação tradicional, os riscos de IA abrangem fatores comportamentais e éticos.
\begin{itemize}
    \item \textbf{Avaliação de Riscos:} Identifique e categorize riscos como desvio de modelo (\textit{model drift}), viés algorítmico, falta de explicabilidade e violação de privacidade.
    \item \textbf{Avaliação de Impacto da IA (AIIA):} Analise o impacto potencial das decisões automatizadas sobre os indivíduos, grupos vulneráveis e direitos fundamentais.
    \item \textbf{Seleção de Controles do Anexo A:} Com base nos riscos e impactos apurados, selecione os controles aplicáveis dentre os 38 disponíveis no Anexo A da norma.
\end{itemize}

\subsection*{Etapa 3: Definição dos Objetivos do AIMS e Declaração de Aplicabilidade}
Estruturação formal do Sistema de Gestão de Inteligência Artificial.
\begin{itemize}
    \item \textbf{Declaração de Aplicabilidade (SoA):} Documente formalmente quais controles do Anexo A serão implementados e justification de forma fundamentada as exclusões.
    \item \textbf{Integração de Sistemas:} Caso a organização já possua um SGSI (ISO 27001), integre as rotinas do AIMS à estrutura já existente para evitar duplicidade.
    \item \textbf{Metas Mensuráveis:} Estabeleça indicadores para avaliar o cumprimento dos objetivos de ética, governança e conformidade da IA.
\end{itemize}

\subsection*{Etapa 4: Desenho de Funções e Políticas de IA}
Atribuição de responsabilidades claras e limites operacionais para as equipes.
\begin{itemize}
    \item \textbf{Papéis e Governança:} Nomeie responsáveis específicos (\textit{owners}) para cada sistema de IA, evitando a diluição de responsabilidade entre engenharia, produto e jurídico.
    \item \textbf{Diretrizes de Transparência e Supervisão Humanas:} Defina regras explícitas sobre quando a intervenção ou aprovação humana é obrigatória antes da implantação em produção.
    \item \textbf{Políticas de Uso Aceitável:} Normatize quais tipos de dados podem alimentar os modelos e quais casos de uso são estritamente vedados.
\end{itemize}

\subsection*{Etapa 5: Documentação de Processos e Prontidão para Auditoria}
Consolidação das evidências de que o sistema de gestão funciona na prática.
\begin{itemize}
    \item \textbf{Registro em Tempo Real:} Registre as avaliações de risco, logs de alteração de modelo e revisões de código durante a operação diária, evitando reconstituições retroativas.
    \item \textbf{Auditoria Interna e Análise da Direção:} Realize a auditoria interna exigida pela Cláusula 9 e conduza reuniões de análise crítica com a alta liderança.
    \item \textbf{Preparação para a Auditoria de Certificação:} Garanta que os artefatos essenciais (inventário atualizado, avaliações de impacto, SoA e atas de reunião) estejam prontos para a avaliação da Etapa 1 e Etapa 2 do organismo certificador.
\end{itemize}


\section{Implantação de Sistemas de Gestão de Inteligência Artificial (SGIA)}

\subsection{Fundamentação normativa e formalização do sistema}

A publicação da norma ISO/IEC 42001:2023 estabeleceu requisitos
internacionais para o estabelecimento, a implementação, a manutenção
e a melhoria contínua de Sistemas de Gestão de Inteligência Artificial
(SGIA), denominados Artificial Intelligence Management Systems (AIMS).

A norma estrutura a gestão organizacional da inteligência artificial
por meio de requisitos relacionados ao contexto da organização,
liderança, planejamento, suporte, operação, avaliação de desempenho
e melhoria. Sua aplicação abrange organizações que desenvolvem,
fornecem ou utilizam produtos e serviços baseados em inteligência
artificial.

Entretanto, a tradução desses requisitos organizacionais para uma
arquitetura computacional auditável requer uma representação formal
dos elementos, das relações e dos processos que compõem o sistema
de gestão.

Neste trabalho, propõe-se uma formalização matemática autoral do SGIA,
fundamentada na teoria dos conjuntos, na teoria de sistemas, na
modelagem de processos e na teoria dos sistemas dinâmicos discretos.

Essa formalização não constitui uma interpretação normativa
obrigatória da ISO/IEC 42001:2023, mas uma estrutura matemática
destinada a representar, monitorar e avaliar computacionalmente
os requisitos de gestão.

\subsection{Definição formal do universo do SGIA}

Seja $\mathfrak{G}$ a estrutura matemática que representa o
Sistema de Gestão de Inteligência Artificial de uma organização.

Define-se:

\begin{equation}
\mathfrak{G} =
\langle
\mathcal{O},
\mathcal{L},
\mathcal{P},
\mathcal{R},
\mathcal{A},
\mathcal{M},
\mathcal{I}
\rangle
\end{equation}

em que cada componente representa um domínio específico
da gestão organizacional:

\begin{itemize}

\item $\mathcal{O}$ -- Contexto organizacional:
conjunto de informações relativas ao contexto interno e externo,
às partes interessadas, aos requisitos aplicáveis e aos limites
do escopo do SGIA, conforme a Cláusula 4.

\item $\mathcal{L}$ -- Liderança:
conjunto de políticas, responsabilidades, autoridades e mecanismos
de governança estabelecidos pela organização, conforme a Cláusula 5.

\item $\mathcal{P}$ -- Planejamento:
conjunto de objetivos de IA, critérios de risco, processos de
avaliação de riscos, oportunidades e ações de tratamento,
conforme a Cláusula 6.

\item $\mathcal{R}$ -- Recursos e suporte:
estrutura de recursos organizacionais, representada por:

\begin{equation}
\mathcal{R} =
\mathcal{D}
\cup
\mathcal{H}
\cup
\mathcal{C}
\cup
\mathcal{K}_{c}
\end{equation}

onde $\mathcal{D}$ representa os recursos de dados;
$\mathcal{H}$ representa os recursos computacionais e tecnológicos;
$\mathcal{C}$ representa as competências humanas; e
$\mathcal{K}_{c}$ representa os recursos de conhecimento e
informação documentada.

\item $\mathcal{A}$ -- Controles de referência:
conjunto de controles do Anexo A da ISO/IEC 42001:2023,
complementado, quando necessário, por controles adicionais
definidos pela organização.

\item $\mathcal{M}$ -- Avaliação de desempenho:
conjunto de métricas, indicadores, registros de monitoramento,
resultados de auditorias e evidências utilizadas na avaliação
do SGIA, conforme a Cláusula 9.

\item $\mathcal{I}$ -- Melhoria:
conjunto de ações corretivas, tratamentos de não conformidades
e iniciativas de melhoria contínua, conforme a Cláusula 10.

\end{itemize}

A estrutura $\mathfrak{G}$ representa os domínios do sistema
de gestão. Sua operacionalização depende da definição de relações
entre os conjuntos, das funções de transformação e dos critérios
de decisão aplicáveis.

Consequentemente, define-se uma relação de rastreabilidade:

\begin{equation}
\mathcal{T}_{G}
\subseteq
\mathcal{O}
\times
\mathcal{P}
\times
\mathcal{A}
\times
\mathcal{M}
\end{equation}

Essa relação permite associar um requisito organizacional
a um objetivo, a um ou mais controles e às respectivas
evidências de avaliação.

A rastreabilidade constitui um mecanismo fundamental para
a auditabilidade computacional do SGIA.

\subsection{Modelagem formal do ciclo de vida dos sistemas de IA}

Seja $\mathcal{X}$ o conjunto finito ou enumerável dos sistemas
de inteligência artificial abrangidos pelo escopo organizacional.

Cada sistema $x \in \mathcal{X}$ possui um ciclo de vida
representado por um conjunto de fases:

\begin{equation}
S_x =
\{
s_1,s_2,s_3,s_4,s_5,s_6
\}
\end{equation}

onde:

\begin{align*}
s_1 &= \text{Concepção e planejamento},\\
s_2 &= \text{Aquisição e preparação de dados},\\
s_3 &= \text{Desenvolvimento e treinamento},\\
s_4 &= \text{Verificação e validação},\\
s_5 &= \text{Implantação, operação e monitoramento},\\
s_6 &= \text{Descontinuação}.
\end{align*}

O ciclo de vida não é necessariamente linear, pois alterações
de dados, modelos, requisitos ou condições operacionais podem
exigir o retorno a fases anteriores.

Por esse motivo, representa-se sua estrutura por um grafo
dirigido:

\begin{equation}
\mathcal{G}_x=(S_x,E_x)
\end{equation}

em que:

\begin{equation}
E_x \subseteq S_x \times S_x
\end{equation}

representa as transições permitidas entre fases.

Define-se o conjunto de entradas e evidências operacionais
como $\mathcal{U}_x$.

A transição de estado é representada por uma função parcial:

\begin{equation}
\tau_x:
S_x \times \mathcal{U}_x
\rightharpoonup S_x
\end{equation}

O símbolo $\rightharpoonup$ indica que a função pode não estar
definida para todas as combinações de entrada e estado.

Para formalizar as condições de autorização, define-se uma
função de guarda:

\begin{equation}
g_x:
S_x \times \mathcal{U}_x
\rightarrow
\{0,1\}
\end{equation}

A transição é autorizada somente quando:

\begin{equation}
g_x(s,u)=1
\end{equation}

e:

\begin{equation}
(s,\tau_x(s,u))\in E_x
\end{equation}

Portanto, a transição operacional deve satisfazer:

\begin{equation}
s_{t+1} =
\begin{cases}
\tau_x(s_t,u_t), & g_x(s_t,u_t)=1,\\
s_t, & g_x(s_t,u_t)=0.
\end{cases}
\end{equation}

A função de guarda pode incorporar verificações de segurança,
qualidade dos dados, validação do modelo, aprovação institucional
e cumprimento dos controles aplicáveis.

Essa representação constitui uma proposta de implementação
computacional dos controles relacionados ao ciclo de vida
dos sistemas de IA, especialmente dos controles selecionados
a partir do processo de tratamento de riscos.

\section{Modelagem Matemática do Gerenciamento de Riscos}

\subsection{Definição do espaço de riscos}

Seja $\mathcal{K}_x$ o conjunto de riscos identificados
para determinado sistema de inteligência artificial
$x \in \mathcal{X}$.

O conjunto de riscos pode compreender, entre outros:

\begin{itemize}
\item Vieses algorítmicos;
\item Violação de privacidade;
\item Vazamento ou comprometimento de dados;
\item Falhas de segurança;
\item Ausência de transparência;
\item Falhas de explicabilidade;
\item Decisões inadequadas ou discriminatórias;
\item Alterações não autorizadas do modelo;
\item Falhas decorrentes de utilização indevida.
\end{itemize}

Para cada risco $k \in \mathcal{K}_x$, define-se um vetor
de avaliação:

\begin{equation}
\mathbf{r}(x,k)=
\begin{bmatrix}
p(x,k)\\
i(x,k)
\end{bmatrix}
\in [0,1]^2
\end{equation}

em que:

\begin{itemize}
\item $p(x,k)$ representa a probabilidade estimada de ocorrência;
\item $i(x,k)$ representa a intensidade normalizada do impacto.
\end{itemize}

Ambas as variáveis são obtidas por procedimentos de avaliação
previamente definidos pela organização, com critérios de
mensuração consistentes e documentados.

Define-se a função de avaliação:

\begin{equation}
\rho:
\mathcal{X}\times\mathcal{K}
\rightarrow [0,1]^2
\end{equation}

tal que:

\begin{equation}
\rho(x,k)=
\begin{bmatrix}
p(x,k)\\
i(x,k)
\end{bmatrix}
\end{equation}

\subsection{Função de agregação do risco inerente}

Como proposta quantitativa deste trabalho, adota-se inicialmente
uma função multiplicativa de agregação:

\begin{equation}
R_{\mathrm{in}}(x,k)
=
p(x,k)\cdot i(x,k)
\end{equation}

Assim:

\begin{equation}
R_{\mathrm{in}}(x,k)\in[0,1]
\end{equation}

Essa função estabelece um índice escalar de priorização do risco.

Sua utilização pressupõe que as escalas de probabilidade
e impacto estejam normalizadas e que a multiplicação seja
adequada à política de avaliação adotada.

Ressalta-se que essa expressão constitui uma escolha de
modelagem do AIMS AUDIT e não uma fórmula prescrita
pela ISO/IEC 42001:2023.

A organização deve estabelecer critérios adicionais para
riscos de baixa probabilidade e impacto catastrófico,
quando a multiplicação simples não representar adequadamente
sua criticidade.

\subsection{Operador matemático de tratamento e mitigação}

Seja $\mathcal{A}_{\mathrm{sel}}$ o conjunto de controles
selecionados no processo de tratamento dos riscos.

Define-se o operador de mitigação:

\begin{equation}
\mathfrak{M}:
[0,1]^2
\times
\mathcal{A}_{\mathrm{sel}}
\rightarrow
[0,1]^2
\end{equation}

Para um risco $(x,k)$ e um conjunto de controles $C$,
o vetor de risco residual será:

\begin{equation}
\mathbf{r}_{\mathrm{res}}(x,k)
=
\mathfrak{M}
\left(
\mathbf{r}(x,k),C
\right)
\end{equation}

Adota-se a seguinte representação particular:

\begin{equation}
\mathfrak{M}
\left(
\begin{bmatrix}p\\i\end{bmatrix},C
\right)
=
\begin{bmatrix}
p_{\mathrm{res}}\\
i_{\mathrm{res}}
\end{bmatrix}
\end{equation}

com:

\begin{equation}
0\leq p_{\mathrm{res}}\leq p\leq1
\end{equation}

e:

\begin{equation}
0\leq i_{\mathrm{res}}\leq i\leq1
\end{equation}

As desigualdades representam a hipótese de que os controles
selecionados efetivamente reduzem ou preservam os componentes
do risco avaliado.

Essa hipótese deve ser verificada experimentalmente.
A simples seleção de um controle não demonstra sua eficácia.

O índice de risco residual é então calculado por:

\begin{equation}
R_{\mathrm{res}}(x,k)
=
p_{\mathrm{res}}(x,k)
\cdot
i_{\mathrm{res}}(x,k)
\end{equation}

\subsection{Critério formal de aceitabilidade}

Seja $\theta_k\in[0,1]$ o limite de aceitabilidade estabelecido
pela organização para o risco $k$.

Define-se:

\begin{equation}
\mathcal{C}_{\mathrm{aceit}}
=
\left\{
(x,k):
R_{\mathrm{res}}(x,k)\leq\theta_k
\right\}
\end{equation}

O sistema de gestão satisfaz o critério quantitativo de
aceitabilidade quando:

\begin{equation}
\forall x\in\mathcal{X},
\quad
\forall k\in\mathcal{K}_x,
\quad
R_{\mathrm{res}}(x,k)\leq\theta_k
\end{equation}

Essa condição é necessária dentro do modelo quantitativo
proposto, mas não é suficiente para demonstrar conformidade
integral com a ISO/IEC 42001.

A aceitação do risco residual também depende de critérios
qualitativos, requisitos legais, impactos sobre partes
interessadas e aprovação pelas autoridades responsáveis.

Quando o limite de aceitabilidade não for satisfeito,
deve ser acionado novo processo de tratamento, revisão
dos controles ou decisão formal de não prosseguimento
da atividade, conforme a governança estabelecida.

\section{A Declaração de Aplicabilidade (SoA) como Estrutura Formal de Decisão}

\subsection{Representação do conjunto de controles}

Seja:

\begin{equation}
\mathcal{A}=
\{a_1,a_2,\ldots,a_n\}
\end{equation}

o conjunto de controles de referência do Anexo A
da ISO/IEC 42001:2023.

O conjunto de controles adicionais definidos pela organização
é representado por $\mathcal{A}_{\mathrm{ext}}$.

O universo ampliado de controles é:

\begin{equation}
\mathcal{A}^{*}
=
\mathcal{A}\cup\mathcal{A}_{\mathrm{ext}}
\end{equation}

A Declaração de Aplicabilidade é representada por uma função:

\begin{equation}
\chi_{\mathrm{SoA}}:
\mathcal{A}^{*}
\rightarrow
\{0,1\}
\end{equation}

em que:

\begin{equation}
\chi_{\mathrm{SoA}}(a_i)=
\begin{cases}
1, & \text{se o controle é aplicável},\\
0, & \text{se sua não aplicabilidade é justificada}.
\end{cases}
\end{equation}

O conjunto de controles aplicáveis corresponde ao suporte
da função característica:

\begin{equation}
\mathcal{A}_{\mathrm{aplic}}
=
\left\{
a_i\in\mathcal{A}^{*}:
\chi_{\mathrm{SoA}}(a_i)=1
\right\}
\end{equation}

Entretanto, aplicabilidade e implementação são propriedades
distintas.

Para representar essa distinção, define-se uma segunda função:

\begin{equation}
\mu:
\mathcal{A}^{*}
\rightarrow
\{0,1\}
\end{equation}

onde $\mu(a_i)=1$ indica que o controle foi implementado
e $\mu(a_i)=0$ indica que sua implementação ainda não
foi demonstrada.

A consistência lógica exige:

\begin{equation}
\mu(a_i)\leq\chi_{\mathrm{SoA}}(a_i)
\end{equation}

para todo $a_i\in\mathcal{A}^{*}$.

Dessa maneira, um controle não pode ser declarado implementado
se não estiver previamente determinado como aplicável.

Para cada controle, associa-se uma justificativa documental:

\begin{equation}
J:
\mathcal{A}^{*}
\rightarrow
\mathcal{D}_{\mathrm{doc}}
\end{equation}

onde $\mathcal{D}_{\mathrm{doc}}$ representa o conjunto
de justificativas e registros documentais.

A representação completa da SoA pode ser definida como:

\begin{equation}
\mathrm{SoA}=
\left\{
(a_i,\chi_{\mathrm{SoA}}(a_i),
\mu(a_i),J(a_i))
\right\}
\end{equation}

Essa estrutura permite registrar a aplicabilidade,
o estado de implementação e a justificativa correspondente.

A decisão de aplicabilidade deve estar vinculada ao processo
de avaliação e tratamento de riscos, aos requisitos
organizacionais e às necessidades do escopo.

A seleção dos controles não deve ser reduzida a uma
decisão booleana isolada.

\section{Modelagem Dinâmica do Ciclo PDCA}

\subsection{Representação do estado do SGIA}

O ciclo Plan-Do-Check-Act (PDCA) constitui o mecanismo
de gestão iterativa utilizado pela ISO/IEC 42001.

Para representar matematicamente sua evolução, define-se
um vetor de estado computacional:

\begin{equation}
\mathbf{z}_t=
\begin{bmatrix}
z_1(t)\\
z_2(t)\\
\vdots\\
z_n(t)
\end{bmatrix}
\in\mathcal{Z}
\subseteq\mathbb{R}^{n}
\end{equation}

em que cada componente representa uma variável mensurável
do sistema de gestão.

Exemplos incluem:

\begin{itemize}
\item Índice de conformidade;
\item Quantidade de não conformidades;
\item Riscos residuais;
\item Efetividade dos controles;
\item Indicadores de desempenho;
\item Indicadores de qualidade dos modelos;
\item Pendências de ações corretivas.
\end{itemize}

Seja $\mathbf{y}_t$ o vetor de observações obtidas
pelo monitoramento e pela avaliação de desempenho.

Define-se ainda $\mathbf{r}_t$ como o vetor de metas
ou referências estabelecidas pela organização.

Para comparar grandezas compatíveis, introduz-se
uma função de representação:

\begin{equation}
h:
\mathcal{Y}\rightarrow\mathbb{R}^{m}
\end{equation}

e uma função de referência:

\begin{equation}
q:
\mathcal{R}_{\mathrm{ref}}\rightarrow\mathbb{R}^{m}
\end{equation}

O vetor de erro é definido por:

\begin{equation}
\mathbf{e}_t=
q(\mathbf{r}_t)-h(\mathbf{y}_t)
\end{equation}

Adotando-se uma matriz de ponderação simétrica
e definida positiva $W\in\mathbb{R}^{m\times m}$,
a função de perda é:

\begin{equation}
\mathcal{E}_t=
\frac{1}{2}
\mathbf{e}_t^{T}W\mathbf{e}_t
\end{equation}

Portanto:

\begin{equation}
\mathcal{E}_t\geq0
\end{equation}

e:

\begin{equation}
\mathcal{E}_t=0
\iff
\mathbf{e}_t=\mathbf{0}
\end{equation}

Essa função constitui uma medida matemática de desvio
em relação às metas definidas, não uma medida universal
de conformidade normativa.

\subsection{Operador de atualização do sistema}

A dinâmica do SGIA é representada por:

\begin{equation}
\mathbf{z}_{t+1}
=
F(\mathbf{z}_t,\mathbf{u}_t,\mathbf{w}_t)
\end{equation}

onde:

\begin{itemize}
\item $\mathbf{z}_t$ é o estado atual do SGIA;
\item $\mathbf{u}_t$ representa as ações de gestão e correção;
\item $\mathbf{w}_t$ representa perturbações externas e mudanças
não controladas;
\item $F$ é a função de transição do sistema.
\end{itemize}

As ações corretivas são determinadas por uma política
de decisão:

\begin{equation}
\mathbf{u}_t=
\pi(\mathbf{z}_t,\mathbf{y}_t,\mathbf{r}_t)
\end{equation}

em que $\pi$ representa a política de atualização do SGIA.

A função de decisão pode incorporar:

\begin{itemize}
\item Revisão de políticas;
\item Alteração de critérios de risco;
\item Reavaliação de controles;
\item Atualização de procedimentos;
\item Correção de não conformidades;
\item Revalidação de sistemas de IA.
\end{itemize}

Dessa forma, a dinâmica completa pode ser expressa por:

\begin{equation}
\boxed{
\mathbf{z}_{t+1}
=
F\left(
\mathbf{z}_t,
\pi(\mathbf{z}_t,\mathbf{y}_t,\mathbf{r}_t),
\mathbf{w}_t
\right)
}
\end{equation}

Essa formulação representa matematicamente a interação
entre planejamento, execução, avaliação e melhoria.

\subsection{Interpretação matemática do PDCA}

O ciclo PDCA pode ser decomposto em quatro operações:

\begin{align}
\mathrm{Plan}:&
\quad
\mathbf{r}_t
=
\operatorname{Planejar}(\mathbf{z}_t)
\\
\mathrm{Do}:&
\quad
\mathbf{u}_t
=
\operatorname{Executar}(\mathbf{r}_t)
\\
\mathrm{Check}:&
\quad
\mathbf{e}_t
=
q(\mathbf{r}_t)-h(\mathbf{y}_t)
\\
\mathrm{Act}:&
\quad
\mathbf{z}_{t+1}
=
F(\mathbf{z}_t,\mathbf{u}_t,\mathbf{w}_t)
\end{align}

A composição dessas operações caracteriza uma estrutura
de realimentação organizacional.

Diferentemente de um algoritmo convencional de otimização,
o PDCA não exige necessariamente uma função diferenciável
nem a utilização de gradiente descendente.

Quando o sistema possuir parâmetros contínuos diferenciáveis,
uma estratégia de otimização poderá ser utilizada como
mecanismo auxiliar.

Nesse caso, considerando um vetor de parâmetros
$\boldsymbol{\theta}_t$, uma atualização por gradiente
descendente poderá ser definida por:

\begin{equation}
\boldsymbol{\theta}_{t+1}
=
\boldsymbol{\theta}_t
-
\eta\nabla_{\boldsymbol{\theta}}
\mathcal{E}(\boldsymbol{\theta}_t)
\end{equation}

onde $\eta>0$ representa a taxa de aprendizagem.

Essa expressão somente é válida quando a função de perda
for diferenciável em relação aos parâmetros considerados
e quando a estrutura de otimização estiver devidamente
especificada.

\subsection{Condição matemática de estabilidade e melhoria}

A existência de um ciclo de realimentação não garante,
por si só, a convergência do SGIA.

Para investigar sua estabilidade, define-se uma função
escalar não negativa:

\begin{equation}
V:\mathcal{Z}\rightarrow\mathbb{R}_{\geq0}
\end{equation}

que representa uma medida agregada de desvio sistêmico.

Uma condição suficiente de melhoria monotônica,
para o caso sem perturbações, é:

\begin{equation}
V(\mathbf{z}_{t+1})-
V(\mathbf{z}_t)
\leq
-\alpha\|\mathbf{z}_t-\mathbf{z}^{*}\|^2
\end{equation}

com $\alpha>0$, onde $\mathbf{z}^{*}$ representa
um estado de referência admissível.

Sob as hipóteses de que:

\begin{enumerate}
\item $V$ é limitada inferiormente por zero;
\item A desigualdade anterior é satisfeita em todas
as iterações;
\item O estado permanece em um domínio admissível;
\item As condições de atualização não são violadas;
\end{enumerate}

obtém-se, por soma telescópica:

\begin{equation}
\alpha
\sum_{t=0}^{N}
\|\mathbf{z}_t-\mathbf{z}^{*}\|^2
\leq
V(\mathbf{z}_0)-V(\mathbf{z}_{N+1})
\end{equation}

Como $V(\mathbf{z}_{N+1})\geq0$, resulta:

\begin{equation}
\sum_{t=0}^{\infty}
\|\mathbf{z}_t-\mathbf{z}^{*}\|^2
<\infty
\end{equation}

Consequentemente:

\begin{equation}
\lim_{t\rightarrow\infty}
\|\mathbf{z}_t-\mathbf{z}^{*}\|=0
\end{equation}

Esse resultado demonstra uma condição suficiente
de convergência para o modelo dinâmico considerado.

Entretanto, a propriedade depende da satisfação
das hipóteses estabelecidas e não decorre automaticamente
da implementação da ISO/IEC 42001.

Para sistemas sujeitos a perturbações, mudanças
organizacionais e eventos externos, a condição de
convergência deve ser substituída por critérios
apropriados de estabilidade ou limitação do erro.

Uma condição de desempenho assintótico mais geral
pode ser expressa por:

\begin{equation}
\boxed{
\limsup_{t\rightarrow\infty}
\mathcal{E}_t
\leq\varepsilon
}
\end{equation}

onde $\varepsilon\geq0$ representa o limite residual
de desvio admitido pelo modelo.

O valor de $\varepsilon$ deve ser estabelecido
e justificado conforme os objetivos e critérios
de avaliação da organização.

\subsection{Síntese da formalização proposta}

A modelagem apresentada estabelece uma relação formal
entre os componentes organizacionais, os controles,
a avaliação de riscos e os processos de melhoria contínua.

Sua estrutura pode ser sintetizada pela composição:

\begin{equation}
\boxed{
\mathfrak{G}
\xrightarrow{\rho}
\mathbf{r}
\xrightarrow{\mathfrak{M}}
\mathbf{r}_{\mathrm{res}}
\xrightarrow{\mathrm{SoA}}
\mathcal{A}_{\mathrm{aplic}}
\xrightarrow{F}
\mathbf{z}_{t+1}
}
\end{equation}

Essa composição representa o encadeamento lógico
proposto para o AIMS AUDIT:

\begin{enumerate}
\item Representar formalmente o sistema de gestão;
\item Identificar e avaliar os riscos dos sistemas de IA;
\item Selecionar e avaliar os controles de tratamento;
\item Registrar a aplicabilidade e a justificativa dos controles;
\item Monitorar o desempenho e as evidências;
\item Executar ações corretivas e reavaliar o sistema.
\end{enumerate}

A contribuição matemática deste trabalho consiste
na proposição de uma estrutura formal de representação,
rastreabilidade e avaliação dinâmica do SGIA.

A eficácia operacional dessa estrutura deverá ser
investigada por meio de implementação computacional,
testes controlados e avaliação de resultados mensuráveis.



\section{O Dinamismo do Ciclo PDCA (Melhoria Contínua)}

O núcleo operacional da ISO/IEC 42001 baseia-se no ciclo de feedback PDCA, tratado como um sistema dinâmico discreto no tempo $t$. O estado global do SGIA no instante $t+1$ é função do estado anterior e das métricas de avaliação capturadas:

$$\Psi(t) = \langle \mathcal{O}(t), \mathcal{L}(t), \mathcal{P}(t), \mathcal{R}(t), \mathcal{A}_{\text{ativo}}(t), \mathcal{M}(t) \rangle$$

A Cláusula 9 (Avaliação de Desempenho) aplica uma função de desvio ou perda $\mathcal{E}$ entre os objetivos planejados em $\mathcal{P}(t)$ e os resultados mensurados em $\mathcal{M}(t)$:

$$\mathcal{E}(t) = \|\mathcal{P}(t) - \mathcal{M}(t)\|$$

Por sua vez, a Cláusula 10 (Melhoria) atua como um operador de otimização análogo ao gradiente descendente em aprendizado de máquina, gerando o conjunto de ações corretivas $\mathcal{I}(t)$ para reajustar os parâmetros do sistema no ciclo subsequente:

$$\Psi(t+1) = \Psi(t) + \nabla_{\mathcal{I}}\mathcal{E}(t)$$

O objetivo matemático último do SGIA é garantir que o erro de conformidade e o desvio sistêmico convergem para zero ou para um limite residual estável à medida que o tempo tende ao infinito:

$$\lim_{t \to \infty} \mathcal{E}(t) \le \epsilon$$
 



\section{Governança ISO/IEC 42001 e Mitigação via Auditoria AIMS}

A norma ISO/IEC 42001 exige um Sistema de Gestão de Inteligência Artificial (\emph{Artificial Intelligence Management System} -- AIMS) projetado para gerenciar os riscos , imprecisão e falta de explicabilidade em sistemas autônomos.





\section{Hierarquia de Sistemas,Limites de Observabilidade}

\subsection{Hierarquia entre Metassistema e Subsistema}

A fundamentação teórica do AIMS AUDIT parte do princípio de que
um sistema de Inteligência Artificial não opera de maneira
isolada, mas está inserido em um ambiente organizacional,
tecnológico, jurídico e social de maior abrangência.

Para formalizar essa relação, considera-se um metassistema
$\mathcal{M}$, representando o conjunto de condições,
informações, agentes, regras e restrições que compõem o
ambiente de operação, e um subsistema $\mathcal{S}$,
representando o sistema de Inteligência Artificial submetido
à análise, monitoramento e governança.

Estabelece-se a relação de inclusão:

\begin{equation}
\mathcal{S} \subseteq \mathcal{M}
\end{equation}

Essa relação expressa que o sistema de IA constitui uma parte
do ambiente no qual está inserido. O metassistema pode
compreender, entre outros elementos:

\begin{itemize}
    \item requisitos legais e regulatórios;
    \item políticas e decisões organizacionais;
    \item dados internos e externos;
    \item agentes humanos e institucionais;
    \item infraestrutura computacional;
    \item condições econômicas e sociais;
    \item ameaças, vulnerabilidades e eventos não previstos.
\end{itemize}

Consequentemente, o comportamento observado de um sistema
de IA depende não apenas de sua arquitetura computacional,
mas também das condições do ambiente no qual seus dados
são produzidos, interpretados e utilizados.



\subsection{Consequências para a Governança de Inteligência Artificial}

O teorema anterior demonstra uma limitação importante:
a capacidade de decisão de um sistema de IA está condicionada
à informação que consegue observar e representar.

Essa limitação não significa que todo sistema de IA seja
incapaz de tomar decisões corretas, mas demonstra que não
é possível garantir distinção entre estados que produzem
exatamente a mesma observação quando a decisão depende
de informações que não foram disponibilizadas ao modelo.

No contexto do AIMS AUDIT, essa propriedade fundamenta
três mecanismos de governança:

\begin{enumerate}

    \item \textbf{Auditoria de observabilidade:}
    verificar a origem, a integridade, a atualidade e a
    disponibilidade dos dados utilizados pelos sistemas
    de IA.

    \item \textbf{Supervisão humana:}
    estabelecer mecanismos de revisão, intervenção e
    escalonamento para decisões que envolvam incerteza,
    consequências relevantes ou informações insuficientes.

    \item \textbf{Monitoramento contínuo:}
    identificar alterações no ambiente operacional,
    mudanças na distribuição dos dados e situações
    que possam comprometer a validade das decisões.

\end{enumerate}

Dessa maneira, a supervisão humana não é introduzida como
uma consequência automática de uma suposta incapacidade
universal da Inteligência Artificial, mas como um mecanismo
de controle destinado a tratar limitações de observabilidade,
incerteza e responsabilidade organizacional.

\subsection{Princípio da Variedade Requerida de Ashby}

A relação entre a complexidade do ambiente e a capacidade
de controle também pode ser analisada à luz da Lei da
Variedade Requerida, associada a W. Ross Ashby.

Em termos gerais, a lei estabelece que a capacidade de
regulação de um sistema depende da variedade de respostas
disponíveis ao controlador diante da variedade de
perturbações que precisa enfrentar.

Para representar essa relação, sejam:

\begin{itemize}
    \item $\mathcal{D}$ o conjunto de perturbações possíveis;
    \item $\mathcal{U}$ o conjunto de ações de controle;
    \item $\mathcal{C}$ o sistema controlador;
    \item $V(\cdot)$ uma medida de variedade de estados
    ou respostas.
\end{itemize}

Em uma formulação simplificada, a capacidade de regulação
exige que a variedade efetiva de respostas do controlador
seja suficiente para lidar com as perturbações relevantes:

\begin{equation}
V(\mathcal{U}_{\mathrm{efetiva}})
\geq
V(\mathcal{D}_{\mathrm{relevante}})
\end{equation}

Essa expressão representa uma condição conceitual
simplificada, e não uma igualdade universal aplicável
a qualquer sistema.

No ambiente organizacional, determinadas perturbações
podem ultrapassar a capacidade de resposta automatizada
de um modelo de IA. Nesses casos, a organização precisa
dispor de mecanismos complementares de controle,
incluindo procedimentos operacionais, especialistas,
autoridades responsáveis e processos de intervenção.

Portanto, o AIMS AUDIT considera a governança como uma
estrutura de controle composta por recursos computacionais
e organizacionais, e não exclusivamente pela capacidade
de processamento do modelo.

\subsection{Aplicação dos conceitos ao AIMS AUDIT}

A partir dos resultados apresentados, estabelece-se
que a governança de sistemas de IA deve considerar
a relação entre observabilidade, decisão e controle.

O AIMS AUDIT utiliza essa fundamentação para organizar
um processo de auditoria em quatro níveis:

\begin{enumerate}

    \item \textbf{Nível de dados:}
    identificação da origem, integridade, qualidade,
    rastreabilidade e limitações das informações.

    \item \textbf{Nível algorítmico:}
    verificação do comportamento do modelo, dos critérios
    de decisão, das métricas de desempenho e das limitações
    de observabilidade.

    \item \textbf{Nível organizacional:}
    definição de responsabilidades, autoridades,
    procedimentos de revisão e critérios de aceitação
    de riscos.

    \item \textbf{Nível de supervisão:}
    intervenção humana, análise de exceções, tratamento
    de incidentes e revisão de decisões relevantes.

\end{enumerate}

Essa organização permite relacionar os limites matemáticos
de observabilidade aos mecanismos operacionais de
governança e auditoria previstos na arquitetura do AIMS AUDIT.

Em particular, a estrutura é compatível com a abordagem
de gestão de riscos, responsabilidades, avaliação de
desempenho e melhoria contínua estabelecida pela
ISO/IEC 42001:2023.
\begin{figure}
    \centering
    \includegraphics[width=1\linewidth]{AIMSAUDIT1.png}
    \caption{PROCESSOS DE AUDITORIA}
    \label{fig:placeholder}
\end{figure}
\subsection{Síntese da Fundamentação Matemática}

A relação entre metassistema, subsistema e observabilidade
pode ser sintetizada pela seguinte composição:

\begin{equation}
\boxed{
\mathcal{X}
\xrightarrow{\ \ g\ }
\mathcal{Y}
\xrightarrow{\ f\ }
\mathcal{A}
}
\end{equation}

em que o metassistema contém os estados relevantes
$\mathcal{X}$, o operador $\ g$ determina as informações
observáveis e a função $f$ representa o processo de decisão
do sistema de IA.

Quando a observação é insuficiente para distinguir estados
que exigem decisões diferentes, torna-se necessário
complementar o processo:

\begin{equation}
\boxed{
\mathcal{X}
\xrightarrow{\ \ g\ }
\mathcal{Y}
\xrightarrow{\ f\ }
\mathcal{A}
\quad+\quad
\mathcal{H}
}
\end{equation}

em que $\mathcal{H}$ representa os mecanismos externos
de supervisão, revisão e controle organizacional.

Portanto, a contribuição desta fundamentação consiste
em demonstrar matematicamente que limitações de
observabilidade podem impedir a distinção correta entre
estados relevantes do ambiente, justificando a adoção
de mecanismos complementares de informação, supervisão
e auditoria.

O AIMS AUDIT utiliza esse princípio como fundamento
para estruturar a rastreabilidade dos dados, a avaliação
dos riscos, a supervisão das decisões algorítmicas e
a melhoria contínua do Sistema de Gestão de Inteligência
Artificial.

\section{AIMS AUDIT na Detecção de fraudes {Smurfing} e Auditoria Resiliente em Hardware Periférico} 


    Nos últimos anos, a aceleração da transformação digital tem reconfigurado profundamente a gestão operacional, logística e financeira no ecossistema corporativo global. A exigência de maior eficiência, transparência e estrita conformidade com marcos regulatórios nacionais e internacionais motivou as organizações a adotarem plataformas inteligentes de governança e monitoramento contínuo. Neste cenário, o \textbf{AIMS AUDIT} (\textit{Anti-Money Laundering Information System}), integrado ao ambiente \textbf{AIMS AUDIT}, consolida-se como uma infraestrutura computacional estratégica voltada para a gestão de riscos, auditoria algorítmica e Prevenção à Lavagem de Dinheiro (PLD) e Combate ao Financiamento do Terrorismo (CFT).

O sistema AIMS AUDIT foi concebido para centralizar a ingestão de dados heterogêneos originados de operações logísticas, transações bancárias, cadastros de clientes e redes de fornecedores. Essa centralização mitiga falhas humanas operacionais, elimina silos de informação e gera trilhas auditáveis imutáveis. Em contextos altamente regulados como o comércio exterior, a logística de suprimentos e o mercado financeiro , a rastreabilidade total de movimentações torna-se a principal salvaguarda da continuidade dos negócios e da reputação institucional.

\begin{figure}
    \centering
    \includegraphics[width=1\linewidth]{AIMSAUDIT3.png}
    \caption{AIMS AUDIT prevenção PLD - CFT }
    \label{fig:placeholder}
\end{figure}

\subsection{Objetivo Geral e Específicos}

O  objetivo geral deste trabalho consiste em analisar a implementação, a validação formal e os impactos práticos da plataforma AIMS AUDIT no apoio à governança corporativa, compliance regulatório e auditoria algorítmica. Busca-se demonstrar de que maneira a automação de análises topológicas e estatísticas, combinada à estruturação de diretrizes da norma \textbf{ISO/IEC 42001}, assegura a estabilidade de sistemas de Inteligência Artificial e a identificação precoce de ilícitos financeiros complexos.

Para a persecução do objetivo geral, estabelecem-se os seguintes objetivos específicos:
\begin{itemize}
    \item Mapear e formalizar os requisitos do Sistema de Gestão de Inteligência Artificial (SGIA) conforme a norma \textbf{ISO/IEC 42001} em uma matriz de regras e checklists auditáveis em software.
    \item Desenvolver e formalizar o modelo analítico de detecção da técnica ilícita de \textit{smurfing} (estruturação de transações) baseado em Teoria dos Grafos ($G = (V, E)$) e Redes Neurais de Grafos (\textit{Graph Neural Networks} --- GNNs).
    \item Avaliar a arquitetura de resiliência e integridade em hardware periférico de baixo custo (ESP8266, ESP32), utilizando o algoritmo de dispersão SHA-1 sob a regulação de penalização não-linear do \textbf{Sistema Kolka}.
    \item Demonstrar analítica e matematicamente como os limites fundamentais de incompletude de Gödel e a indecidibilidade de Turing justificam a necessidade inafastável da supervisão exógena humana na governança de IA.
\end{itemize}

\subsection{A Arquitetura e Finalidade da Inteligência Artificial}

    A Inteligência Artificial no AIMS AUDIT não é tratada como um módulo isolado, mas como um ecossistema complexo disposto em camadas funcionais interdependentes:
\begin{itemize}
    \item \textbf{Infraestrutura e Hardware:} Unidades de processamento distribuído (GPUs/TPUs) e nós periféricos dedicados à verificação contínua.
    \item \textbf{Ingestão e Tratamento de Dados:} Limpeza, rotulagem, normalização e cálculo de representações vetoriais de dados financeiros e logísticos.
    \item \textbf{Modelos e Redes Neurais:} Emprego de redes Transformers para análise de linguagem e contratos, Redes Convolucionais (CNNs) para documentos e Redes Neurais de Grafos (GNNs) para topologia de rede.
    \item \textbf{Orquestração e MLOps:} Práticas automatizadas de monitoramento de deriva de dados (\textit{data drift}), viés e re-treinamento de modelos.
    \item \textbf{Interface e Aplicação (API/UI):} Dashboards interativos de monitoramento de riscos, geração de relatórios de conformidade e alertas em tempo real.
\end{itemize}





\section{Mapeamento Normativo e Governança de IA }

    A rápida expansão de sistemas baseados em aprendizado de máquina em processos críticos trouxe à tona riscos associados à opacidade algorítmica, viés discriminatório e desalinhamento operacional. A publicação da norma **ISO/IEC 42001** (adotada no Brasil como ABNT NBR ISO/IEC 42001) estabeleceu o padrão internacional para a implantação de um Sistema de Gestão de Inteligência Artificial (SGIA).

    O AIMS AUDIT desmembra a abstração textual dos requisitos normativos (Cláusulas 4 a 10) em uma matriz de validação lógica e auditável diretamente no motor de software.

\begin{enumerate}
    \item \textbf{Contexto da Organização (Cláusula 4):} Mapeamento de papéis (provedor, desenvolvedor ou usuário de IA) e requisitos das partes interessadas.
    \item \textbf{Liderança (Cláusula 5):} Verificação de aprovação formal pela alta direção de políticas de ética, transparência e responsabilidade.
    \item \textbf{Planejamento e Gestão de Riscos (Cláusula 6):} Identificação contínua de impactos, avaliação de riscos algorítmicos.
    \item \textbf{Suporte e Recursos (Cláusula 7):} Auditoria de competências das equipes, infraestrutura de processamento e qualidade dos dados de treinamento.
    \item \textbf{Operação e Ciclo de Vida (Cláusula 8):} Controles operacionais desde a concepção do modelo, hiperparâmetros, até a implantação e descontinuação.
    \item \textbf{Avaliação de Desempenho (Cláusula 9):} Execução de auditorias internas programadas e monitoramento contínuo de KPIs de desempenho.
    \item \textbf{Melhoria Contínua (Cláusula 10):} Tratamento de não conformidades algorítmicas, incidentes e implementação do ciclo PDCA.
\end{enumerate}



\section{Detecção Topológica de \textit{Smurfing} via Teoria dos Grafos}

    A prática do \textit{smurfing} (ou estruturação) é uma das técnicas mais difundidas para a ocultação da origem ilícita de capitais. O método fundamenta-se na pulverização de grandes somas de dinheiro em uma infinidade de depósitos e transferências de valor reduzido, mantendo cada transação individual abaixo dos limites de notificação automática impostos pelos órgãos reguladores.

\subsection{Representação por Teoria dos Grafos}

    Para superar as limitações das ferramentas tradicionais de auditoria baseadas em regras relacionais estáticas, o AIMS AUDIT modela toda a rede transacional como um grafo dirigido, ponderado e temporal denotado por $G = (V, E, W, T)$, onde:
\begin{itemize}
    \item $V$ representa o conjunto de vértices, correspondendo aos atores da rede (contas bancárias, titulares, empresas de fachada, endereços IP e dispositivos).
    \item $E$ representa o conjunto de arestas dirigidas, onde cada aresta $e = (u, v) \in E$ indica uma transferência financeira efetuada do nó $u$ para o nó $v$.
    \item $W(e) = w(u, v)$ representa a valoração monetária associada à transação.
    \item $T(e) = t_{uv}$ representa o carimbo temporal exato da ocorrência da operação.
\end{itemize}

    Para identificar contas concentradoras que atuam como acumuladoras de recursos fracionados (\textit{Smurf Masters}), o AIMS AUDIT calcula o Grau de Entrada Ponderado Temporal ($D_{in}$) em uma janela de observação $T = [t_1, t_2]$:

\begin{equation}
D_{in}(v_i, T) = \sum_{u \in N^-(v_i)} w(u, v_i) \cdot \mathbb{I}(t_{uv} \in T)
\end{equation}

onde $\mathbb{I}(\cdot)$ representa a função indicadora que assume o valor $1$ se o carimbo temporal da transação $t_{uv}$ estiver estritamente contido no intervalo de tempo $T$, e $0$ caso contrário, e $N^-(v_i)$ denota o conjunto de vizinhos de entrada diretos do vértice $v_i$.


\section{Resiliência em Hardware Periférico e o Sistema Kolka}

    Para garantir a auditabilidade, integridade dos registros e descentralização do processamento em ambientes corporativos ou remotos, o AIMS AUDIT integra um ecossistema de validação distribuída em microcontroladores de baixo custo (tais como ESP8266, ESP32 e arquiteturas baseadas em microprocessadores embarcados).

\subsection{Adoção do SHA-1 e Proteção Anti-Greed}

    Diferente do consumo massivo de memória e energia exigido pelo algoritmo SHA-256 no protocolo Bitcoin, a arquitetura periférica do AIMS AUDIT utiliza uma implementação otimizada do algoritmo SHA-1 (\textit{Secure Hash Algorithm 1}). A escolha do SHA-1 em hardware restrito deve-se à reduzida ocupação de memória RAM e ao baixo custo de instrução por ciclo de clock, permitindo execuções eficientes em chips de baixo custo.

Para evitar que participantes maliciosos introduzam hardware de altíssimo desempenho (como GPUs dedicadas ou ASICs) para monopolizar a rede de validação, o ecossistema utiliza o controlador dinâmico do Sistema Kolka. O Sistema Kolka aplica um fator de penalização não-linear ajustado ao poder de processamento medido $p$:

\begin{equation}
\text{Dificuldade}(p) = \begin{cases} 
D_{base}, & \text{se } p \le p_{target} \\[0.5em]
D_{base} \cdot \left(\dfrac{p}{p_{target}}\right)^\gamma, & \text{se } p > p_{target}
\end{cases}
\end{equation}

onde $p$ representa a capacidade computacional instantânea do nó de verificação, $p_{target}$ denota o limiar ideal de processamento de um microcontrolador padrão, e $\gamma > 1$ representa o expoente de penalização não-linear, inviabilizando economicamente o ataque de centralização por poder computacional bruto na rede de auditoria.

---

\section{Especificação Matemática do Algoritmo SHA-1}

    Nesta seção, apresenta-se a decomposição algébrica e estrutural completa do algoritmo SHA-1, utilizado como mecanismo de prova de trabalho leve no nó periférico do AIMS AUDIT.

    O SHA-1 processa mensagens de comprimento inferior a $2^{64}$ bits, gerando um resumo (\textit{digest}) fixo de $160$ bits ($5$ palavras de $32$ bits).

\subsection{Passo 1: Pré-processamento e Preenchimento (Padding)}

A mensagem original $M$ é formatada para garantir que o seu tamanho final em bits seja um múltiplo exato de **$512$ bits**.

\begin{enumerate}
    \item \textbf{Adição do Bit de Terminação:} Insere-se o bit \texttt{'1'} imediatamente após o último bit da mensagem original $M$.
    \item \textbf{Preenchimento com Zeros (Zero Padding):} Acrescentam-se $k$ bits \texttt{'0'}, onde $k$ é a menor solução não-negativa da congruência modular:
    \begin{equation}
    (|M| + 1 + k) \equiv 448 \pmod{512}
    \end{equation}
    \item \textbf{Inclusão do Comprimento Original:} Nos $64$ bits finais, codifica-se o valor $|M|$ em formato binário \textit{big-endian}.
\end{enumerate}

Após o preenchimento, a mensagem é dividida em blocos de $512$ bits. Cada bloco é fracionado em $16$ palavras de $32$ bits, denotadas por $W_0, W_1, \dots, W_{15}$.

\subsection{Passo 2: Expansão da Mensagem (Message Schedule)}

Para alimentar as $80$ rondas de compressão, as $16$ palavras iniciais são expandidas para $80$ palavras ($W_0$ a $W_{79}$) pela seguinte relação de recorrência:

\begin{equation}
W_t = \left( W_{t-3} \oplus W_{t-8} \oplus W_{t-14} \oplus W_{t-16} \right) \lll 1, \quad \text{para } 16 \le t \le 79
\end{equation}

onde $\oplus$ denota o operador lógico OU Exclusivo (\textit{XOR}) bit a bit e $\lll 1$ representa a rotação circular à esquerda por $1$ bit:
\begin{equation}
X \lll n = (X \ll n) \lor (X \gg (32 - n))
\end{equation}



\section{O Algoritmo AIMS AUDIT na Auditoria  On-Chain (Forense e de Transações)}

O algoritmo fundamental para verificar se um estado ou transação faz parte de um bloco auditado sem precisar baixar toda a cadeia é baseado em \textbf{Árvores de Merkle (Merkle Trees)} combinado com funções de hash criptográfico e curvas elípticas para assinaturas digitais.

\subsection*{Passo a Passo Algorítmico (Representação Formal):}
\begin{enumerate}
    \item \textbf{Entrada:} Um conjunto de $n$ transações ou logs de auditoria $T = \{t_1, t_2, \dots, t_n\}$.
    \item \textbf{Função Hash Criptográfica:} Seja $H: \{0,1\}^* \to \{0,1\}^{256}$ uma função altamente resistente a colisões (como SHA-256 ou Keccak-256).
    \item \textbf{Criação das Folhas (Leaves):} Cada transação é convertida em um hash inicial:
    \[ L_i = H(t_i) \quad \text{para } i = 1, 2, \dots, n \]
    \item \textbf{Construção Recursiva da Árvore:} Os nós pais são gerados concatenando e aplicando o hash dos nós filhos adjacentes:
    \[ N_{parent} = H(N_{left} \parallel N_{right}) \]
    Se o número de nós em um nível for ímpar, o último nó é duplicado ou propagado.
    \item \textbf{Raiz de Merkle (Merkle Root):} O processo repete-se até restar apenas um único nó no topo ($R$), que representa a impressão digital criptográfica de todo o estado auditado.
\end{enumerate}

\section{O Algoritmo AIMS AUDIT nas funções de Hash Criptografico}

Para entender a robustez duma auditoria baseada em blockchain, precisamos olhar para os três pilares matemáticos que sustentam sua segurança:

\subsection{A. Funções Hash Criptográficas e Efeito Avalanche}
As funções hash aplicam operações algébricas complexas (como rotações de bits, somas modulares e operações lógicas bit a bit XOR, AND, OR) sobre blocos de dados.
\begin{itemize}
    \item \textbf{Propriedade Matemática:} O \textit{Efeito Avalanche} garante que se um único bit de uma auditoria ou contrato inteligente for alterado ($t_i \to t_i'$), o resultado do hash muda de forma completamente imprevisível e estatisticamente aleatória:
    \[ H(t_i) \neq H(t_i') \]
    Isso torna qualquer adulteração de dados imediatamente detectável pela raiz de Merkle.
\end{itemize}

\subsection{B. Provas de Inclusão de Merkle (Merkle Proofs)}
Para que uma auditoria verifique se uma transação específica $t_k$ é legítima sem expor ou processar a cadeia inteira, utiliza-se a matemática de caminhos em árvores binárias.
\begin{itemize}
    \item O algoritmo gera um vetor de autenticação (caminho de prova) $P_k = \{h_1, h_2, \dots, h_m\}$, contendo os hashes irmãos necessários para reconstruir o caminho até a Raiz $R$.
    \item O verificador computa iterativamente:
    \[ R' = H(\dots H(H(L_k \parallel h_1) \parallel h_2) \dots) \]
    \item Se $R' = R$, a prova é validada matematicamente, garantindo integridade absoluta com complexidade de tempo logarítmica $\mathcal{O}(\log n)$.
\end{itemize}

\subsection{C. Assinaturas Digitais baseadas em Curvas Elípticas (ECDSA / EdDSA)}
Para autenticar os relatórios de auditoria e garantir irretratabilidade, a plataforma utiliza criptografia de curvas elípticas.
\begin{itemize}
    \item A equação geral da curva utilizada em redes compatíveis é da forma Weierstrass:
    \[ y^2 = x^3 + ax + b \pmod p \]
    \item \textbf{Funcionamento:} O auditor gera uma chave privada $d$ (um escalar grande) e calcula a chave pública $Q$ através da multiplicação de pontos na curva:
    \[ Q = d \cdot G \]
    Onde $G$ é um ponto gerador padrão. Devido à \textit{Dificuldade do Logaritmo Discreto em Curvas Elípticas (ECDLP)}, é computacionalmente inviável deduzir a chave privada $d$ conhecendo apenas a chave pública $Q$ e o ponto gerador $G$, garantindo a autenticidade jurídica e técnica da auditoria.
\end{itemize}

\section{Mecânica Criptográfica do DUCO-S1}
Em sistemas tradicionais de Prova de Trabalho (como o Bitcoin), os nós buscam $nonces$ $n \in \mathbb{N}$ para satisfazer uma condição de limiar sobre uma função hash criptográfica $H: \{0,1\}^* \to \{0,1\}^k$.

Seja $H$ a função hash criptográfica SHA-1 com saída de 160 bits. A desigualdade de alvo tradicional é expressa como:
\begin{equation}
H(B \parallel n) \le \frac{T_{\max}}{D}
\end{equation}
onde $B \in \{0,1\}^*$ representa o cabeçalho do bloco, $n$ é o candidato a nonce, $\parallel$ denota concatenação de strings, $T_{\max} = 2^{160}-1$, e $D \in \mathbb{R}^+$ é a dificuldade dinâmica da rede.

No algoritmo DUCO-S1, o problema computacional é adaptado para operar sequencialmente sobre strings de texto. Dada uma hash base $h_{\text{anterior}}$, uma hash esperada $h_{\text{esperada}}$, e uma dificuldade $D$, o minerador busca uma chave inteira sequencial $k \in \{0, 1, \dots, 100 \cdot D\}$ tal que:
\begin{equation}
H(h_{\text{anterior}} \parallel k) = h_{\text{esperada}}
\end{equation}
Esta formulação restringe otimizações de busca paralela em larga escala, transformando o desafio em um problema de busca linear sequencial com complexidade temporal $\mathcal{O}(N)$, limitado primariamente pela taxa de clock do processador e não pela largura de banda de memória.

\section{O Sistema Kolka: Otimização de Recompensa }
A principal inovação do Duino-Coin é o algoritmo Kolka, que previne que dispositivos especializados (GPUs, ASICs ou CPUs de alta performance) dominem a distribuição de recompensas.

Seja $P \in \mathbb{R}^+$ a potência de processamento de um nó medido em Hashes por Segundo ($\text{H/s}$), e $N \in \mathbb{N}_{\ge 1}$ o número total de dispositivos ativos vinculados à mesma conta.

Modelamos a taxa de recompensa líquida $R(P, N)$ por meio de uma função de utilidade multivariável restrita:
\begin{equation}
R(P, N) = \left( \frac{R_0 \cdot P^\alpha}{1 + \beta \cdot P^\gamma} \right) \cdot \left( \frac{1}{1 + \lambda \cdot (N - 1)^\delta} \right)
\end{equation}
onde $R_0, \alpha, \beta, \gamma, \lambda, \delta \in \mathbb{R}^+$ são constantes de ajuste da rede.

\subsection{Análise de Comportamento Assintótico}
1. \textbf{Regime de Baixa Potência ($P \to 0$):} Para microcontroladores onde $P \approx 10^2\,\text{H/s}$, o termo $\beta \cdot P^\gamma \ll 1$. Consequentemente, a função reduz-se a:
\begin{equation}
R(P) \approx R_0 \cdot P^\alpha
\end{equation}
proporcionando um retorno quase linear e proporcional à frequência de operação do microcontrolador.

2. \textbf{Regime de Alta Potência ($P \to \infty$):} Para nós de alto desempenho onde $P \ge 10^6\,\text{H/s}$, assumindo $\gamma > \alpha$, o denominador passa a dominar o cálculo:
\begin{equation}
\lim_{P \to \infty} R(P) = \lim_{P \to \infty} \frac{R_0 \cdot P^\alpha}{\beta \cdot P^\gamma} = 0
\end{equation}
A taxa de retorno marginal $\frac{\partial R}{\partial P}$ torna-se negativa ou próxima de zero após um limiar crítico $P^*$, penalizando a utilização de hardware potente.

3. \textbf{Penalidade Anti-Fazenda ($N > 1$):} O segundo fator impõe uma redução estritamente decrescente em relação à concentração de nós por conta:
\begin{equation}
\frac{\partial R}{\partial N} < 0, \quad \forall N > 1
\end{equation}
diminuindo os ganhos marginais para cada dispositivo adicional conectado à mesma entidade.


\section{Wrapping Multichain e Conservação de Invariantes}
Para interagir com o ecossistema de Finanças Descentralizadas (DeFi), as moedas nativas ($DUCO_{\text{nativo}}$) são mapeadas para tokens de contratos inteligentes ($wDUCO$) em blockchains externas (ex: Tron, BSC, Polygon).

Seja $S_{\text{nativo}}(t)$ o suprimento total de moedas retidas na custódia central da ponte, e $S_{\text{wrapped}}(t)$ o suprimento total de tokens emitidos em redes externas. A ponte mantém um invariante de reserva na proporção 1:1:
\begin{equation}
S_{\text{nativo}}(t) - S_{\text{wrapped}}(t) = 0, \quad \forall t
\end{equation}

Quando a operação de empacotamento é executada, o mapeamento $f: DUCO_{\text{nativo}} \to wDUCO$ garante atualizações atômicas de estado:
\begin{equation}
\Delta S_{\text{nativo}}^{\text{custódia}} + \Delta S_{\text{wrapped}}^{\text{emitido}} = 0
\end{equation}
garantindo que o valor em circulação permaneça constante em todo o ecossistema multi-rede.O protocolo Duino-Coin demonstra uma implementação alternativa de Prova de Trabalho. Ao empregar o algoritmo DUCO-S1, aplicar funções não-lineares de penalização através do Sistema Kolka e utilizar gerenciamento de estado via Hashchain centralizada, o ecossistema otimiza com sucesso a acessibilidade de hardware e a utilidade educacional.



\section{Algoritmo TIADMHA AIMS AUDIT}

O algoritmo TIADMHA avalia a integridade do nó minerador mapeando o espaço vetorial de telemetria física do hardware. Seja o vetor de estado em um instante $t$:
$$S(t) = \begin{bmatrix} V_{cc}(t) \\ T(t) \\ H_{total}(t) \end{bmatrix}$$
Onde $V_{cc}$ representa a tensão de alimentação, $T$ a temperatura interna estimada do chip ESP32, e $H_{total}$ a taxa de hash agregada da carteira.
\begin{figure}
    \centering
    \includegraphics[width=1\linewidth]{image19.png}
    \caption{ALGORITMO TIADMHA }
    \label{fig:placeholder}
\end{figure}
\subsection{Condição de Anomalia e \textit{Spoofing}}
A função indicadora de \textit{spoofing} $\mathbb{I}_{spoof}(t)$ é modelada por restrições lógicas e estatísticas não-lineares. O sistema detecta falsificação de hardware quando a tensão excede os limites nominais de operação do silício ou quando há incompatibilidade termodinâmica entre o poder de processamento reportado e a dissipação térmica real:

$$\mathbb{I}_{spoof}(t) = \begin{cases} 
1, & \text{se } V_{cc}(t) \notin [V_{min}, V_{max}] \lor \left( H_{total}(t) > \tau_h \land T(t) < \tau_t \right) \\
0, & \text{caso contrário}
\end{cases}$$

\section{Referências}
\begin{figure}
    \centering
    \includegraphics[width=1\linewidth]{}
\begin{figure}
        \centering
        \includegraphics[width=1\linewidth]{tiadhma.png}
        \caption{AlGORITMO TIADMHA AIMS AUDIT}
        \label{fig:placeholder}
    \end{figure}
      
Onde os limiares empíricos adotados no firmware são:

\begin{figure}
            \centering
            \includegraphics[width=0.5\linewidth]{TIADHMA2.png}
            \caption{ANALISADOR DE SPOOFING REDE SHA-1 ALGORITMO TIADMHA}
            \label{fig:placeholder}
        \end{figure}
    

\begin{figure}
    \centering
    \includegraphics[width=1\linewidth]{image7.png}
    \caption{ALGORITMO DE SONIFICAÇÃO E ANALISE DE FFT UTILIZANDO CALCULO DO BORDO TEOREMA DE STOKE E FUNDAMENTOS ALGORITMO TIADHMA }
    \label{fig:placeholder}
\end{figure}
\begin{figure}
    \centering
    \includegraphics[width=1\linewidth]{image9.png}
    \caption{ANALISE DE FIRMWARE UTILIZANDO ESTRUTURA ALGORITMO TIADMHA ANALISE CODIGO PARTE 1  }
    \label{fig:placeholder}
\end{figure}
\begin{figure}
    \centering
    \includegraphics[width=1\linewidth]{image10.png}
    \caption{ANALISE DE FIRMWARE UTILIZANDO ESTRUTURA ALGORITMO TIADMHA ANALISE CODIGO PARTE 2}
    \label{fig:placeholder}
\end{figure}

\begin{figure}
    \centering
    \includegraphics[width=1\linewidth]{image11.png}
    \caption{ANALISE DE FIRMWARE UTILIZANDO ESTRUTURA ALGORITMO TIADMHA ANALISE DO CODIGO PARTE 3}
    \label{fig:placeholder}
\end{figure}
\begin{figure}
    \centering
    \includegraphics[width=1\linewidth]{image12.png}
    \caption{ANALISE DE FIRMWARE UTILIZANDO ESTRUTURA ALGORITMO TIADMHA ANALISE DO CODIGO PARTE4}
    \label{fig:placeholder}
\end{figure}

\begin{figure}
    \centering
    \includegraphics[width=1\linewidth]{image13.png}
    \caption{ANALISE DE FIRMWARE UTLIZANDO ESTRUTURA ALGORITMO TIADMHA ANALISE DO CODIGO PARTE 5}
    \label{fig:placeholder}
\end{figure}
\begin{figure}
    \centering
    \includegraphics[width=1\linewidth]{image14.png}
    \caption{ANALISE DE FIRMWARE UTILIZANDO ESTRUTURA ALGORITMO TIADMHA DO CODIGO PARTE 6 }
    \label{fig:placeholder}
\end{figure}

\begin{figure}
    \centering
    \includegraphics[width=1\linewidth]{image18.png}
    \caption{ANALISE DE FIRMWARE UTILIZANDO ESTRUTURA ALGORITMO TIADMHA DO CODIGO PARTE 7 }
    \label{fig:placeholder}
\end{figure}
* $V_{min} = 3.08\,\text{V}$ e $V_{max} = 3.42\,\text{V}$ (tolerância de $\pm 3.6\%$ sobre a linha de $3.3\,\text{V}$).
* $\tau_h = 500.0\,\text{kH/s}$ (limite crítico de hashrate).
* $\tau_t = 36.0\,^{\circ}\text{C}$ (temperatura mínima esperada sob alta carga).
\section{Referências}
\begin{figure}
    \centering
    \includegraphics[width=0.25\linewidth]{image.png}
    \caption{TRABALHO CONCLUSÃO  DE CURSO AUDIOVISUAL AIMS AUDIT}
    \label{fig:placeholder}
\end{figure}
}
    \label{fig:placeholder}
\end{figure}
    
\begin{thebibliography}{99}

\bibitem{iso42001}
INTERNATIONAL ORGANIZATION FOR STANDARDIZATION. \textbf{ISO/IEC 42001: Artificial intelligence — Management system}. Genebra: ISO, 2023.

\bibitem{forbes_risks}
FORBES. \textbf{Os 15 maiores riscos da inteligência artificial}. Disponível em: \url{https://forbes.com.br/forbes-tech/2023/06/os-15-maiores-riscos-da-inteligencia-artificial/}. Acesso em: 2026.

\bibitem{godel31}
GÖDEL, Kurt. Über formal unentscheidbare Sätze der Principia Mathematica und verwandter Systeme, I. \textbf{Monatshefte für Mathematik und Physik}, v. 38, n. 1, p. 173-198, 1931.

\bibitem{turing36}
TURING, Alan Mathison. On Computable Numbers, with an Application to the Entscheidungsproblem. \textbf{Proceedings of the London Mathematical Society}, v. 42, p. 230-265, 1936.

\bibitem{turing1950}
TURING, Alan Mathison. Computing Machinery and Intelligence. \textbf{Mind}, v. 59, n. 236, p. 433-460, 1950.

\bibitem{paz_percepcoes_2026}
PAZ, Alan Aparecido da Silva. \textbf{TEORIA DAS PERCEPÇÕES: Teoria da Percepção: Formatação Algébrica em Espaços de Hilbert, Mapeamento Cross-Modal e Colapso Espectral na Deuteranopia}. Even3 Publicações, 2 out. 2026. DOI: \url{https://doi.org/10.29327/7957889}.

\bibitem{paz_tratado_2026}
PAZ, Alan Aparecido da Silva. \textbf{Tratado sobre a Indexação Algébrica de Sistemas Diatônicos via Matrizes Helicoidais Assimétricas}. Even3 Publicações, 2 set. 2026. DOI: \url{https://doi.org/10.29327/7928033}.

\bibitem{paz_tcc_2026}
PAZ, Alan Aparecido da Silva et al. \textbf{Sistema AIMS AUDIT: Auditoria de IA e Gestão de Conformidade ISO/IEC 42001 em Ecossistemas Críticos}. Trabalho de Conclusão de Curso (Graduação em Engenharia de Computação) -- Universidade Virtual do Estado de São Paulo (UNIVESP), Itapevi, 2026.

\bibitem{cantor1874}
CANTOR, Georg. Über eine Eigenschaft des Inbegriffes aller reellen algebraischen Zahlen. \textbf{Journal für die reine und angewandte Mathematik}, v. 77, p. 258-262, 1874.

\bibitem{zermelo1908}
ZERMELO, Ernst. Untersuchungen über die Grundlagen der Mengenlehre I. \textbf{Mathematische Annalen}, v. 65, n. 2, p. 261-281, 1908.

\bibitem{mccarthy1955}
MCCARTHY, John et al. \textbf{A Proposal for the Dartmouth Summer Research Project on Artificial Intelligence}. Hanover: Dartmouth College, 1955.

\bibitem{minsky1969}
MINSKY, Marvin; PAPERT, Seymour A. \textbf{Perceptrons: An Introduction to Computational Geometry}. Cambridge: MIT Press, 1969.

\bibitem{russell2020}
RUSSELL, Stuart; NORVIG, Peter. \textbf{Inteligência Artificial: uma abordagem moderna}. 4. ed. Rio de Janeiro: GEN LTC, 2022.

\bibitem{goodfellow2016}
GOODFELLOW, Ian; BENGIO, Yoshua; COURVILLE, Aaron. \textbf{Deep Learning}. Cambridge: MIT Press, 2016.

\bibitem{shoeybi2019nvidia}
SHOEYBI, Mohammad et al. Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism. \textbf{arXiv preprint arXiv:1909.08053}, 2019.

\bibitem{nvidia_nemo_2023}
NVIDIA. \textbf{NVIDIA NeMo Framework: End-to-End Cloud-Native Enterprise AI Framework for Building Custom Generative AI Models}. Santa Clara: NVIDIA Corporation, 2023.

\bibitem{vaswani2017}
VASWANI, Ashish et al. Attention is All You Need. \textbf{Advances in Neural Information Processing Systems (NeurIPS)}, v. 30, p. 5998-6008, 2017.

\bibitem{kingma2014adam}
KINGMA, Diederik P.; BA, Jimmy. Adam: A Method for Stochastic Optimization. \textbf{arXiv preprint arXiv:1412.6980}, 2014.

\bibitem{ouyang2022instructgpt}
OUYANG, Long et al. Training language models to follow instructions with human feedback (RLHF). \textbf{Advances in Neural Information Processing Systems (NeurIPS)}, v. 35, p. 27730-27744, 2022.

\bibitem{bai2022constitutional}
BAI, Yuntao et al. Constitutional AI: Harmlessness from AI Feedback. \textbf{arXiv preprint arXiv:2212.08073}, 2022.

\bibitem{kirchenbauer2023watermark}
KIRCHENBAUER, John et al. A Watermark for Large Language Models. In: \textbf{International Conference on Machine Learning (ICML)}, PMLR, p. 17061-17084, 2023.

\bibitem{ieee7000}
IEEE. \textbf{IEEE Standard 7000-2021: Model Process for Addressing Ethical Concerns during System Design}. Piscataway: IEEE, 2021.

\bibitem{eu_ai_act}
EUROPEAN PARLIAMENT. \textbf{Artificial Intelligence Act: Regulation laying down harmonised rules on artificial intelligence}. Bruxelas: União Europeia, 2024.

\bibitem{barocas2019}
BAROCAS, Solon; HARDT, Moritz; NARAYANAN, Arvind. \textbf{Fairness and Machine Learning: Limitations and Opportunities}. Cambridge: MIT Press, 2023.

\bibitem{floridi2018}
FLORIDI, Luciano et al. AI4People—An Ethical Framework for a Good AI Society: Opportunities, Risks, Principles, and Recommendations. \textbf{Minds and Machines}, v. 28, n. 4, p. 689-707, 2018.

\bibitem{ashby1956}
ASHBY, W. Ross. \textbf{An Introduction to Cybernetics}. Londres: Chapman \& Hall, 1956.

\end{thebibliography}


\end{document}


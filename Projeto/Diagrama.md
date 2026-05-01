### Fluxograma do Sistema

```mermaid
graph TD
    START([Início]) --> A[Usuário acessa o site]
    A --> B[Página Inicial: Explicação sobre o impacto das telas]
    B --> MENU[Menu Principal]

    MENU --> OP1[1. Casos Reais]
    OP1 --> R1[Exibir relatos reais]
    R1 --> MENU

    MENU --> OP2[2. Impactos no Cérebro]
    OP2 --> R2[Exibir explicação técnica]
    R2 --> MENU

    MENU --> OP3[3. Como Reduzir o Uso]
    OP3 --> R3[Exibir passo a passo]
    R3 --> MENU

    MENU --> OP4[4. Atividades por Idade]
    OP4 --> INPUT[Usuário informa a idade da criança]
    INPUT --> DEC{Faixa Etária?}

    DEC -- 0 a 2 anos --> F1[Mostrar atividades sensoriais]
    DEC -- 3 a 5 anos --> F2[Mostrar brincadeiras criativas]
    DEC -- 6 a 10 anos --> F3[Mostrar atividades físicas e sociais]
    DEC -- 11 a 14 anos --> F4[Mostrar atividades educativas e hobbies]

    F1 & F2 & F3 & F4 --> SUG[Exibir Sugestões]
    SUG --> MENU

    MENU --> END([Final: Sair ou Continuar Navegando])

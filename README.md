# [cite_start]Terminal de Suporte Proativo - Diagnóstico de Rede [cite: 13]

[cite_start]Este projeto é um protótipo funcional de um console de diagnóstico de rede, desenvolvido em **C# (.NET Console)**[cite: 8]. [cite_start]Ele foi criado para substituir sistemas arcaicos por uma interface moderna, focada em **Acessibilidade**, **Prevenção de Erros** e **UX**[cite: 15, 18, 23].

## [cite_start]👥 Equipe [cite: 6]
* **ICARO FERREIRA DE OLIVEIRA**
* **KAIO ROBERTT MORREIRA ABREU**

---

## 🧠 Heurísticas de Nielsen Implementadas

[cite_start]O desenvolvimento seguiu rigorosamente os requisitos da missão propostos no cenário de TI[cite: 15, 19]:

### [cite_start]1. Prevenção de Erros (Heurística #5) [cite: 20]
Para evitar ações catastróficas por erro de digitação, o sistema protege operações críticas:
* [cite_start]**Confirmação Extra:** Antes de executar o comando `RESET`, o sistema entra em modo de alerta e exige uma confirmação clara ($S/N$) do técnico[cite: 20, 32].
* **Validação de IP:** O comando `PING` valida a entrada de dados. [cite_start]Se o usuário digitar caracteres inválidos, o sistema sugere o formato correto: `XXX.XXX.XXX.XXX`[cite: 31].

### [cite_start]2. Reconhecimento em vez de Recordação (Heurística #6) [cite: 21]
[cite_start]O técnico não precisa memorizar comandos extensos ou complexos[cite: 16]:
* [cite_start]**Menu Fixo:** A tela principal exibe permanentemente um "Menu de Comandos Rápidos", permitindo que o usuário identifique as opções visualmente[cite: 21].

### [cite_start]3. Ajuda e Documentação (Heurística #10) [cite: 26]
[cite_start]Implementação do comando `HELP`[cite: 26]:
* [cite_start]**Documentação Contextual:** Oferece uma explicação breve de cada função (Ping, Reset e Sair) sem que o técnico precise sair da tela de operação atual[cite: 27].

---

## [cite_start]🎨 Critérios de Avaliação de UX [cite: 33]

* [cite_start]**Gestão de Cores:** Uso estratégico para reduzir o tempo de reação e indicar estados[cite: 34, 40]:
    * [cite_start]**Verde:** Sucesso e operações finalizadas[cite: 34].
    * [cite_start]**Amarelo/Vermelho:** Estados de atenção e perigo em comandos críticos[cite: 32, 34].
* [cite_start]**UX Writing:** Mensagens instrutivas e claras que guiam o usuário, abandonando o padrão rude de apenas dizer "Command Error"[cite: 17, 34].
* [cite_start]**Resiliência:** O programa foi desenvolvido para sobreviver a entradas de dados inesperadas, como letras em campos onde se esperam números ou IPs[cite: 34].

---

## 🚀 Instruções de Execução

1. [cite_start]Certifique-se de ter o ambiente .NET configurado[cite: 8].
2. Compile e execute a aplicação:
   ```bash
   dotnet run
   ```

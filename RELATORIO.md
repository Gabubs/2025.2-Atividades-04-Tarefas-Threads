# Relatório de Observações - Atividade de Threads

## Informações do Aluno
- **Nome:** _Gabriel Gomes Santos_
- **Matrícula:** _202042014040022_
- **Data:** _08/11/2025_

## Ambiente de Execução

- [ ] Executado localmente
- [x] Executado em Docker/Fedora

**Sistema Operacional:** _Windows_  
**Processador:** _Intel core de 8_  
**Número de Cores:** _Não lembro_

---

## Execução 1

### Resultados Observados

**Thread CPU (Thread 1):**
- Tempo de execução: _0.28_ segundos
- Soma dos primos: _37550402023_
- Ordem de conclusão: _3°_ (1ª, 2ª ou 3ª)

**Thread I/O (Thread 2):**
- Tempo de execução: _0.02_ segundos
- Linhas processadas: _10000_
- Ordem de conclusão: _2°_ (1ª, 2ª ou 3ª)

**Thread Mista (Thread 3):**
- Tempo de execução: _0.02_ segundos
- Total de cálculos: _3482527859448382464_
- Ordem de conclusão: _1°_ (1ª, 2ª ou 3ª)

**Tempo Total do Programa:** _0.32_ segundos

### Observações sobre a Saída

Descreva como as mensagens das threads apareceram no console:

_[Ex: As mensagens das três threads apareceram em ordem, mostrando que estavam executando em tempos diferentes]_

---

## Execução 2 (Repetir para comparação)

### Resultados Observados

**Thread CPU (Thread 1):**
- Tempo de execução: _0.29_ segundos
- Ordem de conclusão: _3°_ (1ª, 2ª ou 3ª)

**Thread I/O (Thread 2):**
- Tempo de execução: _0.01_ segundos
- Ordem de conclusão: _1°_ (1ª, 2ª ou 3ª)

**Thread Mista (Thread 3):**
- Tempo de execução: _0.02_ segundos
- Ordem de conclusão: _2°_ (1ª, 2ª ou 3ª)

**Tempo Total do Programa:** _0.32_ segundos

### Diferenças entre Execuções

_[A segunda foi mais rapida e dessa vez foi executada em 1° da ordem ordem(Anteriormente em 2°), já a primeira foi 0.01 segundo(s) mais lenta]_

---

## Análise e Conclusões

### 1. Qual thread terminou primeiro? Por quê?

_[Operações de I/O por ser a mais curta]_

### 2. Por que os tempos de execução variam entre diferentes execuções?

_[imagino que seja por: interações com outros processos e multiplos outros fatores]_

### 3. Como o sistema operacional gerencia a execução das threads?

_[O Escalonador decide qual thread executará em um determinado momento. Ele Alterna rapidamente entre elas(as threads)]_

### 4. Qual seria o impacto de aumentar o número de threads?

_[Aumentar o número de threads pode melhorar o desempenho ao permitir que várias tarefas sejam executadas ao mesmo tempo, aproveitando melhor os núcleos do processador. Porem, se o numero de threads for muito grande, o sistema gasta mais tempo gerenciando elas do que executando o trabalho, o que pode reduzir a eficiência.]_

### 5. O que aconteceria se executássemos as mesmas operações sequencialmente?

_[Se as operações fossem executadas sequencialmente, elas seriam realizadas uma de cada vez, sem aproveitar o paralelismo. Isso tornaria o processo mais lento, pois apenas um núcleo do processador trabalharia por vez. Na execução paralela, várias operações ocorrem simultaneamente, reduzindo o tempo total de execução.]_

---

## Experimentos Adicionais (Opcional)

### Modificação 1: Aumentar NUM_ITERACOES

**Alteração realizada:** _[Ex: Mudei NUM_ITERACOES de 1000000 para 5000000]_

**Resultado observado:**
- Tempo da Thread CPU: _______ segundos
- Impacto no tempo total: _______

**Conclusão:** _[O que você aprendeu com essa modificação?]_

### Modificação 2: Adicionar mais threads

**Alteração realizada:** _[Ex: Criei 3 threads CPU adicionais]_

**Resultado observado:**
- Comportamento: _______
- Impacto na performance: _______

**Conclusão:** _[O que você aprendeu com essa modificação?]_

---

## Conceitos Aprendidos

Liste os principais conceitos de sistemas operacionais que você compreendeu melhor com esta atividade:

1. _no paralelismo, elas realmente ocorrem ao mesmo tempo, aproveitando múltiplos núcleos do processador._
2. _na concorrência, várias tarefas progridem alternadamente_
(foi isso que eu entedi)
---

## Dificuldades Encontradas

Descreva quaisquer problemas que enfrentou durante a atividade e como os resolveu:

_[Sua resposta aqui]_

---

## Comentários Finais

_[Espaço para observações adicionais, sugestões ou comentários sobre a atividade]_

---

**Data de Conclusão:** _[Data]_  
**Assinatura:** _[Seu nome]_

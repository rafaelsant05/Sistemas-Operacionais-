# Sistemas-Operacionais-

# Atividade – SoSim 

 1) Gerenciador de Processos
- Criados 5 processos com tempos diferentes.  
- Estados observados: Novo, Pronto, Executando, Bloqueado, Finalizado.  
- Troca de contexto ocorre quando um processo termina e outro inicia.  
- Pronto → Executando: o escalonador seleciona o processo e a CPU começa a rodá-lo.  


 2) Escalonador de Processos
- Algoritmos testados: FIFO, Round Robin (q=3), SJF.  
- Tempos médios de espera:  
  - FIFO ≈ 7,2  
  - Round Robin (q=3) ≈ 9,2  
  - SJF ≈ 6,0  
- Melhor resultado: SJF.  

Quantum no Round Robin:  
- Pequeno → muitas trocas de contexto, sistema mais lento.  
- Grande → comportamento parecido com FIFO.  
- Equilibrado → melhora desempenho e justiça entre processos.  



 3) Paginação
- Processo maior que a RAM exigiu paginação.  
- Algumas páginas ficaram fora, gerando 9 faltas de página.  

Falta de página: ocorre quando uma página não está na RAM; o SO pausa, traz do disco e retoma a execução.  

Comparação:  
- Com paginação → permite rodar processos maiores e melhora a multiprogramação.  
- Sem paginação → processo só roda se couber inteiro na RAM.  

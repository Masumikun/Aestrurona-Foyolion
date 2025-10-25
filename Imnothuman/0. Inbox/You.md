---
date created: Saturday, 25th ✦ Oct┆2025 ➣ 17▫43▫48 
date modified: Saturday, 25th ✦ Oct┆2025 ➣ 17▫43▫48 
---
## You
**Função** ➣ Você possui 5⚡ como de costume
**Consumo** ➣ [[árvore]], [[poção]] e [[vizinhos]]
**Recuperar** ➣ [[Chá de bolhas]], [[Chocolate]], [[Cigarro]] e [[Vinho]]

**Interação com:**
- [[árvore]]
	- ***Dia***
	- ❝Pareço mais vivo e realmente me sinto tanto confortável para descansar um pouco❞
	<br>
	- ***Tarde***
	- ❝Sinceramente parece um pouco desconfortante, mas não deve haver problemas❞
	<br>
	- ***Noite***
	- ❝Caramba estamos numa situação de se proteger e você quer sair?!❞
	
- [[poção]]
	- ***Dia*** (*Sem vizinhos*)
	- ❝Vamos descansar e talvez amanhã acontece algo importante.❞
	<br>
	- ***Dia*** (*Com vizinhos* e *Energia*)
	- ❝Talvez seja melhor investir tempo em investigação?❞
	- ❝Certo... vamos descansar❞ (2° tentativa)
	<br>
	- ***Tarde*** (*Sem vizinhos*)
	- ❝Apesar de se um dia tranquilo, não devo me preocupar com agora que irei fazer.*❞
	<br>
	- ***Tarde*** (*Com vizinhos*)
	- ❝Tem certeza que quer um descanso?❞
		- `if(com energia)` ❝Certamente vamos tomar, mas investigamos todos?❞
			- `if(yes)` ❝Certo... vou acreditar que podemos dormir bem...❞
			
			<br>
		- `if(sem energia)` ❝Não é nescessário, já podemos dormir mesmo assim❞
			- `if(3° tentativa)` ❝Como quiser... gaste recursos atoa❞ [^1]


[^1]: - [*] Parabéns você desmaiou no chão de sono e noite a porta ficou livre para qualquer um entra até mesmo uma anomalia

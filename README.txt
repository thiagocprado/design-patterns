Design Patterns -> Solução comum para um problema recorrente ao utilizar o paradigma da orientação a objetos

-----------------------------------------------------------------------------------------------------------------

Criação de uma solução comum para problemas recorrentes 

"Não reinventar a roda"

3 categorias: 

- criacionais: construção, craição de objetos
- estruturais: estrutura e composição entre objetos e classes
- comportamentais: métodos de estado e interação entre os objetos

Comportamentais:

- strategy: 
	- visa resolver a existência de diversos algoritmos para uma ação, resultando na possibilidade de vários ifs.

	o strategy resolve problemas relacionado a diversos if's e else's que podem surgir para fazer alguma determinada ação.
	A solução é usar do polimorfismo, utilizando interfaces ou até mesmo uma classe.

	diminuir a complexidade do nosso código, trocando múltiplas condicionais por classes:
		Esta técnica é chamada de Strategy, que é um dos padrões de projeto

- chain of responsability:
	- visa resolver problemas semelhantes ao do strategy, entretanto lida com condições de chamada, onde se uma condição não 
	for satisfeita será chamada uma nova função para tentar solucionar o problema




- template method:
	- favorece o reaproveitamento de códigos comuns entre classes, evitando assim duplicações de códigos.



- state:
	é possível que um objeto se comporte de formas diferentes, dependendo do seu estado;

	se o resultado de uma chamada de método depende do estado, podemos delegar esta ação para uma classe específica do estado atual

é possível aplicar mais de um padrão no mesmo código


- command:
	um caso de uso em nossa aplicação pode ter várias ações (salvar no banco, enviar e-mail, etc);

	um caso de uso deve ser extraído para uma classe específica, ao invés de estar no arquivo da CLI, controller ou algo do tipo

	a técnica de extração do caso de uso para uma classe específica pode ser chamada de padrão Command;

	o padrão Command da GoF para o padrão que utiliza Command Handler (muito utilizado no padrão de arquitetura Domain Driven Design).


- observer:
	deixar a implementação de todas as tarefas de um caso de uso da aplicação na mesma classe pode trazer problemas:

	Dificuldade de manutenção;
	Classes muito grandes e difíceis de ler;
	Problemas quando precisar alterar a implementação de uma das tarefas.

	é mais interessante separar cada ação em uma classe separada;







- adapter: 
	detalhes de infraestrutura devem ser abstraídos através de interfaces



- decorator:
	adicionar comportamento a classes em tempo de execução;
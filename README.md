# jornadadados_btc_aula16

# Aula 16 - 18/03 - Revisão de Programação orientada a objetos


### Objetivo
- Revisão sobre o objetivo de trabalhar com POO
- Motivação para trabalharmos com Data Classes
- Motivação para trabalharmos com Pydantic
- Motivação para trabalharmos com ORM


### Abstração

Definição: Abstração, no contexto da programação orientada a objetos, é o processo de esconder os detalhes complexos de implementação e exibir apenas as funcionalidades essenciais de um objeto ou classe. Isso permite que pessoas do seu time trabalhem em um nível mais alto de abstração, focando no que o objeto faz, em vez de como ele faz.

#### Exemplo em Python:

        class Veiculo:
            def __init__(self, tipo, cor):
                self.tipo = tipo
                self.cor = cor

            def descrever(self):
                return f"Um {self.tipo} de cor {self.cor}"

        # Usando a abstração
        carro = Veiculo("carro", "azul")
        print(carro.descrever())
    
Neste exemplo, a classe Veiculo abstrai as características e o comportamento de um veículo. O método descrever permite-nos obter uma descrição do veículo sem precisar saber detalhes específicos sobre sua implementação interna.

No Python, o método __init__ e a palavra-chave self são fundamentais para a programação orientada a objetos (POO) e desempenham um papel crucial na definição e no trabalho com classes e objetos.

### O método __init__
- Definição e Propósito: O método __init__ é um método especial, também conhecido como construtor, em classes Python. Ele é chamado automaticamente quando um novo objeto da classe é criado. O propósito principal do método __init__ é inicializar os atributos do novo objeto, configurando-o com os valores iniciais necessários ou o estado padrão.

- Sintaxe e Uso: O método __init__ é definido dentro de uma classe e pode aceitar argumentos além do self (que é obrigatório). Estes argumentos são usados para passar valores iniciais para o objeto.



        class Veiculo:
            def __init__(self, tipo, cor):
                self.tipo = tipo
                self.cor = cor


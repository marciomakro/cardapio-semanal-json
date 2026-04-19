
-----

#  Cardápio Semanal JSON

Este repositório armazena o arquivo de dados para o sistema de cardápio. O objetivo é permitir a atualização dinâmica dos pratos sem a necessidade de novos deploys na aplicação principal.

##  Como utilizar

 Caso precise realizar alterações ou restaurar o arquivo em caso de erro, utilize o modelo abaixo.


-----

## 🛠️ Modelo de Estrutura (modelo\_cardapio.json)

Abaixo está o esquema padrão.

```json
[
  {
    "id": 1,
    "dia_semana": "Segunda-feira",
    "sopa": "Minestrone",
    "salada_1": "Repolho roxo",
    "salada_2": "Feijão branco ao vinagrete",
    "prato_principal": "Proteina de soja gratinada",
    "opcao": "Ovo frito",
    "guarnicao": "Mix de legumes sauté",
    "acompanhamentos": "Arroz Branco, Arroz integral, Feijão Carioca",
    "sobremesa": "Mexerica",
    "disponivel": "sim"
  },
  {
    "id": 2,
    "dia_semana": "Terça-feira",
    "sopa": "",
    "salada_1": "Acelga",
    "salada_2": "Repolhese",
    "prato_principal": "Filé de coxa e sobrecoxa",
    "opcao": "Ovo cozido/PTS",
    "guarnicao": "Creme de milho",
    "acompanhamentos": "Arroz Branco, Arroz integral, Feijão Preto",
    "sobremesa": "Maçã",
    "disponivel": "sim"
  },
  {
    "id": 3,
    "dia_semana": "Quarta-feira",
    "sopa": "",
    "salada_1": "beterraba ralada",
    "salada_2": "Batata bolinha ao vinagrete",
    "prato_principal": "Sassame grelhado",
    "opcao": "Ovo cozido/PTS",
    "guarnicao": "Macarrão ao sugo",
    "acompanhamentos": "Arroz Branco, Arroz integral, Feijão Carioca",
    "sobremesa": "Banana",
    "disponivel": "sim"
  },
  {
    "id": 4,
    "dia_semana": "Quinta-feira",
    "sopa": "",
    "salada_1": "Mix de repolho",
    "salada_2": "Chuchu ao vinagrete",
    "prato_principal": "Carne moída rica",
    "opcao": "Ovo cozido/PTS",
    "guarnicao": "Purê de batatas",
    "acompanhamentos": "Arroz Branco, Arroz integral, Feijão Carioca",
    "sobremesa": "Laranja",
    "disponivel": "sim"
  },
  {
    "id": 5,
    "dia_semana": "Sexta-feira",
    "sopa": "",
    "salada_1": "Acelga",
    "salada_2": "Pepino sunomono",
    "prato_principal": "Figado Acebolado",
    "opcao": "Ovo cozido/PTS",
    "guarnicao": "Virado de couve",
    "acompanhamentos": "Arroz Branco, Arroz integral, Feijão Carioca",
    "sobremesa": "Maçã",
    "disponivel": "sim"
  },
  {
    "id": 6,
    "dia_semana": "Sábado",
    "sopa": "",
    "salada_1": "Repolho ao vinagrete",
    "salada_2": "",
    "prato_principal": "Cubos de frango acebolado",
    "opcao": "Ovo cozido/PTS",
    "guarnicao": "Batata sauté",
    "acompanhamentos": "Arroz Branco, Arroz integral, Feijão Carioca",
    "sobremesa": "Banana",
    "disponivel": "sim"
  },
  {
    "id": 0,
    "dia_semana": "Domingo",
    "sopa": "",
    "salada_1": "Soja ao vinagrete",
    "salada_2": "",
    "prato_principal": "Iscas de frango grelhado",
    "opcao": "Ovo cozido/PTS",
    "guarnicao": "Macarrão ao molho a parte",
    "acompanhamentos": "Arroz Branco, Arroz integral, Feijão Carioca",
    "sobremesa": "Laranja",
    "disponivel": "sim"
  }
]
```

-----

## 📝 Regras de Preenchimento

  * **Campos Vazios:** Se um item não for servido (ex: não há sopa no dia), deixe o valor como string vazia `""`. O sistema irá ocultar o campo automaticamente na interface.
  * **Campo `disponivel`:** \* `"sim"`: O cardápio é exibido normalmente.
      * `"não"`: Exibe uma mensagem de "Cardápio indisponível" para o usuário.
  

-----

⌨️ com ❤️ por [Marcio Gregorio](https://www.google.com/search?q=https://github.com/marciomakro)

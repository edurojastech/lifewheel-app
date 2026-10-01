# Roda da Vida

Aplicação web que ajuda a refletir sobre o equilíbrio entre as principais áreas da vida. A pessoa responde a um questionário, dá notas de 0 a 10 para cada afirmação e visualiza o resultado em um **gráfico de radar**, identificando quais áreas merecem mais atenção para ter uma vida mais positiva e equilibrada.

🔗 **Demo:** https://edurojastech.github.io/lifewheel-app/

> Projeto de estudo, em desenvolvimento.

## Funcionalidades

- Questionário com afirmações por área da vida, avaliadas com notas de 0 a 10
- 12 áreas avaliadas: família, relacionamento amoroso, vida social, espiritualidade, hobbies e diversão, plenitude e felicidade, contribuição social, recursos financeiros, propósito, saúde e disposição, equilíbrio emocional e desenvolvimento intelectual
- Gráfico de radar gerado a partir das notas
- Respostas salvas no navegador (`localStorage`), sem necessidade de cadastro ou servidor
- Página separada para recuperar e visualizar novamente o resultado salvo
- Layout responsivo com Bootstrap

## Tecnologias

| Tecnologia | Uso no projeto |
| --- | --- |
| HTML5 | Estrutura das páginas |
| CSS3 | Estilos personalizados (`css/custom.css`) e animações (`animate.css`) |
| JavaScript | Lógica do questionário, cálculo das notas e persistência dos dados |
| jQuery 3.3.1 | Manipulação do DOM |
| Bootstrap 4.3.1 | Layout responsivo e componentes (com Popper.js 1.14.7) |
| amCharts 3 | Gráfico de radar |
| Font Awesome | Ícones |
| Web Storage (`localStorage`) | Armazenamento local das respostas |
| GitHub Pages | Hospedagem da demo |

## Estrutura do projeto

```
lifewheel-app/
├── index.html                    # Questionário
├── recuperar_roda_vida.html      # Visualização do resultado salvo
├── css/
│   ├── custom.css
│   └── animate.css
├── js/
│   ├── roda_vida.js              # Questionário, notas e salvamento
│   ├── recuprarDados_roda_vida.js# Recuperação dos dados e gráfico
│   └── amcharts.js
└── img/
    └── barra-roda-vida.png
```

## Como executar

Não há dependências para instalar. Basta clonar e abrir no navegador:

```bash
git clone https://github.com/edurojastech/lifewheel-app.git
cd lifewheel-app
```

Abra o `index.html` no navegador ou use uma extensão como o Live Server do VS Code. É necessária conexão com a internet, pois Bootstrap, jQuery, Popper, Font Awesome e partes do amCharts são carregados por CDN.

## Próximos passos

- [ ] Remover o arquivo legado `.old_index.html`
- [ ] Revisar textos repetidos de algumas afirmações
- [ ] Permitir exportar o resultado (imagem ou PDF)
- [ ] Atualizar as bibliotecas para versões atuais

## Autor

Desenvolvido por [Eduardo Rojas](https://github.com/edurojastech).

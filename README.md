# SanCasa : estime o valor do aluguel em São Carlos

Projeto de Machine Learning para prever o valor do aluguel em São Carlos com base nas características do imóvel alugado, que são: tipo de imóvel (casa/apartamento), número de dormitórios, banheiros, garagens, suítes, mobiliado (sim/não). 

Estrutura do projeto:
<pre>
<code>
├── Aluguel_SaoCarlos_Python_Flask
│   ├── ml_model
│   │    ├── model.pkl
│   │    ├── tabela_aluguel_completa.csv
│   │    └── training.py
│   │        
│   ├── static  
│   │    ├── assets
│   │    │    ├── css
│   │    │    ├── js
│   │    │    ├── sass
│   │    │    └── webfonts
│   │    ├── images
│   │    │    ├── fulls
│   │    │    ├── thumbs
│   │    │    ├── avatar.jpg
│   │    │    └── bg.jpg
│   │    
│   ├── templates
│   │    ├── index.html
│   │    ├── LICENSE.txt
│   │    └── README.txt 
│   │        
│   ├── webscraping 
│   │    └── webscraping.ipynb        
│   │ 
├── app.py
├── README.md
└── requirements.txt
</code>
</pre>

- Em <a href="https://github.com/naomyduarteg/Aluguel_SaoCarlos_Python_Flask/tree/main/ml_model">crud</a>, está o arquivo python usado para preparar os dados e treinar o modelo de ML, que gera o arquivo model.pkl, este que será usado para prever os valores.
- Em <a href="https://github.com/naomyduarteg/Aluguel_SaoCarlos_Python_Flask/tree/main/static">data</a>, estão os arquivos que geram a aparência do site.
- Em <a href="https://github.com/naomyduarteg/Aluguel_SaoCarlos_Python_Flask/tree/main/templates">endpoints</a>, está o arquivo que define a estrutura principal do site.
- Em <a href="https://github.com/naomyduarteg/Aluguel_SaoCarlos_Python_Flask/tree/main/webscraping">routes</a>, está o arquivo em Jupiter notebook onde é realizada a raspagem de dados de aluguel.
- Em <a href="https://github.com/naomyduarteg/Aluguel_SaoCarlos_Python_Flask/blob/main/app.py">schemas</a>, está o arquivo principal da API flask que renderiza o template e executa a previsão usando o modelo ML selecionado e os dados inseridos pelo usuário.

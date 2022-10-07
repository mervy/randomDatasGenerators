# randomDatasGenerators
Sites para gerar dados randômicos

https://json-generator.com/

Abaixo uma configuração para dados de um blog
[
  '{{repeat(300, 7)}}',
  {
    id: '{{objectId()}}',
    index: '{{index(1)}}',
    guid: '{{guid()}}',
    isActive: '{{bool()}}',    
    image: 'https://picsum.photos/200/300',
    name: '{{firstName()}}',
    surname: '{{surname()}}',
    password: '{{objectId()}}',  
    email: '{{email()}}',    
    address: '{{integer(100, 999)}} {{street()}}, {{city()}}, {{state()}}, {{integer(100, 10000)}}',
    title: '{{lorem(1, "sentences")}}',
    content: '{{lorem(10, "paragraphs")}}',
    created_at: '{{date(new Date(2014, 0, 1), new Date(), "YYYY-MM-dd hh:mm:ss")}}',
    updated_at: '{{date(new Date(2014, 0, 1), new Date(), "YYYY-MM-dd hh:mm:ss")}}',    
    tags: [
      '{{repeat(7)}}',
      '{{lorem(1, "words")}}'
    ]
  }
]

https://stackoverflow.com/questions/20633310/how-to-get-random-text-from-lorem-ipsum-in-php

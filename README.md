# randomDatasGenerators
Sites para gerar dados randômicos

- https://generatedata.com/
- https://www.mockaroo.com/
- http://www.randat.com/
- https://tableconvert.com/json-to-sql
- https://json-generator.com/

Abaixo uma configuração para dados de um blog nesse último site
<pre><code>
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
</code></pre>

# Sites para gerar dados
- https://www.fotor.com/features/ai-image-generator/
- https://www.fotor.com/blog/best-ai-random-face-generators/
- https://github.com/topics/random-data-generation
- https://towardsdatascience.com/free-resources-for-generating-realistic-fake-data-da63836be1a8
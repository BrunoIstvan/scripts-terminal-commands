# terminal-commands

#grep

O grep é uma ferramenta poderosa para busca de padrões em arquivos de texto. Você pode usá-lo em conjunto com expressões regulares para encontrar padrões complexos. Por exemplo:

  # Procurar todas as linhas que contêm a palavra "exemplo" em um arquivo
  grep 'exemplo' arquivo.txt

  # Procurar todas as linhas que começam com "abc" em um arquivo
  grep '^abc' arquivo.txt
  
  # Procurar todas as linhas que terminam com "123" em um arquivo
  grep '123$' arquivo.txt
  
  # Procurar todas as linhas que contêm uma sequência de três números em um arquivo
  grep '[0-9][0-9][0-9]' arquivo.txt


#awk

O awk é uma ferramenta de processamento de texto extremamente versátil que permite operações mais complexas em arquivos. Ele também suporta expressões regulares. Por exemplo:

  # Imprimir todas as linhas que contêm a palavra "exemplo" em um arquivo
  awk '/exemplo/' arquivo.txt
  
  # Imprimir apenas o segundo campo de todas as linhas que começam com "abc"
  awk '/^abc/ { print $2 }' arquivo.txt
  
  # Substituir todas as ocorrências de "foo" por "bar" em um arquivo
  awk '{ gsub("foo", "bar"); print }' arquivo.txt
  
  
#sed
  
O sed é uma ferramenta que permite a edição de texto em fluxo. Ele é útil para substituir, excluir ou inserir texto com base em padrões de expressões regulares. Exemplos:

  # Substituir todas as ocorrências de "foo" por "bar" em um arquivo
  sed 's/foo/bar/g' arquivo.txt
  
  # Excluir todas as linhas que contêm a palavra "exemplo" em um arquivo
  sed '/exemplo/d' arquivo.txt
  
  # Imprimir apenas as linhas que começam com "abc" em um arquivo
  sed -n '/^abc/p' arquivo.txt

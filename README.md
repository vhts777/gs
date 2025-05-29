Victor Hugo Torres Saldonas

# 1 - mostra a data 
#!/bin/bash: Define o interpretador que executará o script (Bash)
$(date): executa o comando date, que retorna a data e hora atual no formato padrão
echo: exibe a mensagem com o resultado do date

# 2 - nome usuario 
echo "Usuário logado: $USER"
a variável $USER guarda o nome do usuário atualmente logado
echo "Diretório inicial: $HOME"
a variável $HOME contém o diretório inicial (home) desse usuário


# 3 - organizador
#!/bin/bash
define o interpretador Bash para o script
mkdir -p imagens e mkdir -p documentos
cria as pastas imagens/ e documentos/.
o -p evita erro se a pasta já existir
mv *.jpg *.png imagens/ 2>/dev/null
move todos os arquivos .jpg e .png para a pasta imagens/.
o 2>/dev/null evita mensagens de erro caso não existam arquivos com essas extensões
mv *.pdf *.txt documentos/ 2>/dev/null
faz o mesmo com .pdf e .txt, movendo para documentos/.

# 4 - • echo -n "Digite seu nome: "
o -n faz com que o cursor fique na mesma linha ao pedir o nome
read nome
o comando read espera o usuário digitar algo e armazena isso na variável nome
echo "Bem-vindo, $nome!"
exibe uma mensagem personalizada usando a variável que o usuário digitou

Este diretório contém exercícios e soluções para um curso prático de
curso prático de OpenMP.  Informações sobre esses programas podem ser encontradas
nos comentários e nos slides do curso.

Para usar esses programas, copie o arquivo "def" apropriado para
"make.def".  Por exemplo, em um sistema linux rodando os compiladores gnu 
eu digitaria

  cp linux_gnu.def make.def

Então construa os programas e teste-os

   make test

O diretório de soluções usa o mesmo arquivo make.def, então para construir
as soluções, basta digitar "make test".  O diretório extras
contém exercícios adicionais para estudantes mais avançados.  Estes
não foram testados com o mesmo cuidado e podem ter problemas de compilação
e execução em alguns sistemas.

Testamos estes programas em Linux com os compiladores gnu e Intel,
e no Windows 7 com o compilador Intel. Também testámos estes programas
no OS-X com o ambiente gnu carregado com o xcode da Apple.   O ambiente OpenMP da Apple
ambiente OpenMP da Apple não suporta variáveis threadprivate
threadprivadas, então as soluções pi_mc não serão construídas (e precisam 
ser comentadas no makefile).

Nós usamos esses programas com o compilador PGI (pgi.def) 
mas não testámos este caso recentemente e pode precisar de algum trabalho.

Para os utilizadores do Windows, para executar estes programas no Windows 7, usámos o seguinte
procedimento.  Primeiro, vá ao menu Iniciar e seleccione 
   
    INtel parallel studio 2011/ prompt de comando/ ia64 visual studio 2010 mode

cd para a pasta apropriada.  Copie win_intel.def para make.def e depois
use o nmake para construir

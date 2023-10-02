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

## Tutoriais

+ Tim Mattson’s (Intel) [“Introduction to OpenMP”](http://tinyurl.com/OpenMP-Tutorial) (2013) on YouTube.
+ Slides: [Intro_To_OpenMP_Mattson.pdf](https://www.openmp.org/wp-content/uploads/Intro_To_OpenMP_Mattson.pdf)
+ Exercise files: [Mattson_OMP_exercises.zip](https://www.openmp.org/wp-content/uploads/Mattson_OMP_exercises.zip)
+ [An Overview of OpenMP – Ruud van der Pas – Sun Microsystems](https://www.openmp.org/wp-content/uploads/ntu-vanderpas.pdf)
+ [Hands-On Introduction to OpenMP](https://www.openmp.org/wp-content/uploads/omp-hands-on-SC08.pdf), Mattson and Meadows, from SC08 (Austin) (PDF)
 + [Code Exercises](https://www.openmp.org/wp-content/uploads/OMP_Exercises.zip) (zip)
+ [Introduction to OpenMP tutorial](http://www.llnl.gov/computing/tutorials/openMP) from Lawrence Livermore National Lab.
+ [Tutorial on OdinMP C/C++ OpenMP compiler](http://www.ecs.umass.edu/ece/andras/pact_2003_tutorials.htm#OpenMP), support for instrumentation, and the run-time system for OpenMP developed in the Intone project, PACT 2003.
+ An [OpenMP tutorial in French](http://www.idris.fr/formations/openmp/) from the French Supercomputing Center for Scientific Research.
+ [Parallel Program in Fortran 95 Using OpenMP](https://www.openmp.org/wp-content/uploads/F95_OpenMPv1_v2.pdf), by Miguel Hermanns, Universidad Politecnica de Madrid, Spain, 2002 (PDF)
+ [Portuguese tutorial about OpenMP](http://www.ppenteado.net/ast/pp_para/pp_para_on_3.pdf) from Paulo Penteado, Post doctoral researcher at Departamento de Astronomia, Instituto de Astronomia, Geofísica e Ciências Atmosféricas, Universidade de São Paulo (IAG/USP).

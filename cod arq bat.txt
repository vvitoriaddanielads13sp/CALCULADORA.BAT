@echo off
echo
title criando calculadora

echo
:inicio
echo.
echo 1 - soma
echo 2 - dif
echo 3 - mult
echo 4 - div

echo escolha uma das opcoes acima
set /p op=

if %op%==1 goto soma
if %op%==2 goto dif
if %op%==3 goto mult
if %op%==4 goto div

echo

:soma

echo digite um numero
set /p x=
echo digite outro numero
set /p y=

set /a t=%x%+%y%
@echo on o resuldato e %t%

echo deseja sair? (1=sim, 2=Nao)
set /p sair=
if %sair%==1 goto fim
if %sair%==2 goto inicio

:dif

echo digite um numero
set /p x=
echo digite outro numero
set /p y=

set /a t=%x%-%y%
@echo o resuldato e %t%

echo deseja sair? (1=sim, 2=Nao)
set /p sair=
if %sair%==1 goto fim
if %sair%==2 goto inicio


:mult

echo digite um numero
set /p x=
echo digite outro numero
set /p y=

set /a t=%x%*%y%
@echo o resuldato e %t%

echo deseja sair? (1=sim, 2=Nao)
set /p sair=
if %sair%==1 goto fim
if %sair%==2 goto inicio


:div

echo digite um numero
set /p x=
echo digite outro numero
set /p y=

set /a t=%x%/%y%
@echo o resuldato e %t%

echo deseja sair? (1=sim, 2=Nao)
set /p sair=
if %sair%==1 goto fim
if %sair%==2 goto inicio


:fim
@echo off
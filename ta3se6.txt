#!/bin/bash


echo "***************************************"
echo "*                Menu                 *"
echo "*      1. Crear archivo               *"
echo "*      2. Eliminar archivo            *"
echo "*      3. Salir                       *"
echo "***************************************"

echo "Ingrese opcion: "
read opcion
claer

case $opcion in
	1)
		echo"************************"
		echo"*     CREAR ARCHIVO    *"
		echo"************************"
		echo "Ingrese nombre del archivo"
		read archivo

		touch $HOME/Documents/$archivo
		echo "Creado correctamente"

echo "***************************************"
echo "*                Menu                 *"
echo "*      1. Crear directorio            *"
echo "*      2. Eliminar diretorio          *"
echo "*      3. Crear archivo               *"
echo "*      4. Salir                       *"
echo "***************************************"

echo "Ingrese opcion: "
read opcion
claer

	;;

	2)
		clear
		echo"************************"
		echo"*  ELIMINAR ARCHIVO    *"
		echo"************************"
		echo "Ingrese nombre del directorio"
		read directorio

		rmdir $HOME/Documents/$directorio
		echo "Directorio eliminado correctamente"

echo "***************************************"
echo "*                Menu                 *"
echo "*      1. Crear directorio            *"
echo "*      2. Eliminar diretorio          *"
echo "*      3. Crear archivo               *"
echo "*      4. Salir                       *"
echo "***************************************"

echo "Ingrese opcion: "
read opcion
claer

	;;

	3)
		exit
	;;

	*)
		echo "Opcion no valida"
	;;
esac
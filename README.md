# PROYECTO PROGRAMACION 2

###### UNIVERSIDAD DE INVESTIGACION Y DESARROLLO
###### AUTORES: Nicolas E. Martinez - Alexander Leon
###### GRUPO: 4L  

###### DOCENTE: Michael Sneider Puentes Palacio


###### PROYECTO DE PROGRAMACIÓN 2 
###### SEGUNTO CORTE

## Contenido

1. [Expecificaciones del programa.](#Expecificaciones-del-programa)
2. [Herramientas de programación.](#Herramientas-de-programación)
3. [Paso a Paso Instalacion del Programa:](#Paso-a-Paso-Instalacion-del-Programa)
4. [Herramientas utilizadas.](#herramientas-utilizadas)
5. [YOUTUBE Video Funcionamineto.](#YOUTUBE-Video-Funcionamineto)

### Expecificaciones del programa.
El programa esta desarrollado en el lenguaje de programacion C# (pronunciado si sharp en inglés) es un lenguaje de programación multiparadigma desarrollado y estandarizado por Microsoft como parte de su plataforma .NET, que después fue aprobado como un estándar por la ECMA (ECMA-334) e ISO (ISO/IEC 23270). C# es uno de los lenguajes de programación diseñados para la infraestructura de lenguaje común.

Su sintaxis básica deriva de C/C++ y utiliza el modelo de objetos de la plataforma .NET, similar al de Java, aunque incluye mejoras derivadas de otros lenguajes.

### Herramientas de programación

![Visual_Studio_2012_logo_and_wordmark svg](https://user-images.githubusercontent.com/62104633/81871471-795e7a80-953d-11ea-9227-64361e236c14.png)

El trabajo se desarrollo y se codifico con Microsoft Visual Studio el cual es un entorno de desarrollo integrado (IDE, por sus siglas en inglés) para Windows, Linux y macOS. Es compatible con múltiples lenguajes de programación, tales como C++, C#, Visual Basic .NET, F#, Java, Python, Ruby y PHP, al igual que entornos de desarrollo web, como ASP.NET MVC, Django, etc., a lo cual hay que sumarle las nuevas capacidades en línea bajo Windows Azure en forma del editor Monaco.

### Paso a Paso Instalacion del Programa:

Instalar este software, es my sencillo y no te tomara nada de tiempo hacer.

Sigue detenidamente los siguietes pasos:

1. Todos los archivos necesarios estan disponibles en un mismo documento que se encuentra adjunto (.rar), para descargar este comprimido desbes situarte en la parte superior del proyecto, veras un recuadro verde como en la imagen.

   ![Ima1](https://user-images.githubusercontent.com/62104633/81880706-bd5c7a00-9553-11ea-9aeb-1851dc846820.jpg)
 
2. Selecciona o da click en ***`Clone or download`*** (Boton Verde) para ver las opciones de descarga y seleccionamos la opción ***`Download ZIP`*** para poder descargar el software.

   ![Ima2](https://user-images.githubusercontent.com/62104633/81880952-7753e600-9554-11ea-98df-7b0fdf2e112c.jpg) 

3. Se visualizara un cuadro donde deberas seleccionar ***`Download ZIP`*** y automaticamente se comenzara a descargar el archivo.

   ![Sin título-3](https://user-images.githubusercontent.com/62104633/81882321-129a8a80-9558-11ea-959c-1592afe23ecb.jpg)

4. Al descargarlo, se mostrara reflejado en la parte inferior del navegador el archivo .rar 

   ![Sin título-4](https://user-images.githubusercontent.com/62104633/81882578-b5eb9f80-9558-11ea-9f02-1755974bc3c1.jpg)
  
5. Al descargarlo, nos dirigimos al lugar donde quedó descargado el software y descomprimimos el archivo. Al tener ya descomprimido el archivo, abrimos la carpeta y descomprimimos también los dos archivos que aparecen comprimidos.
  
   ![Captura4](https://user-images.githubusercontent.com/62104633/81882855-58a41e00-9559-11ea-8934-400ff08b75bf.PNG)

6. Antes poner a correr el programa debemos descomprimir los archivos de los diferentes idiomas que se encuentran comprimidos.

![Sin título-5](https://user-images.githubusercontent.com/62104633/81883171-20e9a600-955a-11ea-81a9-68a7cb72e8ab.jpg)

7. Ahora a disfrutar, abre el archivo .exe que dice **Trabajo**, se abrira en una pestalla nueva el programa.

   ![Captura6](https://user-images.githubusercontent.com/62104633/81884030-66a76e00-955c-11ea-8619-e4b7bddbcf5f.PNG)
   
   
### Herramientas utilizadas   

Para el diseño del Form1 utilizamos cuadros de herramientas como: ***`TextBox`***, ***`Button`***, ***`Label`***, ***`GropuBox`***, ***`ComboBox`***, ***`FlowLayout`***, ***`Panel`***, ***`ColorDialog`***.

![1](https://user-images.githubusercontent.com/62104633/81881813-c00c9e80-9556-11ea-82ba-bf0bfd58ca06.jpg)

Cada ***`Label`*** utilizado pauta la indicación de lo que el usuario debe hacer.
El label **`"Seleccionar idioma"`** indica que el usuaio debe elegir el idioma que desee, acontinuación, del ***`ComboBox`*** se despliegan una serie de idiomas disponibles.

![Select_Idiom](https://user-images.githubusercontent.com/62104695/81875950-21c50c80-9547-11ea-98cf-c6c137caaab8.png)


```
Utilizamos el siguiente código para programar el Idioma:
private void CB_Idioma_SelectedIndexChanged(object sender, EventArgs e)
        {
            if (CB_Idioma.SelectedIndex == 0)
            {
                //Idioma español
                Thread.CurrentThread.CurrentUICulture = new CultureInfo("es-CO");
                Renombrar();
            }
            else if (CB_Idioma.SelectedIndex == 1)

            {
                //Idioma inglés
                Thread.CurrentThread.CurrentUICulture = new CultureInfo("en-US");
                Renombrar();
            }
            else if (CB_Idioma.SelectedIndex == 2)
            {
                //Idioma francés
                Thread.CurrentThread.CurrentUICulture = new CultureInfo("fr-FR");
                Renombrar();
            }
        }
        
  ```      
En este caso, seleccionamos el idioma Inglés, por la tanto, el idioma para todo el software cambia al idioma seleccionado (en nuestro caso, inglés).

![FORM1_INGL](https://user-images.githubusercontent.com/62104695/81875994-40c39e80-9547-11ea-8ab8-6a6e9aa78eab.JPG)

Dentro del ***`GroupBox`*** **`"Introduce data"`**, añadimos ***`Labels`*** y ***`TextBox`*** los cuales corresponden a los datos requeridos para el Registro de computadores. Cada **`Label`** indica la información que el usuario debe añadir en su respectivo **`TextBox`**, por ejemplo: "Brand name", "Procesador type", "Storage capacity" Al final encontramos el notón **`"Enterokay"`**, el cual registrará cada uno de los computadores una vez el usuario haya dado click en este.

![2](https://user-images.githubusercontent.com/62104633/81881971-298cad00-9557-11ea-8347-4de0203eaf5f.jpg)

En el ***`GroupBox`*** ***`"Add Numbers"`***, está la DLL para la suma de una cadena de números, podemos encontrar 2 Labels con su respectivo TextBox y un **`Button`**, en el primer **`TextBox`** se debe ingresar una cadena de números y en el segundo **`TextBox`** se mostrará el resultado de la suma de dicha cadena numérica una vez el usuario haya dado click en el Button ***`"Calculate".`***

![3](https://user-images.githubusercontent.com/62104633/81882098-796b7400-9557-11ea-9aac-ff903cccde50.jpg)

![suma](https://user-images.githubusercontent.com/62104695/81884140-abcba000-955c-11ea-9e95-de07a0a9dae3.JPG)

En la parte superior, podemos encontrar un ***`Button`*** de ayuda **`"Help"`**, al darle click se abrirá una ventana donde el usuario podrá escribir el problema que presenta 

![HELP](https://user-images.githubusercontent.com/62104695/81871152-dc9bdd00-953c-11ea-8c81-d47d53c23a2a.JPG)

Además, con el ***`Button`*** "Color", el usuario podrá elegir el color que más sea de su agrado mientras realiza el registro de los datos del computador

![Color1](https://user-images.githubusercontent.com/62104695/81870913-7020de00-953c-11ea-9c9c-02d9caa44ea5.JPG)
**`Seleccionamos el color verde`**
![Color2](https://user-images.githubusercontent.com/62104695/81870914-70b97480-953c-11ea-8d8e-1a75b7a5ec80.JPG)

Esto se logra con la siguiente condición:

```
if (colorDialog1.ShowDialog() == DialogResult.OK)
            {
                base.BackColor = colorDialog1.Color;
                CS_Valid.miColor = colorDialog1.Color;
            }
```

Algunos TextBox, como el "Brand name", tienen la validación de que cada vez que ese campo sea llenado, convierta todo su texto en mayúscula. Esto se logra hacer con la siguiente función:

``` 
private void TB_Nom_Marca_Leave(object sender, EventArgs e)
        {
            TB_Nom_Marca.Text = TB_Nom_Marca.Text.ToUpper();
        }  
 ```      
Además todos los TextBox cuentan con algunas validaciones, una de ellas es que todos los campos son obligatorios, en caso de saltarse alguna casilla, se mostrará un mensaje por pantalla donde se indica que ***no pueden ir campos vacíos***

![OBLIGATORIO](https://user-images.githubusercontent.com/62104695/81872836-34881300-9540-11ea-8ef0-9687e8450fbd.JPG)

Los TextBox en los que se debe ingresar los datos de la **`memoria RAM`** y del **`Procesador`** deben ser numéricos, de lo contrario, se mostrará un mensaje por pantalla indicando que ese campo únicamente puede ser numérico

![VALID_NUM1](https://user-images.githubusercontent.com/62104695/81872838-3520a980-9540-11ea-9b06-24b01c4f71c4.JPG)
![VALID_NUM2](https://user-images.githubusercontent.com/62104695/81872835-33ef7c80-9540-11ea-9708-d7a5d1ff8226.JPG)

Siguiendo con las herramientas utilizadas, dentro del ***`FlowLayout`*** incluimos un **`UserControl`**, el **`UserControl`** recibe la información proveniente del Form1 y muestra el nombre del computador registrado. Cada **`UserControl`** tiene en la parte superior derecha un número, el cual indica la cantidad de computadores registrados

![UC](https://user-images.githubusercontent.com/62104695/81876830-34404580-9549-11ea-9558-45a10b5f26b4.JPG)

Este **`UserControl`** tiene un ***`Button`*** el cual permite mostrar la información ya incluida; una vez el usuario de click en ese Button, podrá ver los datos que ya incluyó y si tuvo algún tipo de error en dicha inclusión, podrá realizar actualizaciones a esos datos

![FORM_2](https://user-images.githubusercontent.com/62104695/81877959-32c44c80-954c-11ea-8196-fdee555f5a97.JPG)
**`Actualizacion de datos:`**
![FORM_2 1](https://user-images.githubusercontent.com/62104695/81878059-7cad3280-954c-11ea-84af-c5c709b0d9ba.JPG)


Además de esto, se mostrará una gráfica referente al **`"nombre de la marca" `** VS **` "el respectivo almacenamiento" `** y también actualizará su gráfica una vez el usuario haya actualizado la información
```
Esta línea de código permite alimentar a la gráfica
 miGrafica.AñadirDatos(TB_Nom_Marca.Text, int.Parse(TB_Almacen.Text));
```
![DLL_1](https://user-images.githubusercontent.com/62104695/81878157-d44b9e00-954c-11ea-8dfd-2f5966a375d2.JPG)
       
![DLL_2](https://user-images.githubusercontent.com/62104695/81878254-1ffe4780-954d-11ea-8679-2371671672d5.JPG)

**`Actualizacion de datos:`**
```
Esta función permite la actualización de la gráfica
 public void actualizarChart(int posicion,  string NomMarca, int almacen)
        {
            chart1.Series[0].Points.ElementAt(posicion).SetValueXY( NomMarca, almacen);
            chart1.ChartAreas[0].RecalculateAxesScale();
        }
 ```

El ***`Button`*** **`"Hide/Show"`** permite mostrar u ocultar la etiqueta del "almacenamiento"
![HIDE_SHOW](https://user-images.githubusercontent.com/62104695/81878409-8e430a00-954d-11ea-9463-5fb6cf255099.JPG)

Cada ***`UserControl`*** contiene registrado 1 computador elegido por el usuario, cada uno con su respectiva gráfica
![FORM_2 2](https://user-images.githubusercontent.com/62104695/81878615-2e992e80-954e-11ea-9130-4214a0b78852.JPG)


### YOUTUBE Video Funcionamineto.

En el siguiente enlace podra encontrar un video subido a la plataforma de Youtube en el cual se muestra y se explica todo el funcionamiento del programa, lo que hace, la demostracion de las graficas, del registro, de las actualizaciones, los diferente idiomas, la configuracion visual del programa (cambio de color), las ayudas por problemas o errores entre mas.

https://youtu.be/IfwpBuUyS0o

![Captura_Youtube](https://user-images.githubusercontent.com/62104633/81884592-e41fae00-955d-11ea-9386-ed082f923206.PNG)


   

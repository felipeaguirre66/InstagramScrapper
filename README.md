# InstagramScrapper

This code allows the user to scrape any public instagram account's followers and follows. It downloads them into an excel file.

There is a request limit, which is not possible to predict, but it is around 10,000 and 15,000 followers/follows per day.

The current project involves scrapping all Argentinans politicians followings, and create a net to visualite how they cluster.


# Obtencion del instagram de diputados y senadores
Senadores:
https://www.senado.gob.ar/senadores/listados/listaSenadoRes

Diputados:
https://www.hcdn.gob.ar/diputados/listadip.html

Método:
A. Obtener todos los instagrams disponibles en los links mencionados.
B. Para quienes no se obtuvo un Instagram, se realizó lo siguiente:
1. Buscar su nombre en Google, precedido por la palabra “senador” o “diputad” (según corresponda) y seguido de la palabra “Instagram”.
2. Tomar todos los links resultantes de la búsqueda que sean links de Instagram.
3. Utilizar le método “process.extractBests” para encontrar la mejor coincidencia con el nombre entre todos los candidatos, y dicha coincidencia debe arrojar un puntaje mayor a 70.
4. Entrar al perfil y evaluar que tenga una de las palabras clave: 'senado','diputad','politic','medic','abogad'.
